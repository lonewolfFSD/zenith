# Zenith

> **A sleek, modern Top Notch & Dynamic Control Centre for Windows.**

Zenith transforms the top edge of your screen into a fluid, responsive Dynamic Island and pull-down Control Centre for Windows 10 & 11. Inspired by macOS Top Notch and iOS Dynamic Island, Zenith unifies media playback, system controls, clipboard history, app launching, and real-time hardware metrics into a single lightweight utility.

---

## ✨ Features

### 🏝️ Compact Dynamic Island (Collapsed View)
When idle or collapsed, Zenith rests as an unobtrusive, floating pill anchored to the top of your display:
- **Live Clock & Date**: Clean digital clock with click-to-lock mode (locks island to prevent accidental expansion).
- **Live Weather**: Current temperature and weather condition icon.
- **Battery & Power Gauge**: Real-time percentage indicator and charging bolt indicator.
- **Now Playing Media**: Displays album art, track details, and animated audio equalizer waves whenever music or video is playing on Windows (Spotify, YouTube Music, Apple Music, Tidal, browsers).
- **Synced Live Lyrics**: Real-time karaoke-style lyric sync across active music streams.
- **Track Change Toasts**: Smooth popup pill announcing track name and artist when songs change.
- **Interactive Quick Reply Drawer**: Instant quick replies and notifications for supported apps.

---

### 🎛️ Top Notch Control Centre (Expanded View)
Hovering near the top edge, pressing `Alt+Q`, or clicking the tray icon pulls down the full Control Centre:

| Tab | Capability |
| :--- | :--- |
| **Today** | Daily overview, weather forecast, calendar glance, and quick reminders. |
| **Controls** | System volume slider, output audio device selection, display brightness slider, microphone mute toggle, dark mode toggle, and focus/timer mode. |
| **Studio (Media)** | Full media playback hub with scrubber, play/pause/skip buttons, album artwork, and volume control. |
| **Apps** | Fast application launcher with instant fuzzy search across all installed Windows programs. |
| **Games** | Game shelf with library scanning and 1-click launching for Steam and PC games. |
| **Wallpapers** | Instant desktop wallpaper selector and switcher. |
| **Clipboard** | Real-time clipboard history manager with quick search, preview, and 1-click paste/restore. |
| **System Stats** | Live hardware monitoring for CPU load, RAM utilization, GPU status, and battery health. |

---

### 🎨 Themes & Customization
Zenith features built-in theme presets:
- **Dynamic Blue** (Default)
- **Cream**
- **Jungle**
- **Sakura**
- **Cyber**
- **Sunset**
- **Arctic**
- **Crimson**

---

## ⌨️ Shortcuts & Navigation

| Shortcut / Action | Action |
| :--- | :--- |
| `Alt + Q` | Toggle Zenith Notch / Control Centre |
| `Esc` | Collapse Control Centre back to Compact Island |
| `Hover Top Center` | Expand Control Centre (when Lock Mode is OFF) |
| `Click Clock on Island` | Toggle **Lock Mode** (prevents hover expansion during fullscreen work/gaming) |
| `System Tray Click` | Quick toggle Zenith |

---

## 🚀 Getting Started

### Prerequisites
- Windows 10 (Build 19041+) or Windows 11
- [Node.js](https://nodejs.org/) (v18 or higher recommended)
- `npm`

### Installation

1. Clone or extract the repository:
   ```bash
   cd "E:\Dylamic Island"
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Launch in development mode:
   ```bash
   npm run dev
   ```

---

## 📦 Building & Packaging

To build a standalone Windows installer or unpacked directory:

```bash
# Package into executable directory
npm run pack

# Build Windows NSIS installer
npm run dist
```

---

## 🛠️ Architecture

- **Runtime**: Electron 44+ / Node.js
- **Frontend**: Clean Vanilla JavaScript, CSS3 animations, HTML5 Web Audio & WebGL
- **OS Integration**:
  - Windows Media Session Manager bridge (PowerShell native integration) for media playback, track metadata, and album art.
  - Windows Audio Core API bridge for volume and default device switching.
  - Native Win32 display brightness, accessibility automation, and clipboard listeners.

---

## 📄 License

This project is licensed under the terms described in the `LICENSE` file.
