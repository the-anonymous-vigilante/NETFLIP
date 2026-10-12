<div align="center">

# NETFLIP

**Thousands of Movies & Series for FREE — Netflix & Prime Video, all in one app.**

Action, thriller, romance, sci-fi & more. No subscription, no sign-up, no hidden charges.

![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=for-the-badge&logo=kotlin&logoColor=white)
![Compose](https://img.shields.io/badge/Jetpack_Compose-4285F4?style=for-the-badge&logo=jetpackcompose&logoColor=white)
![Android](https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=white)

</div>

---

## Features

- **Streaming** — thousands of movies & series, latest hits & timeless classics
- **Built-in ad blocking** — interruption-free watching
- **Smart search** — fast search with search-history
- **Watchlist** — save favourites, stored locally with Room database
- **Netflix-style dark UI** — cinematic theme, edge-to-edge, bottom navigation
- **Modern Android stack** — Jetpack Compose + Material 3, minSdk 24

## Screens

- **Home** — trending header + poster rows
- **Search** — overlay search with history chips
- **Watchlist** — saved videos, offline-ready database
- **Profile** — settings & preferences

> Screenshots coming soon — contributions welcome!

## Tech Stack

- **Language:** Kotlin
- **UI:** Jetpack Compose (BOM) + Material 3
- **Database:** Room (SavedVideo, Watchlist, SearchHistory)
- **AI:** Gemini API (server-side, via `.env`)
- **Build:** Gradle KTS, compileSdk 36, Java 11

## Getting Started

**Prerequisites:** Android Studio (Ladybug+), JDK 11+, Android SDK 36, device/emulator with Android 7.0+

```bash
git clone https://github.com/the-anonymous-vigilante/NETFLIP.git
cd NETFLIP
cp .env.example .env
# Edit .env and add your key: GEMINI_API_KEY=your_key_here
```

Free key: https://aistudio.google.com/app/apikey

Then open in Android Studio, Sync Gradle, and press Run. Or via CLI:

```bash
./gradlew assembleDebug
adb install app/build/outputs/apk/debug/app-debug.apk
```

## Project Structure

```
NETFLIP/
├── app/src/main/java/com/example/
│   ├── MainActivity.kt       # Navigation + Scaffold entry
│   ├── data/                 # Room: AppDatabase, SavedVideo, Watchlist, SearchHistory
│   ├── ui/theme/             # Color.kt, Theme.kt, Type.kt (Netflix palette)
│   └── SearchOverlay.kt      # Search UI
├── app/src/main/res/         # Strings, colors, themes, icons
├── assets/                   # Bundled assets
└── .env.example              # GEMINI_API_KEY template
```

## Contributing

1. Fork → branch `feat/your-feature` → commit → push → open PR to `main`
2. Follow the official Kotlin code style

UI polish, bug fixes and new providers are all welcome!

## Disclaimer

> NETFLIP is an educational UI demo. It hosts no content — all data comes from third-party sources. Please respect copyright laws in your country.

## License

Forked from [arafathrahman710/NETFLIP](https://github.com/arafathrahman710/NETFLIP). No license file yet — all rights reserved by default.

---

<div align="center">

Made with love by **@the-anonymous-vigilante** — star this repo if you like it!

</div>
