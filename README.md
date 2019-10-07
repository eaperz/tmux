# tmux cookbook
## Sessions
### Start a new session
```bash
$ tmux
```

### Start new with session name
```bash
$ tmux new -s session_name
```

### Attach
```bash
$ tmux attach
```

### Attach to named
```bash
$ tmux attach -t session_name
```

### List sessions
```bash
$ tmux ls
```

### Kill session
```bash
$ tmux kill-session -t session_name
```

## Setting Vi mode in tmux
You can enable this as a default setting in .tmux.conf with the following:

```
set-window-option -g mode-keys vi
```

## Scrolling down and up
```
ctrl + b then hit [
Now you can scroll down and up using keyboard arrows
Hit q to exit scroll mode
```

## ctrl+b
In tmux, hit the prefix `ctrl+b` and then:

```
# Sessions
    :new<CR>  new session
    s  list sessions
    $  name session
    d  detach session
    ?  list shortcuts

# Windows tabs
    c  create window
    w  list windows
    n  next window
    p  previous window
    f  find window
    ,  name window
    &  kill window

# Panes splits
    %     vertical split
    "     horizontal split

    o     swap panes
    q     show pane numbers, when the numbers show up type the key to goto that pane
    x     kill pane
    +     break pane into window (e.g. to select text by mouse to copy)
    -     restore pane from window
    space toggle between layouts
    {     move the current pane left
    }     move the current pane right
    z     toggle pane zoom
```

__source: https://gist.github.com/MohamedAlaa/2961058__
