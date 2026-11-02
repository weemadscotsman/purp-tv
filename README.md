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
| **The TV app** | [PurpTV-public.apk](https://github.com/weemadscotsman/purp-tv/releases/download/v1.9.150/PurpTV-public.apk) — 297.5 MB, Android-signed release, build 176 |
| **The PC app** | [PurpTV-Desktop.exe](https://github.com/weemadscotsman/purp-tv/releases/download/v1.9.150/PurpTV-Desktop.exe) — 69.6 MB, Windows 10 or 11; unsigned Windows executable |

### SHA-256

```
ccccecf2012305327bd8135312a5a5c0c4eb9465283234248d4a3a01885392f3  PurpTV-public.apk
e585bf522df20fd0714d68ecc568f7c9dab0a9066b72af04985b51afe2ef9d7f  PurpTV-Desktop.exe
```

## Getting it running

1. **On the PC** — run Purp LINK, press *Auto-find game folders* or *Add folder…* to point at
   your own games, then *Start serving*.
2. **On the box** — install the APK. On a Fire TV: Settings → My Fire TV → Developer options →
   unknown sources, then open the file. Or side-load it with `adb install -r PurpTV-public.apk`.
3. **Same Wi-Fi** — the television finds the PC on your home network by itself. No pairing code,
   no account.
4. **Play** — open Games, pick a console, pick a game. It downloads from your PC and runs.

Some systems and games require your own compatible BIOS files. Compatibility varies by device and emulator.

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

## Build 176 verification and limitations

317 regression tests run: 315 passed, 2 skipped; 3 additional privacy tests passed. Mixed-HDR/4K Watch Together remains under hardware acceptance. 3D Cinema is not included. All 184 requirements remain tracked; this is not a claim of complete product acceptance.

[Release notes and exact checksums](https://github.com/weemadscotsman/purp-tv/releases/tag/v1.9.150)
