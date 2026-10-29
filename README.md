# Purp TV

**YOUR TELLY. TAKEN BACK.**

A home screen for Fire TV, Firestick and Android TV. Your games on one endless shelf. Two
tellies playing the same game with no codes. Arcade CRT glow on every console. And a wee
reaper who naps on your buttons.

The launcher is free. It ships with no games, no BIOS files and no films — it plays the ones
you own.

## Get it

| | |
|---|---|
| **The TV app** | [PurpTV-public.apk](https://github.com/weemadscotsman/purp-tv/releases/download/v1.9.88/PurpTV-public.apk) — 276 MB, signed release, build 114 |
| **The PC app** | [PurpTV-Desktop.exe](https://github.com/weemadscotsman/purp-tv/releases/download/v1.9.88/PurpTV-Desktop.exe) — 36 MB, Windows 10 or 11 |

### SHA-256

```
a19cd1ae44ff59a0a09b87c021e5ea80c4b4b0446b3287f2fe61861195dc25b6  PurpTV-public.apk
d771d4c2a08c54cf2422558b51f0d22ee12a23df150b46803a09251d9554cf49  PurpTV-Desktop.exe
```

## Getting it running

1. **On the PC** — run Purp LINK, press *Auto-find game folders* or *Add folder…* to point at
   your own games, then *Start serving*.
2. **On the box** — install the APK. On a Fire TV: Settings → My Fire TV → Developer options →
   unknown sources, then open the file. Or side-load it with `adb install PurpTV-public.apk`.
3. **Same Wi-Fi** — the television finds the PC on your home network by itself. No pairing code,
   no account.
4. **Play** — open Games, pick a console, pick a game. It downloads from your PC and runs.

Dreamcast, N64, PC Engine and Neo Geo need your own BIOS in the game folder. Everything else
runs as it is.

## How it is built

The public APK is built from the same launcher as the internal one, with the developer's own
catalogue, artwork, firmware and machine paths taken out. The build refuses to publish if any
of it survived. The launcher then ships with an **empty** catalogue: everything on screen comes
from the PC you point at your own games from, over your own network.

## Known limits

- Play Together is home Wi-Fi only.
- One host and one guest per session.
- Fire OS will not put another app inside a Purp TV window. Your game and HDMI inputs can.
- A large disc-based game can be refused on a 4 GB Fire TV, because Purp TV keeps space free
  for app installs. The same game runs on a Fire Stick 4K Max.

Not affiliated with Amazon, Google or any console maker. Fire TV and Android TV are trademarks
of their owners. A DreamForge project · Edinburgh.
