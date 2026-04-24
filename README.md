# Boffin Themes for DevOps Environment

## 1. Neovim Themes

### 1.1 Tokyonight

```bash
https://github.com/folke/tokyonight.nvim.git
```
## 2. Warp Themes

### 2.1 Tokyonight

```yaml
accent: "#7aa2f7"
background: "#1a1b26"
details: darker
foreground: "#a9b1d6"
terminal_colors:
  bright:
    black: "#363b54"
    blue: "#7aa2f7"
    cyan: "#7dcfff"
    green: "#41a6b5"
    magenta: "#bb9af7"
    red: "#f7768e"
    white: "#acb0d0"
    yellow: "#e0af68"
  normal:
    black: "#363b54"
    blue: "#7aa2f7"
    cyan: "#7dcfff"
    green: "#41a6b5"
    magenta: "#bb9af7"
    red: "#f7768e"
    white: "#787c99"
    yellow: "#e0af68"
```

## 3. K9s Themes

### 3.1 Tokyonight

```yaml
# -----------------------------------------------------------------------------
#  tokyo night
# -----------------------------------------------------------------------------

foreground: &foreground "#a9b1d6"
background: &background "#1a1b26"
current_line: &current_line "#1e202e"
selection: &selection "#515c7e"
comment: &comment "#51597d"
cyan: &cyan "#7dcfff"
green: &green "#73daca"
yellow: &yellow "#e0af68"
orange: &orange "#ff9e64"
magenta: &magenta "#bb9af7"
pink: &pink "#f7768e"
blue: &blue "#7aa2f7"
red: &red "#f7768e"
white: &white "#c0caf5"

k9s:
  # general k9s styles
  body:
    fgColor: *foreground
    bgColor: *background
    logoColor: *orange
  # command prompt styles
  prompt:
    fgColor: *foreground
    bgColor: *background
    suggestColor: *orange
  # clusterinfoview styles.
  info:
    fgColor: *orange
    sectionColor: *foreground
  # dialog styles.
  dialog:
    fgColor: *foreground
    bgColor: *background
    buttonFgColor: *foreground
    buttonBgColor: *green
    buttonFocusFgColor: *background
    buttonFocusBgColor: *foreground
    labelFgColor: *comment
    fieldFgColor: *foreground
  frame:
    # borders styles.
    border:
      fgColor: *selection
      focusColor: *foreground
    menu:
      fgColor: *foreground
      keyColor: *blue
      # used for favorite namespaces
      numKeyColor: *blue
    # crumbview attributes for history navigation.
    crumbs:
      fgColor: *background
      bgColor: *cyan
      activeColor: *orange
    # resource status and update styles
    status:
      newColor: *blue
      modifyColor: *yellow
      addColor: *white
      errorColor: *red
      highlightColor: *orange
      killColor: *magenta
      completedColor: *comment
    # border title styles.
    title:
      fgColor: *foreground
      bgColor: *background
      highlightColor: *blue
      counterColor: *green
      filterColor: *magenta
  views:
    # charts skins...
    charts:
      bgColor: *background
      defaultDialColors:
        - *blue
        - *red
      defaultChartColors:
        - *blue
        - *red
    # tableview attributes.
    table:
      fgColor: *foreground
      bgColor: *background
      markColor: *pink
      # header row styles.
      header:
        fgColor: *foreground
        bgColor: *background
        sorterColor: *cyan
    # xray view attributes.
    xray:
      fgColor: *foreground
      bgColor: *background
      cursorColor: *current_line
      graphicColor: *blue
      showIcons: false
    # yaml info styles.
    yaml:
      keyColor: *green
      colonColor: *blue
      valueColor: *foreground
    # logs styles.
    logs:
      fgColor: *foreground
      bgColor: *background
      indicator:
        fgColor: *foreground
        bgColor: *selection
        toggleOnColor: *cyan
        toggleOffColor: *foreground
    help:
      fgColor: *foreground
      bgColor: *background
      indicator:
        fgColor: *red
        bgColor: *background
```
