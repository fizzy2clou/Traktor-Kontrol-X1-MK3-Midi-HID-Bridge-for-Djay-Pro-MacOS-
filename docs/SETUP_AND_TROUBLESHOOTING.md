# Setup and Troubleshooting

## The app doesn't appear in Applications
Check `~/Applications` (your user Applications folder), not only `/Applications`. The bridge is a menu-bar app and may not show a normal window when running.

## No MIDI control in djay Pro
- Ensure the menu-bar app says the bridge is running.
- Select **X1 MK3 Bridge Two Banks** in djay's MIDI preferences.
- Ensure djay is connected to the bridge's virtual MIDI ports.
- Restart djay after installing a mapping.
- Avoid running another bridge instance.

## Buttons have colors but not the expected hotcue slots
Press MENU to switch between 1–4 and 5–8. Verify the Two Banks mapping is selected, not the older Dynamic Color Test mapping.

## Hotcue LEDs do not match djay colors
Ensure the installed mapping includes the unique 16-color `userInfo.padColorsActive` palette. Older mappings with duplicate palette values cannot distinguish all 16 colors.

## Displays don't update
Enable macOS Accessibility permissions for the app/helper process as prompted. Quit and reopen the app and djay. The initial deck discovery may take several seconds.

## Track-ending underglow blinks while paused
The bridge estimates whether playback is moving from remaining-time changes. It should stop warning after countdown motion ceases. Confirm the Accessibility reader is operating and restart the app if needed.

## macOS says the app can't be verified
This build is not notarized. Review the specific security prompt in **System Settings → Privacy & Security** and approve only if you trust the source. Do not disable Gatekeeper globally.

## Controller not found
Connect the X1 MK3 directly over USB, check power/cable, and close Native Instruments Traktor or other software claiming the device.

## Logs
Use **Open Bridge Log** in the menu-bar app if present. Include macOS version, djay version, and the last relevant log lines when reporting an issue. Do not post personal paths, credentials, or sensitive song/library data publicly.
