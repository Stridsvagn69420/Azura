# Azura
A cross-platform music player featuring Rich Presence in Discord and Cyrkensia server repositories

# Installing
## Kagero (Cross-platform)
WIP.

## Pacman (Arch Linux)
WIP.

## XBPS (Void Linux)
WIP.

## DNF (Fedora)
WIP.

## APT (Ubuntu, Linux Mint)
WIP.

## Rust SDK
1. You need to install the [tauri-cli](https://tauri.app/v1/guides/getting-started/tauri-cli). I prefer using Cargo for this, so I'll have to run `cargo install tauri-cli --version "^1.0.0"`.
2. Clone the repository: `git clone https://github.com/Stridsvagn69420/Azura.git && cd Azura`.
3. Install all NPM dependencies: `npm i`
4. Build the Tauri application: `cargo tauri build`.
5. Your binary will be locaed at `src-tauri/target/release/azura[.exe]`.

<hr>

# The Fates-Audioplayer Project
The Fates-Audioplayer Project is a collection of apps/tools/servers to listen to music. It is called Fates-Audioplayer because I named the programs after characters/locations from [Fire Emblem Fates](https://fireemblem.fandom.com/wiki/Fire_Emblem_Fates). I originally made it *just* for Rich Presence in Discord, similar to Spotify.

## History
The original name was DiscordRPC-Player, written with WPF but supposed to be MAUI later, and there still might be some artifacts of it in the Git history.  
Later I decided to also add music repositories to share/distribute it better across devices. I soon realized that using C# would be too complicated for me, so I was thinking about Gtk,l Qt (developing with it is very good on Linux, but not Windows) or Electron, before I came across Tauri, which is basically Electron but way better in so many ways (it uses Rust).  
Shigure was also suppoed to use Flutter to run on iOS, Android and the Web, but playing music there with all features that I need is harder to do, so went to an Android-only native app.

## Comparision
|                | [Azura](https://github.com/Stridsvagn69420/Azura)              | [Cyrkensia](https://github.com/Stridsvagn69420/Cyrkensia) | [Shigure](https://github.com/Stridsvagn69420/Shigure) | [Azura-Web](https://github.com/Stridsvagn69420/Azura-Web)            |
| -------------- | -------------------------------------------------------------- | --------------------------------------------------------- | ----------------------------------------------------- | -------------------------------------------------------------------- |
| Origin of Name | Songstress and one of the main characters                      | City famous for its singers, dances and the Opera House   | Son of Azura and singer                               | (Like Azura, just with a Web suffix)                                 |
| Teck stack     | Rust, Svelte, Tauri                                            | Go, Fiber (Nginx or Apache Reverse Proxy)                 | Kotlin, Android Native                                | Svelte (Nginx or Apache)                                             |
| Target         | Linux, Windows (macOS supported)                               | Linux (Windows and others supported)                      | Android 10 or higher                                  | Web (Chrome, Chromium-based, Firefox)                                |
| Role           | Main desktop music player with all features (GTK/system theme) | Easy-to-use server for hosting music repositories         | Mobile music player with all features except RPC      | Web music player with all features except RPC (Custom theme for Web) |
