<h1 align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="assets/logo-dark.svg">
    <img src="assets/logo-light.svg" alt="" width="64" align="middle">
  </picture>
  Starshot Launcher - Android gaming frontend
</h1>

<p align="center">
  Starshot Launcher - a comfortable and familiar emulation and gaming frontend for Android.
</p>

<p align="center">
  <a href="#features">Features</a> •
  <a href="#installation">Installation</a> •
  <a href="#architecture">Architecture</a> •
  <a href="#contributing">Contributing</a>
</p>

---

## Overview & Features

Starshot is an Android emulation frontend designed to provide a console-like, Material Design adjacent, utilitarian experience for managing and launching your game collection. Insightful choices with a focus on usability, reliability and quick setup make it ideal for those who want their experience streamlined without sacrificing functionality. Named after the [Breakthrough Starshot](https://en.wikipedia.org/wiki/Breakthrough_Starshot) initiative that has long inspired me and what I believe possible for humanity, Starshot will get you where you want to go at light speed.

### 🎮 Console-Style Experience
- **Tile-based home screen** grid, border style and many more personalizations, widgets, and shortcuts
- **Game library shelves** for quick access to your custom and generated collections
- **System categories** organized by platform (NES, SNES, PS1, PS2, etc.)
- **Controller-first UX** with full D-pad/analog navigation

### 📚 Unified Game Library
- **Auto-scan ROM directories** with hash-based identification
- **Multiple metadata providers** (IGDB, SteamGridDB, ScreenScraper) for rich game info & style
- **Grid, list and carousel views** with customizable display options
- **Advanced organization** by system, favorites, recently played and more

### 🕹️ Emulator Flexibility
- **No embedded emulators** - works with your existing emulator apps as you'd expect
- **Auto-detect installed emulators** on your device
- **Per-system & per-game emulator mapping** with sensible defaults, including emulator and RetroArch Core overrides for special configurations

### 🏆 RetroAchievements Integration
- **Native RetroAchievements support** with login persistence
- **Per-game achievement tracking** and progress display (with dual-screen support)
- **Hardcore mode support** for organized achievement hunting

### 🕹️ RomM Integration
- **RomM server support** allows you to fetch games from the RomM instance on your PC or server
- **In-app RomM browser** to explore and download from your collection, showing you (or, configurably, hiding) what you already have installed to your device
- **Full directories support** so you can find exactly what you are looking for in your instance
- **Collections support** to easily access your curated lists of games

### 📱 Adaptive Design
- **Phones** - Optimized portrait and landscape layouts
- **Tablets** - Expanded grid and views
- **Gaming handhelds** - Controller-optimized interface
- **Dual-screen devices** - Optional split mode for devices like the [AYN Thor](https://www.ayntec.com/products/ayn-thor) and [AYANEO Pocket DS](https://www.ayaneo.com/product/AYANEO-Pocket-DS)

### 🎨 Theming & Customization
- **Theme engine** with colors, styles and proportions
- **Configurable sound effects** for navigation and actions
- **Customizable wallpapers** for user personalization
- **Dynamic color theme support** based on wallpapers with overrides

### 📁 Media & Extras
- **Video, screenshots and manuals viewer** organized by game and system
- **Music player** for game soundtracks
- **News feed** with RSS support for gaming news - *Planned*

## Requirements

- **Android 11+** (API level 30)
- **Emulator apps** installed for your game systems
- **ROM files** dumped from your legally owned games

## Installation

### From Releases
1. Download the latest APK from [Releases](https://github.com/Jacob-Noah/Starshot/releases)
2. Install on your Android device
3. Configure your ROM directory (or specific system mappings if you don't use an ES-DE standard directory structure) in Settings
4. Configure your scrapers in Settings
5. Run a scan, run a scrape and enjoy your games!

## Architecture

Starshot is built with a modern Android architecture, leveraging Kotlin and Jetpack Compose for a responsive UI. The app follows the MVVM pattern, with repositories abstracting data sources and Hilt managing dependencies. The database layer uses Room for local storage of game metadata, while Ktor handles network requests to scrapers and APIs. Coil is used for efficient image loading and caching and Compose Navigation manages in-app navigation.

## Contributing

We are looking for testers to help improve Starshot. It is in active development and in use every day to keep making it better. If you want to help out, you can make an issue here on GitHub or join the Starshot Launcher [Discord server](https://discord.gg/nhHSGfVAzk) to discuss the app, suggest features, or report bugs.

When making an issue, please provide as much detail as possible, including steps to reproduce, screenshots and device information if relevant. There is an issue template to help guide you through the process.

## Roadmap

We maintain a to-do list of features and improvements. It is currently private to the tester team, but we anticipate changes to our triage as we enter public beta. Release information will be posted in the Starshot Launcher [Discord server](https://discord.gg/nhHSGfVAzk).

## Acknowledgments
- [RetroAchievements](https://retroachievements.org/) for the achievements API
- [RomM](https://romm.app/) for the API in their ROM management server
- [IGDB](https://www.igdb.com/) for game artwork and metadata
- [SteamGridDB](https://www.steamgriddb.com/) for game artwork
- [ScreenScraper](https://www.screenscraper.fr/) for game artwork and metadata
- The [Android](https://developer.android.com) and [Kotlin](https://developer.android.com/kotlin) communities for their excellent documentation and libraries
- [ES-DE](https://es-de.org/) for the structure of their ROM directories and metadata management
- [volekdesigns](https://volekdesigns.com/) for the amazing Starshot logo design

---

<p align="center">
  Made with ❤️ and impatience in receiving my AYN Thor, for retro gaming enthusiasts & the dual-screen handheld community
</p>
