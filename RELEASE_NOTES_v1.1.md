# X1 × djay Bridge v1.1 — Release Notes

**Status:** v1.1 pre-release published, with downloadable Apple Silicon macOS distribution ZIP.

**[Download v1.1 ZIP](https://github.com/fizzy2clou/Traktor-Kontrol-X1-MK3-Midi-HID-Bridge-for-Djay-Pro-MacOS-/releases/download/v1.1/X1_djay_Bridge_v1.1_Distribution.zip)** · [Release page](https://github.com/fizzy2clou/Traktor-Kontrol-X1-MK3-Midi-HID-Bridge-for-Djay-Pro-MacOS-/releases/tag/v1.1)

## Included in distribution archive

- Apple Silicon macOS menu-bar application
- Runtime Rust HID↔MIDI bridge executable and macOS Accessibility helper
- Corrected X1 MK3 hardware descriptor and display support
- White menu-bar X1 icon and branded application icon
- **X1 MK3 Bridge Two Banks.djayMidiMapping** (65 mappings, 16 distinct cue-color values)
- Installer, uninstaller, and end-user documentation

## Features
- MENU button toggles FX and hotcue controls 1–4 / 5–8 on both decks
- Bank 1: blue/orange FX and underglow; Bank 2: purple/red
- Dynamic 16-color hotcue LEDs
- Five displays including deck/loop info and Neural Mix
- Configurable remaining-time underglow blink with pause detection
- Start/Stop from macOS menu bar

## File identification
`X1_djay_Bridge_v1.1_Distribution.zip`

SHA-256:
```
2c395dfbb2e77c55925b0f58395bec994db388253ff649bfeeb200d201241b78
```

## Release checklist
Before advertising the release as stable, test installation and operation on another Apple Silicon Mac, and review third-party logo/dependency redistribution rights. This binary is ad-hoc signed and not notarized by Apple.

The downloadable ZIP is attached to the **published v1.1 pre-release**. Install it using the bundled `INSTALL.command` and select the bundled **X1 MK3 Bridge Two Banks** mapping in djay Pro.
