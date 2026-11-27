# Setup and Troubleshooting

## Which version supports the dual BPM display?

**v1.2**, tested on the developer's X1 MK3. The public v1.1 ZIP does not support it; a v1.2 distribution has not yet been published.

## The app doesn't appear in Applications

Check `~/Applications`, not only `/Applications`. The bridge is a menu-bar app and does not need to open a normal window.

## No MIDI control in djay Pro

- Ensure the menu-bar app has started the bridge.
- Select **X1 MK3 Bridge Two Banks** in djay MIDI preferences.
- Check that djay is using the bridge's virtual MIDI ports.
- Restart djay after installing the mapping.
- Avoid running another bridge instance.

## BPM screens do not appear (v1.2)

- Enable **Show BPM while adjusting tempo** in the menu-bar controls.
- Verify that the tempo knobs send **CC 40 (Deck 1)** and **CC 41 (Deck 2)**.
- The BPM view should start on **both** loop screens whenever either knob moves.
- Confirm the bridge has macOS Accessibility permission for djay's BPM display.
- Ensure you are actually running the updated **v1.2** app, not v1.1.

## BPM is blank or outdated (v1.2)

The MIDI controller only triggers BPM mode. BPM values are read from djay Pro through Accessibility. If the UI labels are unavailable or change in a djay update, the reader may need adjustment. Check Accessibility access and restart both apps.

## BPM covers the loop title or progress bar (v1.2)

This was fixed in the tested v1.2 renderer. The BPM screens should be dedicated **white-on-black fullscreen views** with only the deck label, large number and BPM label. Make sure the final v1.2 fixes are installed.

## Only one loop screen shows BPM (v1.2)

The completed stable v1.2 uses a shared activation behavior: turning **either CC 40 or CC 41** must show **both decks' BPM simultaneously**, then both return to loop displays after the configured delay. Older v1.2 patches lacked this behavior.

## Buttons show unexpected hotcues

Press MENU to switch between cues 1–4 and 5–8. Confirm the **Two Banks** mapping is selected, not the old Dynamic Color Test mapping.

## Hotcue colors do not match djay

Use the mapping containing the 16 distinct `userInfo.padColorsActive` values. Mapping edits may require restarting djay.

## Normal displays do not update

Enable Accessibility permissions for the app/helper and restart. Live track, remaining-time, loop, and BPM data depend on macOS Accessibility.

## Underglow warning blinks when paused

The bridge detects movement of the remaining-time countdown to suppress blinking when paused. Check Accessibility and restart the bridge if detection is stale.

## The app can't be verified

The community binary is not notarized. Review the app-specific first-run approval under **System Settings → Privacy & Security**. Do not disable Gatekeeper globally.

## Controller not found

Reconnect the X1 MK3 over USB, check power/cable, and close Traktor or other programs claiming the HID device.

## Logs

Use **Open Bridge Log** if present. When reporting issues, include relevant recent messages and macOS/djay versions, but redact personal paths, credentials and sensitive library information.