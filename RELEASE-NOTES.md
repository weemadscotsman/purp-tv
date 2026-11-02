# PURP TV Build 176 — 1.9.150-media-ready

This update preserves the purple launcher, Games, native Broadcast, Search, HDMI previews and nearby multiplayer.

## Changes
- Refined EPG focus, Up Next and aspect-aware previews; curated Archive shelf.
- Player readiness guards prevent controls querying an unprepared decoder.
- Broadcast starts at a validated programme offset and recovers from early playback completion.
- Watch Together recreates a failed decoder and avoids repeated seek requests during buffering.
- Desktop compatibility streaming keeps playlists and cached segments responsive while two encoders are busy, and identifies independently encoded segment boundaries.
- Desktop cache follows the user's profile instead of assuming an E: drive. Search imports use the installed application's folder.
- Native torrent metadata search feeds the existing player; metadata discovery alone is not proof of an available stream.

## Verification
- 317 regression tests run: 315 passed, 2 skipped; 3 additional privacy-scanner tests passed.
- Public APK privacy scan passed: empty bundled game catalogue, no developer box art or BIOS payloads. Original Android signing certificate retained.
- Desktop application-module and packaged-state scans passed. Windows executable is not Authenticode-signed.
- See release-manifest.json and SHA256SUMS.txt for exact binary identities.

## Known limitations
- Internet multiplayer is not released; nearby play uses the local network, with one host and one guest.
- 4K/mixed-HDR Watch Together and sustained host/guest playback remain under hardware acceptance. Compilation and first frames are not a complete playback pass.
- Some emulator prompts require gamepad buttons rather than remote OK; handheld link modes vary.
- Arbitrary third-party apps cannot be embedded as video-wall panes. Native HDMI behaviour depends on the television.
- Content availability, formats, torrent peers and provider authentication can prevent playback.
- 3D Cinema controls are requested follow-up work, not included in this release.
- REQUIREMENTS.json retains all 184 IDs; full product acceptance is incomplete.

## Install / update
Install PurpTV-public.apk on the Fire TV using Android's installer, or use `adb install -r PurpTV-public.apk` with ADB enabled. Update in place; do not clear app data. Confirm launcher/default-home permissions after an update. Run PurpTV-Desktop.exe on your own Windows 10/11 PC, choose the folders you want to share, and connect on the same network. No games, BIOS files, films, credentials or personal profiles are supplied.

## Rollback
The prior public v1.9.88 assets remain available on GitHub. Android normally refuses a version downgrade; preserve app data and do not uninstall merely to force one. The original signing certificate is unchanged.
