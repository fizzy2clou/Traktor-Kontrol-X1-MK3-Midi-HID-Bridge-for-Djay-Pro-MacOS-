# Installation — X1 × djay Bridge

## Published download: v1.1

**[Download v1.1 for Apple Silicon macOS](https://github.com/fizzy2clou/Traktor-Kontrol-X1-MK3-Midi-HID-Bridge-for-Djay-Pro-MacOS-/releases/download/v1.1/X1_djay_Bridge_v1.1_Distribution.zip)**.

**Version note:** v1.2 has been tested as the stable version on the developer's Mac, but **the installable v1.2 ZIP is not yet published**. The v1.1 ZIP does not include the dual BPM-screen feature described in the [v1.2 user guide](USER_GUIDE.md).

## Requirements

- Apple Silicon Mac
- Native Instruments Traktor Kontrol X1 MK3, connected via USB
- djay Pro for macOS
- macOS Accessibility permission for live deck information

## Install the currently published v1.1

1. Download `X1_djay_Bridge_v1.1_Distribution.zip` from the [v1.1 release](https://github.com/fizzy2clou/Traktor-Kontrol-X1-MK3-Midi-HID-Bridge-for-Djay-Pro-MacOS-/releases/tag/v1.1).
2. Extract the archive and open Terminal in the extracted `X1 djay Bridge v1.1` folder.
3. Run `bash INSTALL.command`.
4. Find `X1 djay Bridge v1.1.app` in `~/Applications`.
5. Launch it and use the white X1 menu-bar icon to start the bridge.
6. In djay Pro, select the included **X1 MK3 Bridge Two Banks** MIDI mapping for the bridge's virtual MIDI ports.
7. Configure your preferred underglow warning threshold.

The distribution includes the MIDI mapping and an installer.

## Installing v1.2 when released

After a tested v1.2 distribution archive is uploaded, follow its own installation instructions and ensure only one bridge version is running. **Do not assume that the v1.1 ZIP contains the v1.2 BPM features.**

## macOS security and permissions

The community build is not notarized. If macOS blocks the app, use its app-specific approval under **System Settings → Privacy & Security**; do not disable Gatekeeper globally. Allow Accessibility access to the bridge/helper for live track/loop/BPM details. Restart the app after granting permission.

Close Traktor and any other running bridge instance to avoid contention for the controller. Restart djay Pro if its new MIDI mapping does not appear immediately.