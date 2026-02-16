# Starshot Launcher - Android gaming frontend

<!-- <p align="center">
  <img src="docs/images/logo.png" alt="Starshot Logo" width="200"/>
</p> -->

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

I would say something really inspirational here about my vision for this app or why I made it, but the reality is, waiting months for your [AYN Thor](https://www.ayntec.com/products/ayn-thor) to arrive is a pain in the butt and I needed to do SOMETHING. I hope you enjoy.

### 🎮 Console-Style Experience
- **Tile-based home screen** with grid and border style personalizations
- **Recently played carousel** for quick access to your games
- **System categories** organized by platform (NES, SNES, PS1, PS2, etc.)
- **Controller-first UX** with full D-pad/analog navigation

### 📚 Unified Game Library
- **Auto-scan ROM directories** with hash-based identification
- **Multiple metadata providers** (IGDB, SteamGridDB, ScreenScraper) for rich game info & style
- **Grid, list and carousel views** with customizable display options
- **Advanced organization** by system, favorites and recently played

### 🕹️ Emulator Flexibility
- **No embedded emulators** - works with your existing emulator apps
- **Auto-detect installed emulators** on your device
- **Per-system emulator mapping** with sensible defaults
- **Per-game override support** for special configurations

### 🏆 RetroAchievements Integration
- **Native RetroAchievements support** with login persistence
- **Achievement popups** with custom sounds
- **Per-game achievement tracking** and progress display (with dual-screen support)
- **Hardcore mode support**

### 🕹️ RomM Integration
- **RomM server support** allows you to fetch games from the RomM instance on your PC or server
- **In-app RomM browser** to explore and download your collection
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
- **Dynamic color theme support** based on game artwork - *Coming soon*

### 📁 Media & Extras
- **Video, screenshots and manuals viewer** organized by game and system
- **Music player** for game soundtracks - *Coming soon*
- **News feed** with RSS support for gaming news - *Coming soon*

## Requirements

- **Android 13+** (API level 33)
- **Emulator apps** installed for your game systems
- **ROM files** dumped from your legally owned games

## Installation

### From Releases
1. Download the latest APK from [Releases](https://github.com/Jacob-Noah/Starshot/releases)
2. Install on your Android device
3. Configure your ROM directory (or specific system mappings you don't use ES-DE standard directories) in Settings
4. Configure your scrapers in Settings
5. Run a scan, run a scrape and enjoy your games!

## Architecture

Starshot is built with a modern Android architecture, leveraging Kotlin and Jetpack Compose for a responsive UI. The app follows the MVVM pattern, with repositories abstracting data sources and Hilt managing dependencies. The database layer uses Room for local storage of game metadata, while Ktor handles network requests to scrapers and APIs. Coil is used for efficient image loading and caching and Compose Navigation manages in-app navigation.

## Contributing

I am looking for testers to help improve Starshot. It is in active development and in use every day to keep making it better. If you want to help out, you can make an issue here on GitHub or join my [projects Discord server](https://discord.gg/WJD97fw) to discuss the app, suggest features, or report bugs.

When making an issue, please provide as much detail as possible, including steps to reproduce, screenshots and device information if relevant. There is an issue template to help guide you through the process.

## Roadmap

A current to-do list of features and improvements can be found in my [projects Discord server](https://discord.gg/WJD97fw) in the [#todos](https://discord.com/channels/365599795886161941/1468436633329205258) channel.

## Acknowledgments

- [RetroAchievements](https://retroachievements.org/) for the achievements API
- [RomM](https://romm.app/) for the API in their ROM management server
- [IGDB](https://www.igdb.com/) for game artwork and metadata
- [SteamGridDB](https://www.steamgriddb.com/) for game artwork
- [ScreenScraper](https://www.screenscraper.fr/) for game artwork and metadata
- The [Android](https://developer.android.com) and [Kotlin](https://developer.android.com/kotlin) communities for their excellent documentation and libraries
- [ES-DE](https://es-de.org/) for the structure of their ROM directories and metadata management

---

<p align="center">
  Made with ❤️ and impatience, for retro gaming enthusiasts & the dual-screen handheld community
</p>
