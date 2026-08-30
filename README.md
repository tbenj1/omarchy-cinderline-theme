# Cinderline

A warm, dark theme for [Omarchy](https://omarchy.org/) built around deep charcoal-brown surfaces, parchment text, muted earth tones, and ember-orange accents.

Cinderline is designed to feel technical without feeling sterile: dark enough for long sessions, warm enough to avoid the usual blue-black developer aesthetic, and restrained enough that warnings, errors, selections, and active elements remain meaningful.

> **Charcoal. Parchment. Ember.**

---

## Preview

<!-- Add your preview image to the repository and uncomment this line. -->

<!-- ![Cinderline for Omarchy](preview.png) -->

Cinderline uses a near-black brown foundation with progressively warmer surfaces and an ember-orange accent.

The result is a desktop aesthetic inspired by technical notebooks, old terminals, burnt paper, warm metals, and low-light workspaces rather than neon cyberpunk styling.

---

## Installation

### Install from GitHub

Install Cinderline directly through Omarchy:

```bash
omarchy theme install https://github.com/tbenj1/omarchy-cinderline-theme.git
```

Then activate it:

```bash
omarchy theme set cinderline
```

Once installed, Cinderline will also appear in Omarchy's theme selector.

### Install through the Omarchy menu

Open the Omarchy menu and navigate to:

```text
Install
└── Style
    └── Theme
```

Enter the repository URL:

```text
https://github.com/tbenj1/omarchy-cinderline-theme.git
```

After installation, select **Cinderline** under:

```text
Style
└── Theme
```

### Local development

To test or modify Cinderline locally:

```bash
mkdir -p ~/.config/omarchy/themes/cinderline
```

Copy the theme files into:

```text
~/.config/omarchy/themes/cinderline/
```

Then activate it:

```bash
omarchy theme set cinderline
```

---

# Palette

Cinderline is built around a warm technical palette derived from the visual system originally developed for the **Root Cause Handbook**.

## Core Colors

| Role               | Color            | Hex       |
| ------------------ | ---------------- | --------- |
| Background         | Near-black brown | `#0e0c0b` |
| Dark Background    | Charcoal black   | `#0d0b09` |
| Deepest Background | Near black       | `#080706` |
| Surface            | Warm charcoal    | `#1e1912` |
| Selection          | Burnt brown      | `#402312` |
| Accent             | Ember orange     | `#e97835` |
| Foreground         | Warm parchment   | `#dfd0bb` |
| Light Foreground   | Pale parchment   | `#e4d8c6` |
| Bright Foreground  | Ivory parchment  | `#f2e6d4` |
| Muted              | Earth brown      | `#6b5847` |

## Semantic Colors

| Role    |    Normal |    Bright |
| ------- | --------: | --------: |
| Red     | `#d87363` | `#ef8d79` |
| Yellow  | `#f1c76a` | `#f6d890` |
| Orange  | `#e97835` |         — |
| Green   | `#87b978` | `#a1ca91` |
| Cyan    | `#8fb5aa` | `#abd0c6` |
| Blue    | `#86a6b8` | `#a3bdcb` |
| Magenta | `#b9899a` | `#d0a3b0` |
| Brown   | `#6b3a1d` |         — |

### Additional Design Accents

The broader Cinderline visual language also uses:

| Purpose                           |       Hex |
| --------------------------------- | --------: |
| Navigation / alternate background | `#150f0a` |
| Warm inset surface                | `#1e140c` |
| Border                            | `#4a3424` |
| Primary heading                   | `#f6cf98` |
| Secondary heading                 | `#efb85f` |
| Link / amber accent               | `#f2b667` |
| Success / tip                     | `#87b978` |
| Warning                           | `#f1c76a` |
| Ember                             | `#e97835` |

---

## `colors.toml`

Cinderline uses Omarchy's semantic theme system as the source of truth:

```toml
mode = "dark"

accent = "#e97835"
selection = "#402312"
muted = "#6b5847"

background = "#0e0c0b"
dark_background = "#0d0b09"
darker_background = "#080706"
lighter_background = "#1e1912"

dark_foreground = "#8c7b67"
foreground = "#dfd0bb"
light_foreground = "#e4d8c6"
bright_foreground = "#f2e6d4"

red = "#d87363"
yellow = "#f1c76a"
orange = "#e97835"
green = "#87b978"
cyan = "#8fb5aa"
blue = "#86a6b8"
magenta = "#b9899a"
brown = "#6b3a1d"

bright_red = "#ef8d79"
bright_yellow = "#f6d890"
bright_green = "#a1ca91"
bright_cyan = "#abd0c6"
bright_blue = "#a3bdcb"
bright_magenta = "#d0a3b0"
```

Omarchy uses this palette to generate compatible styling for supported components and applications.

---

# Typography

Cinderline has an optional companion font package that reproduces the typography originally paired with this color system.

The font package is maintained separately so the theme itself remains lightweight and focused entirely on visual theming.

## Cinderline Fonts

**Repository:**
[github.com/tbenj1/omarchy-cinderline-fonts](https://github.com/tbenj1/omarchy-cinderline-fonts)

The recommended Cinderline typography stack is:

| Purpose                 | Typeface                                         |
| ----------------------- | ------------------------------------------------ |
| Editorial / headings    | **Lora**                                         |
| UI / proportional text  | **IBM Plex Sans**                                |
| Terminal / shell / code | **IBM Plex Mono Nerd Font / BlexMono Nerd Font** |

The combination gives Cinderline two complementary personalities.

**Lora** provides the warm, editorial character.

**IBM Plex Sans** keeps interfaces clean and technical.

**IBM Plex Mono** carries the same design language into terminals, code, Waybar, and the Omarchy shell.

### Installing the Companion Fonts

Clone the font repository:

```bash
git clone https://github.com/tbenj1/omarchy-cinderline-fonts.git
cd omarchy-cinderline-fonts
```

Then run:

```bash
./install.sh
```

See the font repository for package information, Fontconfig configuration, verification, and removal instructions.

> The font package is optional. Cinderline does not require it to function.

---

# Design Philosophy

Cinderline intentionally avoids the saturated blues and purples common to many dark development themes.

Its visual hierarchy is built around four concepts.

### Charcoal

The desktop begins with a very dark brown-black rather than pure black.

```text
#0e0c0b
```

This keeps the environment dark while giving surfaces a subtle warmth.

### Parchment

Primary text avoids stark white.

```text
#f2e6d4
```

Warm off-white text maintains high contrast without making the interface feel clinical.

### Ember

The primary accent is a restrained burnt orange.

```text
#e97835
```

It identifies active elements and important interface states without dominating the desktop.

### Earth

Secondary colors remain deliberately desaturated.

Greens resemble sage, blues lean toward steel, cyan toward oxidized metal, and reds toward terracotta.

The terminal palette therefore remains functional without breaking the overall visual language.

---

# Repository Structure

The Cinderline theme repository is intentionally minimal:

```text
omarchy-cinderline-theme/
├── backgrounds/
│   ├── ...
│   └── README.md
├── colors.toml
├── icons.theme
├── preview.png
├── README.md
├── LICENSE
└── .gitignore
```

The companion typography project lives separately:

```text
omarchy-cinderline-fonts/
├── fontconfig/
├── install.sh
├── uninstall.sh
├── verify.sh
├── README.md
├── LICENSE
└── NOTICE.md
```

Keeping the projects separate allows Cinderline's visual theme to be installed independently from system-wide typography changes.

---

# Updating

Git-installed Omarchy themes can be updated through Omarchy:

```bash
omarchy theme update
```

After an update, reactivate Cinderline if necessary:

```bash
omarchy theme set cinderline
```

---

# Removing Cinderline

Remove the theme with:

```bash
omarchy theme remove cinderline
```

The optional Cinderline font package is managed separately. See the [`omarchy-cinderline-fonts`](https://github.com/tbenj1/omarchy-cinderline-fonts) repository for its uninstall procedure.

---

# Customization

Cinderline is intentionally straightforward to modify.

The central palette lives in:

```text
colors.toml
```

For example, the main accent:

```toml
accent = "#e97835"
```

can be changed while leaving the rest of the palette untouched.

Likewise, changing:

```toml
background = "#0e0c0b"
```

allows the overall darkness of the theme to be adjusted without rebuilding individual application configurations.

This is one of the primary reasons Cinderline uses Omarchy's semantic palette instead of maintaining independent color definitions for every application.

---

# Related Project

## Cinderline Fonts

The matching typography package is maintained independently:

**[`omarchy-cinderline-fonts`](https://github.com/tbenj1/omarchy-cinderline-fonts)**

```text
https://github.com/tbenj1/omarchy-cinderline-fonts
```

It provides the complete Cinderline typography stack using **Lora**, **IBM Plex Sans**, and **IBM Plex Mono Nerd Font** while leaving this repository dedicated solely to the Omarchy visual theme.

---

## About the Name

**Cinderline** combines the visual character of burnt charcoal and glowing embers with the precise, structured lines of a technical workspace.

Dark surfaces form the cinder.

Ember highlights define the line.

**Cinderline.**