# Personal tmux Configuration README

No-nonsense configuration for tmux.

## Configuration Features

### Vi-style Scrollback

- **Mode**: Vi mode enabled for scrollback.
- **Key Bindings**:
  - `v`: Begin text selection.
  - `V`: Select entire line.
  - `y`: Copy selected text.
  - Mouse drag will not exit copy mode.

### General Settings

- **Escape Time**: No delay for escape key sequences.
- **Mouse Support**: Mouse interactions enabled.
- **Window Indexing**: Starts from 1.
- **Scrollback Limit**: History limited to 10,000 lines.

### Tmux Plugins

- **TPM**: Tmux Plugin Manager for handling plugins.
- **Installed Plugins**:
  - `vim-tmux-navigator`: Navigate panes and Vim/Neovim using `Ctrl-hjkl`.
  - `tmux-resurrect`: Persist tmux sessions after computer restart.
  - `tmux-continuum`: Auto-save sessions every 15 minutes.
- **Resurrect and Continuum Settings**: Capture pane contents and enable automatic restore
  functionality.

### Key Bindings

- **Prefix**: Set to `Ctrl-b`.
- **Clear Screen**: `Ctrl-l`.
- **Split Panes**: Vertical with `-`, horizontal with `|`.
- **Reload Config**: Press `r` to reload tmux configuration.
- **Pane Resizing**: Use `h`, `j`, `k`, `l` with repeatable resize commands.
- **Maximize Pane**: `m` to toggle pane maximization.
- **Sessionizer**: `f` to launch a custom sessionizer script.
- **Safe Kill-Session**: `X` to confirm before killing a session.

### TMUX Plugin Manager

- Initialized at the end of the tmux configuration file.

## Dependencies

- Requires a script to be places at `tmux neww ~/.config/scripts/tmux-sessionizer.sh`
  (unapologetically stolen from [@ThePrimeagen](https://github.com/ThePrimeagen))
- Ensure TPM and listed plugins are installed in `~/.tmux/plugins/`.

---

**Note:** This configuration is tailored for users who prefer Vim-style navigation and requires
familiarity with tmux and its plugin ecosystem for optimal usage.
