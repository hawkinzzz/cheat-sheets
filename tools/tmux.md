# Tmux
tmux is a terminal multiplexer: it enables a number of terminals to be created, accessed, and controlled from a single screen. tmux may be detached from a screen and continue running in the background, then later reattached.

Github Repo: [Tmux Source Code](https://github.com/tmux/tmux)
Documentation: [Documentation | Tmux](https://github.com/tmux/tmux/wiki)

## Installation

### Ubuntu
```bash
sudo apt -y install tmux
```

## Cheatsheet
Source: [Tmux Cheat Sheet & Quick Reference](https://tmuxcheatsheet.com)

### Sessions
#### Start a new session
```bash
tmux
```

#### Start a new session with the name _mysession_
```bash
tmux new -s mysession
```

#### kill/delete session _mysession_
```bash
tmux kill-session -t mysession
```

#### Rename Session
``ctrl`` + ``b``   ``$``

#### Detatch from session
``ctrl`` + ``b``   ``d``

#### Show all sessions
```bash
tmux ls
```

#### Attach to a session with the name _mysession_
```bash
tmux a -t mysession
```

#### Move to previous session
``ctrl`` + ``b``   ``(``

#### Move to next session
``ctrl`` + ``b``   ``)``

### Panes
#### Split plane horizontally
``ctrl`` + ``b``   ``%``

#### Split plane vertically
``ctrl`` + ``b``   ``"``

#### Move the current pane left
``ctrl`` + ``b``   ``{``

#### Move the current pane right
``ctrl`` + ``b``   ``}``

#### Switch pane to the direction (arrow)
``ctrl`` + ``b``   ``up``
``ctrl`` + ``b``   ``down``
``ctrl`` + ``b``   ``left``
``ctrl`` + ``b``   ``right``

#### Resize current pane height(holding second key is optional)
``Ctrl`` + ``b`` + ``up``
``Ctrl`` + ``b``   ``Ctrl`` + ``up``
``Ctrl`` + ``b`` + ``down``
``Ctrl`` + ``b``   ``Ctrl`` + ``down``

#### Resize current pane width(holding second key is optional)
``Ctrl`` + ``b`` + ``right``
``Ctrl`` + ``b``   ``Ctrl`` + ``right``
``Ctrl`` + ``b`` + ``left``
``Ctrl`` + ``b``   ``Ctrl`` + ``left``

#### Close current pane
``Ctrl`` + ``b``   ``x``

### Misc
#### Enter command mode
``Ctrl`` + ``b``   ``:``

#### Enable mouse mode ([More info](https://github.com/tmux/tmux/wiki/Getting-Started#using-the-mouse))
```bash
: set mouse on
```
