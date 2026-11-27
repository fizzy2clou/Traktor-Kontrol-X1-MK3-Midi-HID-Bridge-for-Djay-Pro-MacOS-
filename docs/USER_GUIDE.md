# User Guide — X1 × djay Bridge v1.2

**v1.2 is the stable version tested on the development Mac.** The GitHub-downloadable application is currently v1.1, which does not have dual BPM displays.

The bridge connects the Traktor Kontrol X1 MK3 over USB HID and exposes virtual MIDI ports for djay Pro.

## Menu-bar app

- **Start / Stop:** Start or stop the bridge without opening Terminal.
- **Warning threshold:** Choose how many seconds remain before the underglow starts blinking (20 seconds by default).
- **Show BPM while adjusting tempo (v1.2):** Enable or disable the temporary BPM screens.
- **BPM screen duration (v1.2):** Choose a return delay of 1–10 seconds (2 seconds by default).
- **Quit:** Close the application and stop the bridge.

## Dual BPM screens — new in v1.2

Both loop screens temporarily display the BPM of their **own** deck whenever you turn **either** mapped tempo knob:

| MIDI input | Left loop screen | Right loop screen |
| --- | --- | --- |
| CC 40 (Deck 1 tempo) | DECK 1 / Deck 1 BPM / BPM | DECK 2 / Deck 2 BPM / BPM |
| CC 41 (Deck 2 tempo) | DECK 1 / Deck 1 BPM / BPM | DECK 2 / Deck 2 BPM / BPM |

Each BPM display fills its 128 × 64 screen with **white lettering and large BPM digits on a black background**. No track title, loop size, loop text, or progress bar is drawn during BPM mode. Both loop screens enter and exit BPM mode together. Continuing to turn either knob keeps the screens in BPM mode; after the chosen delay they return to their normal loop displays together.

The bridge reads current BPM values from djay Pro through macOS Accessibility. **MIDI CC values trigger the display; they are not interpreted as BPM values.** The BPM feature can be disabled from the menu bar.

## MENU button banks

Press the hardware MENU button to toggle banks.

| Physical controls | Bank 1 (default) | Bank 2 |
| --- | --- | --- |
| Left FX buttons | FX 1–4, blue | FX 5–8, purple |
| Right FX buttons | FX 1–4, orange | FX 5–8, red |
| Left hotcue buttons | Cues 1–4 | Cues 5–8 |
| Right hotcue buttons | Cues 1–4 | Cues 5–8 |

The physical MENU illumination remains orange. The FX and underglow colors indicate the current bank.

## Hotcue LEDs

Hotcues follow djay's 16-color feedback palette. Existing cue slots display their assigned colors. Empty slots remain dim. The displayed physical slots follow the selected bank.

## Underglow

- Bank 1: blue left, orange right
- Bank 2: purple left, red right
- Below the configured remaining-time threshold while playback advances: the appropriate side blinks between its bank color and OFF
- Paused: the countdown-motion detector prevents ongoing blinking

## Five displays

Normal mode uses the loop screens for track, remaining time, progress and loop information, the FX screens for Neural Mix, and the center screen for the djay logo. During BPM mode **only the two loop screens** change.

## Troubleshooting

See [Setup and Troubleshooting](SETUP_AND_TROUBLESHOOTING.md).