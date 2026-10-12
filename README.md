# 🌸 Seelen UI Anime Glassmorphism Widgets Suite for KDE Plasma

[![KDE Plasma](https://img.shields.io/badge/KDE_Plasma-5.27%20%7C%206.x-38bdf8?style=flat-square&logo=kde)](https://kde.org/plasma-desktop/)
[![Qt Version](https://img.shields.io/badge/QtQuick-2.15+-41cd52?style=flat-square&logo=qt)](https://www.qt.io/)
[![Widgets](https://img.shields.io/badge/Widgets-12%20Plasmoids-f472b6?style=flat-square)](#-widget-catalog)
[![License](https://img.shields.io/badge/License-MIT-a855f7?style=flat-square)](#-license)

A curated collection of **12 native KDE Plasma desktop widgets (`.plasmoid`)** designed with **Seelen UI acrylic glassmorphism**, neon cyberpunk telemetry, and a sleek **anime aesthetic**.

These applets run natively on KDE Plasma without third-party docks, electron containers, or background overhead.

---

## 📑 Table of Contents

- [🎨 Visual Design Philosophy](#-visual-design-philosophy)
- [🍱 Widget Catalog](#-widget-catalog)
  - [1. Seelen Clock (Chrono Dial)](#1-seelen-clock-chrono-dial)
  - [2. Seelen Music Player (Audio & Synced Lyrics)](#2-seelen-music-player-audio--synced-lyrics)
  - [3. Seelen System Monitor (Telemetry HUD)](#3-seelen-system-monitor-telemetry-hud)
  - [4. Seelen Weather (Atmospheric HUD)](#4-seelen-weather-atmospheric-hud)
  - [5. Seelen Quick Launcher (App Dock)](#5-seelen-quick-launcher-app-dock)
  - [6. Seelen Daily Quotes (Soul Quotes)](#6-seelen-daily-quotes-soul-quotes)
  - [7. Seelen Focus Timer (Pomodoro)](#7-seelen-focus-timer-pomodoro)
  - [8. Seelen Sticky Memo (Mission Log)](#8-seelen-sticky-memo-mission-log)
  - [9. Seelen Network Monitor (Telemetry)](#9-seelen-network-monitor-telemetry)
  - [10. Seelen Battery Core (Reactor)](#10-seelen-battery-core-reactor)
  - [11. Seelen Audio HUD (Master Matrix)](#11-seelen-audio-hud-master-matrix)
  - [12. Seelen Daily Quests (RPG EXP Tasks)](#12-seelen-daily-quests-rpg-exp-tasks)
- [🚀 Quick Installation](#-quick-installation)
  - [Option A: One-Liner Terminal Install (Recommended)](#option-a-one-liner-terminal-install-recommended)
  - [Option B: KDE Package Manager CLI (kpackagetool)](#option-b-kde-package-manager-cli-kpackagetool)
  - [Option C: Plasma Graphical Interface (GUI)](#option-c-plasma-graphical-interface-gui)
  - [Option D: Direct Drag-and-Drop](#option-d-direct-drag-and-drop)
- [🖥️ How to Add Widgets to Your Desktop](#️-how-to-add-widgets-to-your-desktop)
- [🛠️ Customization & Tweaks](#️-customization--tweaks)
- [⚙️ Requirements & Compatibility](#️-requirements--compatibility)
- [🗑️ Uninstallation](#️-uninstallation)
- [📄 License & Credits](#-license--credits)

---

## 🎨 Visual Design Philosophy

- **Frosted Acrylic Glassmorphism**: Translucent acrylic gradient surfaces (`#32ffffff` highlight down to subtle translucent obsidian tones) with rounded corners (`18px` radius).
- **Luminous Specular Highlight**: Top-edge specular sheen rim (`1.2px`, `#70ffffff`) simulating physical beveled glass.
- **Cyber-Neon Accent Palette**:
  - 🌸 **Sakura Pink** (`#f472b6`)
  - 🌐 **Cyber Cyan** (`#38bdf8`)
  - ⚡ **Electric Violet** (`#a855f7`)
  - 🌿 **Mint Green** (`#34d399`)
  - 🌅 **Sunset Amber** (`#fb923c`)
- **Fluid Micro-Animations**: Smooth opacity fades (`Easing.OutQuad`) and spring-like height transitions (`Easing.OutCubic`).
- **Zero Dock/Docker Overhead**: Pure QtQuick / QML declarative applets loaded directly by `plasmashell`.

---

## 🍱 Widget Catalog

| File | Applet ID | Category | Default Size | Highlight Features |
| :--- | :--- | :--- | :---: | :--- |
| `org.seelen.anime.clock.plasmoid` | `org.seelen.anime.clock` | Date and Time | 260 × 290 | Analogue watch face, UTC telemetry pill, date complication, dead-beat seconds |
| `org.seelen.anime.music.plasmoid` | `org.seelen.anime.music` | Multimedia | 360 × 480 | MPRIS2 playback controls, real-time synchronized LRCLIB lyrics, seek-on-click |
| `org.seelen.anime.system.plasmoid` | `org.seelen.anime.system` | System Information | 300 × 190 | CPU & RAM live utilization gauges, sync rating telemetry |
| `org.seelen.anime.weather.plasmoid` | `org.seelen.anime.weather` | Environment & Weather | 300 × 180 | Live IP geolocation, real-time temperature with °C/°F toggle, condition emoji, humidity, wind, and AQI |
| `org.seelen.anime.launcher.plasmoid` | `org.seelen.anime.launcher` | Application Launchers | 320 × 110 | Desktop cyber dock with quick triggers for Terminal, Browser, Code, Discord, Spotify |
| `org.seelen.anime.quotes.plasmoid` | `org.seelen.anime.quotes` | Utilities | 320 × 160 | Inspiring anime quotes with interactive click-to-cycle, character & series attribution |
| `org.seelen.anime.pomodoro.plasmoid` | `org.seelen.anime.pomodoro` | Utilities | 260 × 240 | 25-minute Pomodoro focus countdown, session completed counter, Play/Pause/Reset |
| `org.seelen.anime.notes.plasmoid` | `org.seelen.anime.notes` | Utilities | 280 × 200 | Translucent mission memo checklist with quick buffer reset |
| `org.seelen.anime.network.plasmoid` | `org.seelen.anime.network` | System Information | 280 × 160 | Real-time live ping latency (ms) and bandwidth RX / TX telemetry |
| `org.seelen.anime.battery.plasmoid` | `org.seelen.anime.battery` | System Information | 280 × 160 | Sci-Fi reactor core gauge, charge status, interactive power profile switch (Balanced/Eco/Performance) |
| `org.seelen.anime.volume.plasmoid` | `org.seelen.anime.volume` | Multimedia | 280 × 170 | Master volume slider, instant mute toggle, 0% / 25% / 50% / 75% / 100% quick presets |
| `org.seelen.anime.quests.plasmoid` | `org.seelen.anime.quests` | Utilities | 310 × 210 | RPG quest checklist (Solo Leveling style) with interactive task completion, EXP bar & Level Up |

---

### Detailed Widget Breakdown

#### 1. Seelen Clock (Chrono Dial)
- **ID**: `org.seelen.anime.clock`
- **File**: `org.seelen.anime.clock.plasmoid`
- **Visuals**: Classical precision dial enclosed in beveled frosted glass. Features an outer bezel ring with 60 minute ticks, inner chapter track, faceted sword hands for hours and minutes, and a dead-beat second hand.
- **Complications**: Live date pill (Day & Month), flashing heartbeat indicator, and top UTC digital telemetry tag (`UTC HH:MM`).

#### 2. Seelen Music Player (Audio & Synced Lyrics)
- **ID**: `org.seelen.anime.music`
- **File**: `org.seelen.anime.music.plasmoid`
- **Audio Control**: Full MPRIS2 integration (compatible with Spotify, VLC, MPV, Firefox, Brave, Chrome).
- **Synced Lyrics Display**: Fetches time-stamped synced lyrics via LRCLIB. Displays active lines with glowing focus, fading inactive lyrics, and automatically scrolling the active lyric to the viewport center.
- **Interactive Seek**: Clicking on any lyric row instantly seeks the media player to that precise timestamp!
- **Auto Collapse**: Expands smoothly when music is playing and minimizes/hides when playback ceases.

#### 3. Seelen System Monitor (Telemetry HUD)
- **ID**: `org.seelen.anime.system`
- **File**: `org.seelen.anime.system.plasmoid`
- **Telemetry**: Monitored CPU load %, RAM consumed vs. total (`9.3 / 16.0 GB`), and an EVA-style `SYNC RATE: 99.4%` status metric.
- **Gauges**: Gradient neon progress bars with dynamic color shifts.

#### 4. Seelen Weather (Atmospheric HUD)
- **ID**: `org.seelen.anime.weather`
- **File**: `org.seelen.anime.weather.plasmoid`
- **Live IP Geolocation**: Automatically determines the user's city and geographical coordinates via IP address (`wttr.in` & `GeoJS` fallback).
- **Real-Time Atmospheric Telemetry**: Live temperature, weather condition description, dynamic day/night weather emoji, humidity %, wind speed (km/h), and live Air Quality Index (`AQI` via Open-Meteo).
- **Interactive Controls**:
  - Click the **`WEATHER`** tag pill to trigger an immediate manual telemetry sync (with animated syncing indicator).
  - Click anywhere on the card to toggle between Celsius (°C) and Fahrenheit (°F).
  - Automatically refreshes every 15 minutes in the background.

#### 5. Seelen Quick Launcher (App Dock)
- **ID**: `org.seelen.anime.launcher`
- **File**: `org.seelen.anime.launcher.plasmoid`
- **Cyber Dock**: Glass-framed dock icons for rapid workflow launching:
  - 💻 `Terminal`
  - 🌐 `Browser`
  - ⚡ `Code`
  - 💬 `Discord`
  - 🎵 `Music`
  - 📂 `Files`

#### 6. Seelen Daily Quotes (Soul Quotes)
- **ID**: `org.seelen.anime.quotes`
- **File**: `org.seelen.anime.quotes.plasmoid`
- **Curated Wisdom**: Inspiring quotes from iconic anime (Kamina / *Gurren Lagann*, Okabe Rintaro / *Steins;Gate*, Luffy & Brook / *One Piece*, Kenshin / *Rurouni Kenshin*).
- **Interactive**: Click the quote card anytime to cycle to the next quote with an animated fade.

#### 7. Seelen Focus Timer (Pomodoro)
- **ID**: `org.seelen.anime.pomodoro`
- **File**: `org.seelen.anime.pomodoro.plasmoid`
- **Functionality**: 25:00 focus timer engineered for deep work sessions.
- **Controls**: Interactive START / PAUSE toggle button, RESET action, and a completed study sessions badge counter (`★ SESSIONS: X`).

#### 8. Seelen Sticky Memo (Mission Log)
- **ID**: `org.seelen.anime.notes`
- **File**: `org.seelen.anime.notes.plasmoid`
- **Aesthetic**: Cyberpunk translucent sticky note.
- **Features**: Active objective checklist, mission log headers, and quick-clear buffer capability.

#### 9. Seelen Network Monitor (Telemetry)
- **ID**: `org.seelen.anime.network`
- **File**: `org.seelen.anime.network.plasmoid`
- **Network Telemetry**: Live ping latency gauge (`18 ms`), real-time download bandwidth rate (MB/s), and upload rate (MB/s).

#### 10. Seelen Battery Core (Reactor)
- **ID**: `org.seelen.anime.battery`
- **File**: `org.seelen.anime.battery.plasmoid`
- **Reactor Core**: S² Engine aesthetic battery monitor with high-visibility charge percentage and glowing active charging indicator.
- **Mode Toggle**: Click the mode pill to toggle power profiles: `BALANCED` ➔ `PERFORMANCE` ➔ `ECO`.

#### 11. Seelen Audio HUD (Master Matrix)
- **ID**: `org.seelen.anime.volume`
- **File**: `org.seelen.anime.volume.plasmoid`
- **Interactive Slider**: Click or drag along the neon volume bar to adjust system audio level.
- **Mute Toggle**: Click the audio badge or mute icon to instantly toggle master audio mute.
- **Quick Preset Pills**: One-click jumps to preset levels: `0%`, `25%`, `50%`, `75%`, `100%`.

#### 12. Seelen Daily Quests (RPG EXP Tasks)
- **ID**: `org.seelen.anime.quests`
- **File**: `org.seelen.anime.quests.plasmoid`
- **Solo Leveling RPG HUD**: Gamify your daily routine!
- **Features**: Interactive checkboxes for daily quests. Checking an objective awards EXP, fills the glowing EXP progression bar, and triggers Level Up celebrations.

---

## 🚀 Quick Installation

Choose any of the following installation methods:

### Option A: One-Liner Terminal Install (Recommended)

Since `.plasmoid` packages are zip archives, you can extract and install all 12 widgets into your user's Plasma widgets folder in one command:

```bash
# Navigate to this folder
cd ~/Desktop/Seelen-Anime-Widgets

# Extract all 12 plasmoids to ~/.local/share/plasma/plasmoids/
mkdir -p ~/.local/share/plasma/plasmoids
python3 -c "
import glob, zipfile, os
dest = os.path.expanduser('~/.local/share/plasma/plasmoids')
for p in glob.glob('*.plasmoid'):
    widget_id = p.replace('.plasmoid', '')
    target = os.path.join(dest, widget_id)
    os.makedirs(target, exist_ok=True)
    with zipfile.ZipFile(p, 'r') as z:
        z.extractall(target)
    print(f'✓ Installed: {widget_id}')
"

# Refresh KDE system cache
kbuildsycoca6 --noincremental 2>/dev/null || kbuildsycoca5 --noincremental 2>/dev/null
```

> **Tip:** If the widgets don't appear in the menu immediately, reload `plasmashell`:
> ```bash
> systemctl --user restart plasma-plasmashell 2>/dev/null || (killall plasmashell && nohup plasmashell >/dev/null 2>&1 &)
> ```

---

### Option B: KDE Package Manager CLI (`kpackagetool`)

You can install individual widgets using KDE's native package tool:

**For KDE Plasma 6:**
```bash
cd ~/Desktop/Seelen-Anime-Widgets
for widget in *.plasmoid; do
    kpackagetool6 -t Plasma/Applet -i "$widget" || kpackagetool6 -t Plasma/Applet -u "$widget"
done
```

**For KDE Plasma 5:**
```bash
cd ~/Desktop/Seelen-Anime-Widgets
for widget in *.plasmoid; do
    kpackagetool5 -t Plasma/Applet -i "$widget" || kpackagetool5 -t Plasma/Applet -u "$widget"
done
```

---

### Option C: Plasma Graphical Interface (GUI)

1. Right-click on your desktop wallpaper and choose **"Add Widgets..."** (or **"Enter Edit Mode"** ➔ **"Add Widgets..."**).
2. Click **"Get New Widgets"** at the bottom of the widget sidebar.
3. Select **"Install from Local File..."**.
4. Browse to `~/Desktop/Seelen-Anime-Widgets/` and select any `.plasmoid` file to install.

---

### Option D: Direct Drag-and-Drop

In KDE Plasma, you can directly **drag and drop** any `.plasmoid` file from your file manager (Dolphin or Desktop) onto your desktop workspace or panel to add it immediately.

---

## 🖥️ How to Add Widgets to Your Desktop

Once installed:
1. Right-click any empty space on your desktop wallpaper.
2. Select **"Add Widgets..."** from the context menu.
3. In the widget search bar, type `Seelen`.
4. All 12 widgets will appear with their custom icons and descriptions:
   - *Seelen Clock*
   - *Seelen Music Player*
   - *Seelen System Monitor*
   - *Seelen Weather*
   - *Seelen Quick Launcher*
   - *Seelen Daily Quotes*
   - *Seelen Focus Timer*
   - *Seelen Sticky Memo*
   - *Seelen Network Monitor*
   - *Seelen Battery Core*
   - *Seelen Audio HUD*
   - *Seelen Daily Quests*
5. Drag and drop your favorite widgets onto your desktop or panels and arrange them to fit your setup!

---

## 🛠️ Customization & Tweaks

Each widget is packaged as a `.plasmoid` zip file containing:
```text
org.seelen.anime.<name>.plasmoid
├── metadata.desktop
├── metadata.json
└── contents/
    └── ui/
        └── main.qml
```

To modify colors, default values, fonts, or dimensions:
1. **Unpack the widget**:
   ```bash
   mkdir -p custom_widget
   python3 -c "import zipfile; zipfile.ZipFile('org.seelen.anime.music.plasmoid').extractall('custom_widget')"
   ```
2. **Edit `custom_widget/contents/ui/main.qml`** with any text editor.
3. **Repack into `.plasmoid`**:
   ```bash
   cd custom_widget
   python3 -c "
   import zipfile, os
   with zipfile.ZipFile('../org.seelen.anime.music.plasmoid', 'w', zipfile.ZIP_DEFLATED) as z:
       for root, dirs, files in os.walk('.'):
           for file in files:
               p = os.path.join(root, file)
               z.write(p, os.path.relpath(p, '.'))
   "
   cd .. && rm -rf custom_widget
   ```
4. Reinstall the widget using [Option A](#option-a-one-liner-terminal-install-recommended) or [Option B](#option-b-kde-package-manager-cli-kpackagetool).

---

## ⚙️ Requirements & Compatibility

- **Desktop Environment**: KDE Plasma 5.24+ or KDE Plasma 6.x
- **Frameworks & Libraries**:
  - `QtQuick 2.15+`
  - `QtQuick.Controls 2.15+`
  - `QtQuick.Layouts 1.15+`
  - `org.kde.plasma.plasmoid 2.0`
  - `org.kde.plasma.core 2.0`
- **Media Player (for Seelen Music Player)**:
  - Any MPRIS2-compliant player (Spotify, VLC, MPV, Firefox, Chrome, Brave, Strawberry, Clementine, etc.)
  - Internet connection for fetching synced lyrics from LRCLIB.

---

## 🗑️ Uninstallation

To remove all Seelen Anime widgets from your system:

```bash
# Remove installed widgets directory
rm -rf ~/.local/share/plasma/plasmoids/org.seelen.anime.*

# Refresh KDE Plasma cache
kbuildsycoca6 --noincremental 2>/dev/null || kbuildsycoca5 --noincremental 2>/dev/null

# Optional: Restart plasmashell to update widget explorer
systemctl --user restart plasma-plasmashell 2>/dev/null || true
```

---

## 📄 License & Credits

- **Author**: dexorto ([github.com/dexorto](https://github.com/dexorto))
- **Design Inspiration**: [Seelen UI](https://github.com/eythaann/Seelen-UI), Cyberpunk HUD aesthetics, Evangelion telemetry, and modern frosted glass UI.
- **License**: MIT License. Free to use, modify, and distribute.
