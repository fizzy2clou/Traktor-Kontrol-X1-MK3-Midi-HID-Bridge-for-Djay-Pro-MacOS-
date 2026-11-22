# Installation — X1 × djay Bridge v1.1

**The compiled distribution ZIP is not available on GitHub yet.** These instructions apply once the maintainer uploads the release asset.

## Requirements
- Apple Silicon Mac
- Native Instruments Traktor Kontrol X1 MK3 connected via USB
- djay Pro for macOS
- Permission to use macOS Accessibility for live deck information

## Install
1. Download `X1_djay_Bridge_v1.1_Distribution.zip` from the repository's Releases page.
2. Extract it. Open Terminal in the extracted `X1 djay Bridge v1.1` folder.
3. Run `bash INSTALL.command`.
4. Find `X1 djay Bridge v1.1.app` in `~/Applications`.
5. Start the app. The white X1 icon will appear in the macOS menu bar.
6. Open djay Pro and choose **X1 MK3 Bridge Two Banks** as the mapping for the bridge's virtual MIDI ports.
7. Use the menu-bar icon to Start/Stop the bridge and adjust warning seconds.

The installer is intended to include both the app and the `X1 MK3 Bridge Two Banks.djayMidiMapping` file. Confirm both are present in the release ZIP.

## Mac security
The first community package is not notarized. If macOS blocks opening it, visit **System Settings → Privacy & Security** to review the app-specific Open Anyway option. Never disable Gatekeeper globally.

## Accessibility permission
If the deck displays do not update, grant the bridge's launched process the relevant Accessibility permission under **System Settings → Privacy & Security → Accessibility**, then restart the bridge.

## Important
Close Traktor and any other running copy of the bridge to avoid competing for the X1. If the MIDI mapping is not visible immediately in djay Pro, quit and restart djay.
