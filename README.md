# st

This is my patched version of st. The base version is directly from suckless.org.

## Patches

The list below shows the currently applied patches to the master branch.

- st-alpha-0.8.2.diff (adds transparency)
- st-anysize-0.8.1.diff (st leaves no gaps if the height/width doesn't match a multiple of character height)
- st-font2-20190416-ba72400.diff (allows to set multiple spare fonts as fallback)
- st-scrollback-0.8.2.diff (add scrollback functionality)

## Hotkeys

There are various shortcuts and hotkeys used in this version. Included in my build are the following.

| ModKey | Shift | Key     | Function        |
|--------|-------|---------|-----------------|
| Alt    |       | Break   | Send break      |
| Alt    |       | Print   | Toggle printer  |
| Alt    |       | Print   | Print screen    |
|        | Shift | Insert  | Clipboard paste |
| Alt    |       | c       | Clipboard copy  |
| Alt    |       | v       | Clipboard paste |
| Alt    |       | p       | Selected paste  |
| Alt    |       | NumLock | Toggle Numlock  |
| Alt    |       | k       | Scroll up       |
| Alt    |       | j       | Scroll down     |
| Alt    | Shift | u       | Zoom in         |
| Alt    | Shift | i       | Zoom out        |

## Installation

To install this package you can run several commands.

### AUR

If you're on Arch you can use the Arch User Repository.
For simplicity you can use a AUR-helper such as yay.

- `yay -S st-tiyn-git`

Or you can clone it and run it by makepkg.

- `git clone https://aur.archlinux.org/st-tiyn-git.git`
- `makepkg -sirc`

### MAKE

The most basic way is to clone the repository and then invoke make.

- `git clone https://github.com/tiyn/st`
- `make clean install`
