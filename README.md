# Cinderline

A warm, dark theme for [Omarchy](https://omarchy.org/) built around charcoal-brown surfaces, parchment text, muted earth tones, and ember-orange accents.

> **Charcoal. Parchment. Ember.**

![Cinderline preview](preview.png)

## Installation

```bash
omarchy theme install https://github.com/tbenj1/omarchy-cinderline-theme.git
omarchy theme set cinderline
```

Or open the Omarchy menu and use **Install → Style → Theme**, then paste:

```text
https://github.com/tbenj1/omarchy-cinderline-theme.git
```

## Omarchy 4 / Quattro

Cinderline follows the modern Omarchy theme model while retaining familiar compatibility files found in established community themes.

- `colors.toml` is the canonical palette and includes both semantic Quattro roles and ANSI `color0`–`color15` aliases.
- `shell.toml` provides coordinated Cinderline colors for the Quattro shell.
- Omarchy regenerates protected terminal/editor files from `colors.toml` when the theme is installed from Git.
- App-specific files are also committed for local themes, legacy Omarchy integrations, and compatible theme-hook tooling.

### Display safety

Cinderline does **not** define monitors or display topology. Its `hyprland.conf` contains border colors only. There are no monitor, workspace, input, animation, bind, or executable rules in the theme.

That means your monitor arrangement remains the responsibility of your normal Omarchy/Hyprland monitor configuration, just as it is with other themes.

## Included surfaces

Cinderline includes theme data for:

- Omarchy Quattro shell
- Hyprland borders and legacy Hyprlock colors
- Alacritty, Foot, Ghostty, and Kitty
- btop and cava
- Chromium
- GTK color overrides
- Waybar, Walker, Mako, and SwayOSD legacy integrations
- Omarchy screen-share picker
- Obsidian
- Zed
- Zen-style color variables

Some of these files are retained for compatibility. Current Git-installed Omarchy deliberately drops executable/config-sensitive files such as terminal configs and regenerates them locally from `colors.toml`.

## Backgrounds

Five 4K wallpapers are included:

1. **Ember Horizon**
2. **Nebula Dust**
3. **Earth & Ink**
4. **Ink & Ochre**
5. **Ember Gradient**

Cycle them with:

```bash
omarchy theme bg next
```

## Palette

| Role | Hex |
|---|---|
| Background | `#0e0c0b` |
| Dark background | `#0d0b09` |
| Surface | `#1e1912` |
| Selection | `#402312` |
| Border | `#4a3424` |
| Accent / Ember | `#e97835` |
| Foreground | `#dfd0bb` |
| Bright foreground | `#f2e6d4` |
| Muted | `#6b5847` |
| Heading amber | `#efb85f` |
| Sage | `#87b978` |
| Steel blue | `#86a6b8` |

## Companion Fonts

The matching typography package is maintained separately:

**[tbenj1/omarchy-cinderline-fonts](https://github.com/tbenj1/omarchy-cinderline-fonts)**

It provides:

- **Lora** — editorial / serif
- **IBM Plex Sans** — proportional UI
- **IBM Plex Mono Nerd Font / BlexMono Nerd Font** — terminal, shell, and code

## Repository layout

```text
omarchy-cinderline-theme/
├── backgrounds/
├── gtk-3.0/
├── gtk-4.0/
├── zed/themes/
├── colors.toml
├── shell.toml
├── hyprland.conf
├── hyprlock.conf
├── alacritty.toml
├── foot.ini
├── ghostty.conf
├── kitty.conf
├── btop.theme
├── cava_theme
├── chromium.theme
├── gtk.css
├── hyprland-preview-share-picker.css
├── mako.ini
├── obsidian.css
├── swayosd.css
├── walker.css
├── waybar.css
├── zed.json
├── zen.css
├── icons.theme
├── preview.png
├── README.md
└── LICENSE
```

## Updating

```bash
omarchy theme update
```

## Removing

```bash
omarchy theme remove cinderline
```

## Cinderline

Dark surfaces form the cinder. Ember highlights define the line.

**Cinderline.**
