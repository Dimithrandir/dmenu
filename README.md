# Dimthrandir's build of dmenu

My modified build of [suckless](https://suckless.org/)' [dmenu](https://tools.suckless.org/dmenu/).

Built on version 5.3.

## Features

### Emoji font

Default emoji font is added to the configuration so all emojis are properly displayed.

This font and its features can be changed with option `-fne`.

### Full item width

When dmenu lists item vertically with a given prompt, items can optionaly fill the whole width of dmenu with `-t`.

### [border](https://tools.suckless.org/dmenu/patches/border/) patch

version [dmenu-border-20230512-0fe460d](https://tools.suckless.org/dmenu/patches/border/dmenu-border-20230512-0fe460d.diff)

Applied as is.

### [center](https://tools.suckless.org/dmenu/patches/center/) patch

version [dmenu-center-20250407-b1e217b.diff](https://tools.suckless.org/dmenu/patches/center/dmenu-center-20250407-b1e217b.diff)

Appear at the top of screen by default.

dmenu is centered vertically only when `-c` is used.

The minimal width of dmenu when centered can be set with `-mw`.

### [highlight](https://tools.suckless.org/dmenu/patches/highlight/) patch

version [dmenu-highlight-20201211-fcdc159.diff](https://tools.suckless.org/dmenu/patches/highlight/dmenu-highlight-20201211-fcdc159.diff)

Highlight colors can be set with options  `-nhf` `-nhb` `-shf` `-shb`.

### [numbers](https://tools.suckless.org/dmenu/patches/numbers/) patch

version [dmenu-numbers-20220512-28fb3e2.diff](https://tools.suckless.org/dmenu/patches/numbers/dmenu-numbers-20220512-28fb3e2.diff)

Numbers can be enabled with option `-n`.

### Usage instructions

`man`, `help` and `usage` are updated with the new options.

## Requirements

In order to build dmenu you need the Xlib header files.

## Installation

Edit config.mk to match your local setup (dmenu is installed into the /usr/local namespace by default).

Afterwards enter the following command to build and install dmenu (if necessary as root):

    make clean install

## Running dmenu

See the man page for details.
