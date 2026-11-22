# X1 × djay Bridge

**A macOS menu-bar HID-to-MIDI bridge for the Native Instruments Traktor Kontrol X1 MK3 and djay Pro.**

**Version:** 1.1  
**Platform:** Apple Silicon macOS (other architectures unverified)  
**Status:** Community release candidate.

> Independent community project. Not affiliated with or endorsed by Native Instruments or Algoriddim.

## Download

**The v1.1 app archive has not been uploaded yet.** When available, download it from [GitHub Releases](../../releases). The release archive must be generated from the tested app on the maintainer's Mac.

## Features

- Menu-bar app: **Start**, **Stop**, and adjustable remaining-time warning threshold
- Five X1 MK3 screens for loops, track information, Neural Mix, and center logo
- **MENU** switches both decks' FX and hotcue controls between 1–4 and 5–8
- All **16 djay hotcue colors**, displayed on corresponding X1 LEDs
- FX LED colors: Bank 1 blue/orange; Bank 2 purple/red
- Twelve underglow LEDs, following bank colors and blinking color/OFF near track end
- Countdown-based pause detection, avoiding false blinking when paused
- djay Pro **X1 MK3 Bridge Two Banks** MIDI mapping packaged with the app distribution

## Requirements

- Native Instruments Traktor Kontrol X1 MK3 via USB
- djay Pro for macOS
- Apple Silicon Mac (other architectures untested)
- macOS Accessibility permission for track and loop information

## Installation

Once the distribution ZIP is published:

1. Download and extract `X1_djay_Bridge_v1.1_Distribution.zip` from [Releases](../../releases).
2. In Terminal, navigate to the extracted `X1 djay Bridge v1.1` folder and run `bash INSTALL.command`.
3. Open the app in `~/Applications`. Its white X1 icon appears in the menu bar.
4. In djay's MIDI configuration, select **X1 MK3 Bridge Two Banks** for the X1 bridge MIDI ports.
5. Set the desired warning threshold in the menu-bar controls.

See [Installation](docs/INSTALLATION.md) and [Troubleshooting](docs/SETUP_AND_TROUBLESHOOTING.md).

## Bank controls

| Control | Bank 1 | Bank 2 (MENU) |
| --- | --- | --- |
| Left FX | FX 1–4 (blue) | FX 5–8 (purple) |
| Right FX | FX 1–4 (orange) | FX 5–8 (red) |
| Left hotcues | Cues 1–4 | Cues 5–8 |
| Right hotcues | Cues 1–4 | Cues 5–8 |
| Underglow | Blue/orange | Purple/red |

Read the [User Guide](docs/USER_GUIDE.md).

## Compatibility and security

This first release is not Developer ID notarized; macOS may request explicit first-run approval in **System Settings → Privacy & Security**. Do not disable Gatekeeper globally. Close Traktor and other bridge instances before connecting the X1.

## Source and licensing

This repository initially contains documentation only. The tested Rust source tree and packaged macOS app have **not** yet been uploaded. A license has not been selected, so no open-source reuse rights are granted by default. Review third-party dependencies, branding, and redistribution rights before publishing binaries/source.

## Documentation

- [Installation](docs/INSTALLATION.md)
- [User Guide](docs/USER_GUIDE.md)
- [Setup and troubleshooting](docs/SETUP_AND_TROUBLESHOOTING.md)
- [Release checklist](docs/RELEASE_CHECKLIST.md)
