# X1 × djay Bridge

**A macOS menu-bar HID-to-MIDI bridge for the Native Instruments Traktor Kontrol X1 MK3 and djay Pro.**

**Current tested version:** v1.2 (stable on the development X1 MK3 setup)  
**Latest public download:** v1.1 (Apple Silicon macOS pre-release)  
**Platform:** Apple Silicon macOS; other architectures not verified.

> Independent community project. Not affiliated with or endorsed by Native Instruments or Algoriddim.

## Download and version status

**[Download X1 × djay Bridge v1.1 for macOS](https://github.com/fizzy2clou/Traktor-Kontrol-X1-MK3-Midi-HID-Bridge-for-Djay-Pro-MacOS-/releases/download/v1.1/X1_djay_Bridge_v1.1_Distribution.zip)** — the currently published ZIP includes the menu-bar application, installer and **X1 MK3 Bridge Two Banks** djay MIDI mapping.

**v1.2 has been tested successfully on the development Mac, but its installable distribution ZIP has not yet been published to GitHub.** The BPM feature described below requires v1.2; downloading v1.1 will not install it. See [v1.2 release notes](docs/V1_2_RELEASE_NOTES.md).

## Features

- **Native macOS menu-bar controls:** Start/Stop, adjustable end-of-track underglow warning, and (in v1.2) an optional BPM display with adjustable timeout.
- **Five X1 MK3 displays:** deck/loop information, loop size/progress, Neural Mix icons and center djay logo.
- **New in v1.2 — dual BPM screens:** Turning either tempo knob (CC 40 for Deck 1 or CC 41 for Deck 2) temporarily switches **both loop screens** to BPM, showing each deck's live djay BPM simultaneously. Large white digits on black, centered DECK 1 / DECK 2 at the top and BPM at the bottom. Both return to their usual loop information together after the configured delay.
- **MENU button banks:** FX and hotcues 1–4 in Bank 1 or 5–8 in Bank 2 on both decks.
- **16-color hotcue LEDs:** per-slot MIDI color feedback from djay Pro.
- **Bank-aware lighting:** Bank 1 blue/orange FX and underglow; Bank 2 purple/red. Inactive controls remain dim.
- **Track-ending warning:** bank-colored underglow flashes color/OFF as remaining time passes the configured threshold while playback advances; pauses stop the flashing.

## Dual BPM display (v1.2)

| Tempo control | Left loop screen | Right loop screen |
| --- | --- | --- |
| Turn CC 40 — Deck 1 | Deck 1 current BPM | Deck 2 current BPM |
| Turn CC 41 — Deck 2 | Deck 1 current BPM | Deck 2 current BPM |
| Stop turning | Both return to normal loop information after the configured delay | |

Enable **Show BPM while adjusting tempo** in the menu-bar application. Adjust the **BPM screen duration** (1–10 seconds, default 2 seconds). BPM values are read from djay Pro via macOS Accessibility, not calculated from the MIDI CC position.

## Bank controls

| Physical controls | Bank 1 (default) | Bank 2 (MENU) |
| --- | --- | --- |
| Left FX | Deck 1 FX 1–4, blue | Deck 1 FX 5–8, purple |
| Right FX | Deck 2 FX 1–4, orange | Deck 2 FX 5–8, red |
| Left hotcues | Cues 1–4 | Cues 5–8 |
| Right hotcues | Cues 1–4 | Cues 5–8 |
| Underglow | Blue / orange | Purple / red |

## Requirements

- Native Instruments **Traktor Kontrol X1 MK3** connected over USB
- **djay Pro** for macOS
- **Apple Silicon Mac** (other architectures untested)
- macOS Accessibility permission for track, loop and BPM information

## Installation

For the **currently published v1.1**, download the ZIP above, extract it, and run `bash INSTALL.command` from the extracted `X1 djay Bridge v1.1` folder. Find the app under `~/Applications`, select **X1 MK3 Bridge Two Banks** in djay's MIDI preferences, and start the bridge from its white X1 menu-bar icon.

**Do not use v1.1 installation instructions as a v1.2 upgrade procedure.** The v1.2 distribution and installation instructions will be added when the tested v1.2 app is packaged. See [installation guide](docs/INSTALLATION.md).

## Documentation

- [User guide (v1.2 behavior)](docs/USER_GUIDE.md)
- [v1.2 release notes](docs/V1_2_RELEASE_NOTES.md)
- [Installation and version status](docs/INSTALLATION.md)
- [Setup and troubleshooting](docs/SETUP_AND_TROUBLESHOOTING.md)
- [Release checklist](docs/RELEASE_CHECKLIST.md)

## Security, source and licensing

The published v1.1 app is not Developer ID notarized and may require explicit first-run approval through macOS Privacy & Security. Do not disable Gatekeeper globally. Close Traktor and competing bridge instances before use.

The current Rust source tree has not yet been published in this repository. No open-source license has been selected. Review dependency and trademark redistribution rights before republishing binaries or source.
