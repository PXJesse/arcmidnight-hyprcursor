# Hyprcursor port of ArcMidnight cursors

This is a hyprcursor theme, converted from the ArcMidnight x-cursor theme by [yeyushengfan258](https://github.com/yeyushengfan258/ArcMidnight-Cursors/).

> [!NOTE]
> I claim no right to the cursors, all credit for designing these cursors goes to yeyushengfan258.

## Installation

Add the contents of the `dist` directory in this repo to your local icons folder.

```sh
mkdir -p /home/$USER/.local/share/icons
cp ./dist/ /home/$USER/.local/share/icons/ArcMidnight
```

Set the following environment variables (for example in your Hyprland config file):

```hl
env = HYPRCURSOR_SIZE,24
env = HYPRCURSOR_THEME,ArcMidnight
```

## Project structure

> [!WARNING]
> The below description is a future state I would like to create. For now, the `src` folder contains the SVG files, but
does NOT contain the `meta.hl` files per cursor. It is therefore not a usable working state!

This project contains both the working state of this Hyprcursor theme, as well as a compiled state. The working state (available
in the `src` folder) is available so users of this repository can easily view the SVGs, as well as manipulate them and compile
their own version using the [hyprcursor-util](https://github.com/hyprwm/hyprcursor/tree/main/hyprcursor-util) utility. One use
case for this is to create different color schemes of this cursor, like [SylviaBun](https://github.com/SylviaBun/ArcMidnight-Cursors-Viridian)
did using a `sed` command.

```
├── dist/
│   ├── hyprcursors/
│   │   ├── move.hlc
│   │   ├── pencil.hlc
│   │   └── ...
│   └── manifest.hl
├── src/
│   ├── hyprcursors/
│   │   ├── move/
│   │   │   ├── meta.hl
│   │   │   └── move.svg
│   │   ├── pencil/
│   │   │   ├── meta.hl
│   │   │   └── pencil.svg
│   │   └── ...
│   └── manifest.hl
└── README.md
```

