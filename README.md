# dmenu - dynamic menu

dmenu is an efficient dynamic menu for X.

## dwrik's build

This is my build of dmenu from suckless. This build of dmenu includes the following patches:

- allow-color-fonts - enables colored fonts and emojis
- fuzzymatch - enables fuzzy string matching

This build also requires `libxft-bgra`, a patched version of `libxft`. Due to an issue in `libxft` dmenu crashes on trying to render emojis. Hence the patched version is required till the issue gets fixed upstream.

## Requirements

In order to build dmenu you need the Xlib header files.

## Installation

Edit config.mk to match your local setup (dmenu is installed into
the /usr/local namespace by default).

Afterwards enter the following command to build and install dmenu
(if necessary as root):
```
make clean install
```

## Running dmenu

See the man page for details.
