<p align="center">
  <img src="assets/icon.png" width="128" alt="NotchIsland icon">
</p>

<h1 align="center">NotchIsland</h1>

<p align="center">Dynamic Island for MacBooks with a notch · by <a href="https://github.com/theoron-apps">Theoron</a></p>

<p align="center">
  <a href="../../releases/latest"><b>Download</b></a> ·
  English · <a href="README.ru.md">Русский</a> · <a href="README.uk.md">Українська</a>
</p>

---

## Features

- **Music** — Apple Music, Spotify, Telegram songs and browser audio with a live equalizer and a glow around the island.
- **Notifications in the notch** — charging, AirPods and other Bluetooth devices, network and VPN changes, high temperature, volume.
- **Activities** — timer, Keep Awake, camera and microphone indicators, calls.
- **Shelf** — a file tray with AirDrop, clipboard history and a quick note.
- **Stats & battery** — CPU, memory, network, temperatures and power draw in watts.
- Three island styles, gestures, trackpad haptics. English, Ukrainian and Russian.

## Requirements

- macOS 26.7.1 or later
- A MacBook with a notch (other displays are supported as an option)

## Install

1. Download `NotchIsland-<version>.dmg` from [Releases](../../releases/latest).
2. Open the DMG and drag **NotchIsland** into **Applications**.
3. Open NotchIsland. macOS will say it can't verify the developer — click **Done**.
4. Open **System Settings → Privacy & Security** and scroll down to **Security**.
5. Click **Open Anyway** next to the NotchIsland message and confirm with your password or Touch ID.
6. Launch NotchIsland again — from now on it opens normally.

Why: the app isn't signed with a paid Apple Developer ID yet, so macOS asks you to confirm the first launch once.

> Advanced: instead of steps 3–5 you can run
> `xattr -dr com.apple.quarantine /Applications/NotchIsland.app`

## Permissions

| Permission | Why |
|---|---|
| Automation (Music, Spotify, System Events) | show the current track, control playback, switch the theme |
| System audio recording | the live equalizer reacts to real sound; nothing is recorded or saved |
| Bluetooth | notifications when headphones and other devices connect |
| Location | only so macOS reveals the Wi‑Fi network name |
| Clipboard | clipboard history, if you turn it on |

You can revoke any of them in **System Settings → Privacy & Security**.

## Update

Download the new DMG and replace the app in Applications. After an update the island shows what's new. Your settings are kept.

## Privacy

- The app runs in the macOS sandbox and collects no analytics.
- Clipboard history, notes and settings stay on your Mac.
- Network access is limited to the optional internet speed test (Apple's servers, the same service `networkQuality` uses) and a daily update check against this GitHub repository (can be turned off in About).

## Uninstall

Quit NotchIsland (right-click the island → Quit), delete it from Applications and, if you like, remove `~/Library/Containers/devplaceholder.WAZ2022C.NotchIsland`.

## Contact

News and support — Telegram [@TheoronApps](https://t.me/TheoronApps).
