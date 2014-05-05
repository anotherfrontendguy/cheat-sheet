## Tmux

[must-haves](http://robots.thoughtbot.com/a-tmux-crash-course#must-haves)

```sh
# remap prefix to Control + a
set -g prefix C-a
unbind C-b
bind C-a send-prefix

# force a reload of the config file
unbind r
bind r source-file ~/.tmux.conf

# quick pane cycling
unbind ^A
bind ^A select-pane -t :.+
```

### Splits

| Key           | Action          |
|:--------------|:----------------|
| prefix + %    | vertical split  |
| prefix + "    | horizontal split|

### Window Management

| Key           | Action               |
|:------------- |:-------------------- |
| prefix + c    | new window           |
| prefix + n    | next window          |
| prefix + p    | previous window      |
| prefix + w    | choose window        |
| prefix + z    | toggle fullscreen    |
| prefix + &    | confirm kill window  |
| prefix + ,    | rename window        |

### Session Management

| Key           | Action               |
|:------------- |:-------------------- |
| prefix + d    | detach from session |
| prefix + (    | switch to previous session |
| prefix + )    | switch to next session |
| prefix + L    | last used session |
| prefix + s    | display session list (move with arrow keys, enter to attach to a session |
| prefix + $    | rename current session |


### not yet ordered
prefix + alt + 5 = copy mode -> V select -> Y yank

## Terminal

| Key   | Action                                                         |
|:------|:-------------------------------------------------------------- |
| ⌃A    | moves to the start of the line                                 |
| ⌃B    | move back one character                                        |
| ⌃E    | moves to the end of the line                                   |
| ⌃F    | move forward one character                                     |
| ⌃K    | delete from the cursor to the end of the line                  |
| ⌃U    | delete from the cursor to the beginning of the line            |
| ⌃W    | delete from the cursor to the beginning of the current word    |

esc+B: move back one word  
esc+F: move forward one word

### Non-Recursive Find

e.g. list all .dotfiles in your home directory  
*note: if you symlink your dotfiles (e.g. with [rcm](https://github.com/thoughtbot/rcm))
you would have to exchange `-type f` with `-type l`*

```sh
find ~ -maxdepth 1 -type f -name ".*"
```

## Sublime

| Key    | Action                                                         |
|:-------|:-------------------------------------------------------------- |
| ⌃⌘↑    | move line/selection up                                         |
| ⌃⌘↓    | move line/selection do wn                                      |
| ⇧⌘↵    | insert line before                                             |
| ⌘X     | delete line                                                    |
| ⌃M     | jump to matching brack et                                      |
| ⇧⌃M    | select between current  parantheses                            |
