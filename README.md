<h3 align="center">
	<img src="https://raw.githubusercontent.com/catppuccin/catppuccin/dev/assets/logos/exports/1544x1544_circle.png" width="100" alt="Logo"/><br/>
	<img src="https://raw.githubusercontent.com/catppuccin/catppuccin/dev/assets/misc/transparent.png" height="30" width="0px"/>
	Catppuccin's Style Guide
	<img src="https://raw.githubusercontent.com/catppuccin/catppuccin/dev/assets/misc/transparent.png" height="30" width="0px"/>
</h3>

<h6 align="center">
  <a href="https://github.com/catppuccin/style-guide#-ports">Ports</a>
  ·
  <a href="https://github.com/catppuccin/style-guide#-terminals">Terminals</a>
  ·
  <a href="https://github.com/catppuccin/style-guide#-code-editors">Code Editors</a>
</h6>

<p align="center">
    <a href="https://github.com/catppuccin/style-guide/stargazers"><img src="https://img.shields.io/github/stars/catppuccin/style-guide?colorA=1e1e28&colorB=c9cbff&style=for-the-badge&logo=starship style=for-the-badge"></a>
    <a href="https://github.com/catppuccin/style-guide/issues"><img src="https://img.shields.io/github/issues/catppuccin/style-guide?colorA=1e1e28&colorB=f7be95&style=for-the-badge"></a>
    <a href="https://github.com/catppuccin/style-guide/contributors"><img src="https://img.shields.io/github/contributors/catppuccin/style-guide?colorA=1e1e28&colorB=b1e1a6&style=for-the-badge"></a>
</p>

<p align="center">
	A guide on how to properly style and implement the Catppuccin palette on various things such as terminal emulators, user interfaces, code editors, etc...
</p>

# 🍉 Ports

## Creation

You can create ports using [this](https://github.com/catppuccin/template) public template as a blueprint. However, you shouldn't create them the traditional way (by clicking **Use this template**), because this leaves a _small_ tag under the repos' name that says `generated from <template>`. To avoid this, follow the instructions below:

1. Create the repo and leave it empty
2. Add this template as a remote: `git remote add template git@github.com:catppuccin/template.git`
3. Pull from it: `git pull template main --depth=1`
4. Delete the remote: `git remote remove template`

## Styling Rules

-   The name of the repo must be the simplest version of the app's name (e.g `nvim` instead of `NeoVim`)
-   Put the images under `assets/`. If there are a bunch of them consider [creating an empty branch](https://gist.github.com/joncardasis/e6494afd538a400722545163eb2e1fa5) (e.g. `assets`) and storing them there.
-   Format the repo's description as "`<allusive emoji>` Vibrant pastel theme for App"
-   Add `catppuccin` to the topics.
-   Uppercase meta files (e.g. `README.md`)
-   Don't add health files (like `CODE_OF_CONDUCTS.md` or `SUPPORT.md`), those are organization-wide files stored [here](https://github.com/catppuccin/.github).
-   Emojis are _the way_, feel free to use them as much as you want.

# 🦄 General Standard

These are general use cases for most of the palette relevant for user interfaces. The `function` expresses a very vague use-case of a color and the `scope example` how it is generally used:

| Function     | Scope Examples                     | Color     | Color Hex  |                                                                          |
| ------------ | ---------------------------------- | --------- |------------|------------------------------------------------------------------------- |
| `base`       | `splits`; `sign columns`           | black0    | `#161320`  | <img src="assets/palette/circles/black0.png" height="23" width="23"/>    |
| `surface`    | `x`                                | black1    | `#1A1826`  | <img src="assets/palette/circles/black1.png" height="23" width="23"/>    |
| `top`        | `background`                       | black2    | `#1E1E2E`  | <img src="assets/palette/circles/black2.png" height="23" width="23"/>    |
| `overlay`    | `floating elements`; `cursor line` | black3    | `#302D41`  | <img src="assets/palette/circles/black3.png" height="23" width="23"/>    |
| `standout`   | `searches`                         | black4    | `#575268`  | <img src="assets/palette/circles/black4.png" height="23" width="23"/>    |
| `subtle`     | `comments`                         | gray0     | `#6E6C7E`  | <img src="assets/palette/circles/gray0.png" height="23" width="23"/>     |
| `active`     | `foreground`                       | white     | `#D9E0EE`  | <img src="assets/palette/circles/white.png" height="23" width="23"/>     |
| `inactive`   | `x`                                | gray2     | `#C3BAC6`  | <img src="assets/palette/circles/gray2.png" height="23" width="23"/>     |
| `projection` | `cursors`                          | rosewater | `#F5E0DC`  | <img src="assets/palette/circles/rosewater.png" height="23" width="23"/> |

# 🎃 Terminals

## Main

#### Normal

| Scope    | Color  |
| -------- | ------ |
| `color0` | gray0  |
| `color1` | red    |
| `color2` | green  |
| `color3` | yellow |
| `color4` | blue   |
| `color5` | pink   |
| `color6` | sky    |
| `color7` | gray2  |

#### Bright

| Scope     | Color  |
| --------- | ------ |
| `color8`  | gray1  |
| `color9`  | red    |
| `color10` | green  |
| `color11` | yellow |
| `color12` | blue   |
| `color13` | pink   |
| `color14` | sky    |
| `color15` | white  |

#### Extended Colors

| Scope     | Color     |
| --------- | --------- |
| `color16` | peach     |
| `color17` | rosewater |

## UI

#### Misc

| Scope         | Color     |
| ------------- | --------- |
| `cursor`      | rosewater |
| `cursor text` | black2    |
| `urls`        | rosewater |

#### Window

| Scope             | Color    |
| ----------------- | -------- |
| `active border`   | lavender |
| `inactive border` | black4   |
| `bell border`     | yellow   |

#### Tabs

| Scope                     | Color  |
| ------------------------- | ------ |
| `active tab foreground`   | pink   |
| `active tab background`   | black4 |
| `inactive tab foreground` | white  |
| `inactive tab background` | black2 |

## Syntax

| Scope                  | Color  |
| ---------------------- | ------ |
| `foreground`           | white  |
| `background`           | black2 |
| `selection foreground` | white  |
| `selection background` | black4 |
| `mark1 foreground`     | black2 |
| `mark1 background`     | blue   |
| `mark2 foreground`     | black2 |
| `mark2 background`     | pink   |
| `mark3 foreground`     | black2 |
| `mark3 background`     | teal    |

# 🍨 Code Editors

## Syntax

(WIP)

&nbsp;

<p align="center"><img src="https://raw.githubusercontent.com/catppuccin/catppuccin/dev/assets/footers/gray0_ctp_on_line.svg?sanitize=true" /></p>
<p align="center">Copyright &copy; 2020-present <a href="https://github.com/catppuccin" target="_blank">Catppuccin Org</a>
<p align="center"><a href="https://github.com/catppuccin/catppuccin/blob/main/LICENSE"><img src="https://img.shields.io/static/v1.svg?style=for-the-badge&label=License&message=MIT&logoColor=d9e0ee&colorA=302d41&colorB=c9cbff"/></a></p>
