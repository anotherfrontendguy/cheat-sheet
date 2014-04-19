## Tmux

[must-haves](http://robots.thoughtbot.com/a-tmux-crash-course)

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
| :------------ |:----------------|
| prefix + %    | vertical split  |
| prefix + "    | horizontal split|

### Window Management

| Key           | Action               |
| ------------- | -------------------- |
| prefix + c    | new window           |
| prefix + n    | next window          |
| prefix + p    | previous window      |
| prefix + w    | choose window        |
| prefix + z    | toggle fullscreen    |
| prefix + &    | confirm kill window  |
| prefix + ,    | rename window        |

### not yet ordered
prefix + s = choose session  
prefix + alt + 5 = copy mode -> V select -> Y yank
