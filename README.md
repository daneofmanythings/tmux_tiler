<div align='center'>

# tmux tiler

## Summary

enabling left stacking dynamic tiling for tmux

</div>

## Description

This plugin emulates a dynamic tiling window manager with the following format:

```
.____________________________________.
|          |                         |
|          |                         |
|   sub    |                         |
|          |                         |
|__________|                         |
|          |                         |
|          |                         |
|   sub    |          main           |
|          |                         |
|__________|                         |
|          |                         |
|    .     |                         |
|    .     |                         |
|    .     |                         | 

(The panes on the left auto scale to equal height)
```

It addss two commands:
- `tmux-tiler-open: <M-enter>`
- `tmux-tiler-close: <M-x>`

and one option that controls the default width of the main pane:
- `tmux-tiler-main-width: 60`

## Setup

Make sure you've get [tpm](https://github.com/tmux-plugins/tpm) installed.
Add this line to your tmux config file:
```
set -g @plugin 'daneofmanythings/tmux-tiler'
```

Then, reload your config with
```
<prefix>:source path/to/your/tmux.config
```
and install with `<prefix>I` (the default tpm hotkey)

## Usage

###### NOTE: RE-BINDING THE COMMANDS AND OPTION IS CURRENTLY NOT IMPLEMENTED

Use the pane open and close commands as normal and enjoy the dynamic tiling!


## Shoutouts

[tmux-plugins](https://github.com/tmux-plugins): Excellent plugin manager and beautiful code. This project is based on their repositories.

## License

This project is licensed under the MiT license
