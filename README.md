# tmux
紀錄 tmux 設定檔

## Mac OS
```
# creat .tmux.conf file 
vim ~/.tmux.conf

# reload tmux config
tmux source-file ~/.tmux.conf

# list tmux sessions
tmux ls
```

## Changes
- Change prefix from 'Ctrl+B' to 'Ctrl+A'
- Using the mouse on a pane

### tmux-plugins/tmux-pain-control

#### Navigation

- `prefix + h` and `prefix + C-h`<br/>
  select pane on the left
- `prefix + j` and `prefix + C-j`<br/>
  select pane below the current one
- `prefix + k` and `prefix + C-k`<br/>
  select pane above
- `prefix + l` and `prefix + C-l`<br/>
  select pane on the right


**Note**: This overrides tmux's default binding for toggling between last
active windows, `prefix + l`.
[tmux-sensible](https://github.com/tmux-plugins/tmux-sensible) gives you
a better binding for that, `prefix + a` (if your prefix is `C-a`).


#### Resizing panes

- `prefix + shift + h`<br/>
  resize current pane 5 cells to the left
- `prefix + shift + j`<br/>
  resize 5 cells in the down direction
- `prefix + shift + k`<br/>
  resize 5 cells in the up direction
- `prefix + shift + l`<br/>
  resize 5 cells to the right

These mappings are `repeatable`.

The amount of cells to resize can be configured with `@pane_resize` option. See
[configuration section](#configuration) for the details.


<img align="right" src="/screenshots/pane_splitting.gif" alt="pane splitting"/>

#### Splitting panes

- `prefix + |`<br/>
  split the current pane into two, left and right.
- `prefix + -`<br/>
  split the current pane into two, top and bottom.
- `prefix + \`<br/>
  split current pane full width into two, left and right.
- `prefix + _`<br/>
  split current pane full height into two, top and bottom.

Newly created pane always has the same path as the original pane.


#### Swapping windows

- `prefix + <` - moves current window one position to the left
- `prefix + >` - moves current window one position to the right


## Plugin
- [tmux-plugins/tpm](https://github.com/tmux-plugins/tpm)
- [tmux-plugins/tmux-sensible ](https://github.com/tmux-plugins/tmux-sensible)
- [tmux-plugins/tmux-yank](https://github.com/tmux-plugins/tmux-yank)
- [wfxr/tmux-power](https://github.com/wfxr/tmux-power)
- [tmux-plugins/tmux-prefix-highlight](https://github.com/tmux-plugins/tmux-prefix-highlight)
- [tmux-plugins/tmux-pain-control](https://github.com/tmux-plugins/tmux-pain-control)

