# User Guide — X1 × djay Bridge v1.1

The X1 MK3 acts as a USB HID controller bridged to virtual MIDI ports for djay Pro on macOS.

## Menu-bar app
- **Start**: run the bridge
- **Stop**: stop the bridge
- **Warning threshold**: set the remaining-time point where underglow warning blinking begins
- **Quit**: close the app and bridge

## MENU banks
Press the hardware MENU button once to enter Bank 2; press again to return to Bank 1.

| Physical controls | Bank 1 | Bank 2 |
| --- | --- | --- |
| Left FX buttons | FX 1–4, blue | FX 5–8, purple |
| Right FX buttons | FX 1–4, orange | FX 5–8, red |
| Left hotcue buttons | Cues 1–4 | Cues 5–8 |
| Right hotcue buttons | Cues 1–4 | Cues 5–8 |

The MENU button's built-in orange illumination may remain unchanged. The FX and underglow colors indicate the selected bank.

## Hotcues
The eight physical hotcue buttons reflect the selected bank's cue slots. Existing cues light with their selected djay colors (16-color dynamic palette). Empty cues retain dim idle lighting.

## Underglow
- Bank 1: blue on left, orange on right
- Bank 2: purple on left, red on right
- During playback, when remaining time falls below the configured warning threshold, each side blinks between its bank color and OFF
- When paused, blinking stops after countdown-motion detection settles

## Displays
The X1's five screens display loop/deck information, Neural Mix icons, and a center djay logo. Display data is obtained using macOS Accessibility; Accessibility permissions must be enabled for live updates.

## Troubleshooting
See [Setup and Troubleshooting](SETUP_AND_TROUBLESHOOTING.md).
