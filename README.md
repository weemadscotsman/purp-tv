# PURP TV

Play your games, watch your films and tune into your own channels on the big screen. Browse your collection by cover, find a title, or pick up a game together. PURP LINK brings the Windows folders you choose into the app over your home network.

PURP TV is free. Add your own games, media and any system files your emulators require.

## Download

| Device | Package |
| --- | --- |
| Fire TV, Android TV and compatible Android devices | [Android APK](https://github.com/weemadscotsman/purp-tv/releases/latest/download/PurpTV-public.apk) |
| Meta Quest | [Quest APK](https://github.com/weemadscotsman/purp-tv/releases/latest/download/PurpTV-Quest.apk) |
| Windows 10 or 11 | [PURP LINK EXE](https://github.com/weemadscotsman/purp-tv/releases/latest/download/PurpTV-Desktop.exe) |

See the [latest public release](https://github.com/weemadscotsman/purp-tv/releases/latest) for requirements, changes and SHA-256 checksums. Explore the app and setup on the [PURP TV website](https://purp-tv.netlify.app/).

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

## Historical verification for build 176

317 regression tests run: 315 passed, 2 skipped; 3 additional privacy tests passed. Mixed-HDR/4K Watch Together remains under hardware acceptance. 3D Cinema is not included. All 184 requirements remain tracked; this is not a claim of complete product acceptance.

[Release notes and exact checksums](https://github.com/weemadscotsman/purp-tv/releases/tag/v1.9.150)
