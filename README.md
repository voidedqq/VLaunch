<div align="center">

# VLaunch

### Modern launcher for Windows

<img src="VLaunch.png" width="900">

Fast. Lightweight. Keyboard-first.

Launch applications, access tools, and stay focused without digging through menus.

Built for people who prefer their keyboard over their mouse.

<br>

![Platform](https://img.shields.io/badge/platform-windows-blue?style=for-the-badge)
![Framework](https://img.shields.io/badge/framework-.NET%2010-purple?style=for-the-badge)
![UI](https://img.shields.io/badge/ui-wpf-darkgreen?style=for-the-badge)
![Status](https://img.shields.io/badge/status-beta-darkred?style=for-the-badge)

</div>

---

## Table of Contents

* [Introduction](#introduction)
* [Why VLaunch?](#why-vlaunch)
* [Features](#features)
* [Feature Status](#feature-status)
* [Installation](#installation)
* [Theming](#theming)
* [Built-in Themes](#built-in-themes)
* [Local Storage](#local-storage)
* [Roadmap](#roadmap)
* [Screenshots](#screenshots)
* [Thanks](#thanks)
* [Credits](#credits)
* [License](#license)

---

## Introduction

VLaunch is a modern Windows launcher built with C# and WPF.

Designed around speed and keyboard-first workflows, VLaunch allows you to instantly launch applications without navigating through desktop shortcuts, folders, or the Start Menu.

The project takes inspiration from Raycast, Spotlight, Flow Launcher, and PowerToys Run while maintaining a lightweight and highly customizable approach.

---

## Why VLaunch?

Most Windows launchers are either bloated, outdated, or overloaded with features most users never touch.

VLaunch focuses on the essentials:

* Fast application launching
* Clean modern interface
* Local-first configuration
* Lightweight resource usage
* Customizable themes
* No accounts
* No subscriptions
* No telemetry

---

## Features

* Fast application launching
* Keyboard-focused workflow
* Search history
* System tray integration
* Startup support
* Local configuration
* JSON-based theme system
* Custom hotkeys
* Lightweight design
* Modern glass-inspired interface

---

## Feature Status

| Feature               | Status |
| --------------------- | ------ |
| Application Launching | ✅      |
| Search History        | ✅      |
| System Tray           | ✅      |
| Theme System          | ✅      |
| Startup Support       | ✅      |
| Custom Hotkeys        | 🚧     |
| Settings Page         | 🚧     |
| File Search           | 📅     |
| Plugin System         | 📅     |
| Command Palette       | 📅     |

---

## Installation

1. Download the latest release from the Releases page.
2. Run `VLaunchSetup.exe`.
3. Complete the installation.
4. Launch VLaunch from the desktop or Start Menu.

### Requirements

* Windows 10 or Windows 11
* x64 processor

---

## Theming

VLaunch supports fully customizable JSON themes.

Theme files are stored in:

```txt
%AppData%\VLaunch\Themes
```

Every `.json` file inside this folder will automatically appear in the theme picker.

### Example Theme

```json
{
  "Name": "VLaunch",
  "Background": "#FF15151D",
  "SearchBackground": "#FF1E1E28",
  "Accent": "#8B5CF6",
  "Text": "#FFFFFF",
  "MutedText": "#9A9AA6",
  "Border": "#FF2B2B36",
  "CornerRadius": 24,
  "SearchRadius": 18,
  "Blur": true
}
```

### Theme Properties

| Property         | Description                                |
| ---------------- | ------------------------------------------ |
| Name             | Theme name displayed inside VLaunch        |
| Background       | Main launcher background                   |
| SearchBackground | Search bar background                      |
| Accent           | Accent color used throughout the interface |
| Text             | Primary text color                         |
| MutedText        | Secondary text color                       |
| Border           | Border color                               |
| CornerRadius     | Main launcher corner radius                |
| SearchRadius     | Search bar corner radius                   |
| Blur             | Enables blur effects when supported        |

---

### Understanding Colors

VLaunch uses hexadecimal color values.

Standard colors use:

```txt
#RRGGBB
```

Example:

```txt
#8B5CF6
```

Purple.

You can also use transparency:

```txt
#AARRGGBB
```

Where:

```txt
AA = transparency
RR = red
GG = green
BB = blue
```

Examples:

| Value | Transparency |
| ----- | ------------ |
| FF    | 100% visible |
| E6    | 90% visible  |
| CC    | 80% visible  |
| 99    | 60% visible  |
| 66    | 40% visible  |
| 33    | 20% visible  |
| 00    | Invisible    |

Example:

```txt
#FF15151D
```

Fully opaque dark background.

Example:

```txt
#9915151D
```

Semi-transparent dark background.

Example:

```txt
#3315151D
```

Very transparent dark background.

---

### Transparency Tips

For most themes, it is recommended to keep transparency relatively low.

Good:

```txt
#FF15151D
#E615151D
#CC15151D
```

Usually too transparent:

```txt
#9915151D
#6615151D
#3315151D
```

Excessive transparency can make text harder to read and may reduce visual consistency across different Windows setups.

---

### Corner Radius

Corner radius controls how rounded the launcher appears.

Examples:

```txt
8   = subtle rounding
16  = modern
24  = default VLaunch style
32+ = very rounded
```

---

### Blur

```json
"Blur": true
```

Enables blur effects when supported.

```json
"Blur": false
```

Disables blur effects.

---

After saving a theme file, open the theme picker and select it instantly without restarting VLaunch.


---

## Built-in Themes

Current bundled themes:

* Dark Glass
* Void Glass
* Midnight Neon
* AMOLED
* Catppuccin Mocha
* HyperX
* Nothing

More themes will be added in future releases.

---

## Local Storage

All launcher data is stored locally.

Location:

```txt
%AppData%\VLaunch
```

Structure:

```txt
VLaunch
├── config.json
├── history.json
└── Themes
    ├── DarkGlass.json
    ├── AMOLED.json
    ├── Nothing.json
    └── CustomTheme.json
```

No cloud services are used.

No user data is collected.

---

## Roadmap

### Planned

* Acrylic blur improvements
* Startup wizard
* Settings page
* Better application indexing
* File searching
* Command palette
* Plugin support
* Custom commands
* Additional theme customization
* More built-in themes
* Improved animations
* Theme marketplace

---

## Screenshots

### Main Window

<img src="VLaunch.png" width="900">

---

## Credits

Inspired by:

* Raycast
* Spotlight
* Flow Launcher
* PowerToys Run

---

## Thanks

Special thanks to:

* **@solaenum** — for calling it a virus
* **@jib123w** — for testing it
* **@goonoftheforce** — for testing it

ily

---

## Status

VLaunch is currently in beta and under active development.

Features, behavior, and configuration options may change between releases.

Feedback, bug reports, and suggestions are welcome.

---

## License

Copyright (c) 2026 voided

All Rights Reserved.

You may not:

* Redistribute
* Modify
* Resell
* Reupload
* Claim this project as your own

without explicit permission from the author.
