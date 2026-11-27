# X1 × djay Bridge v1.2 — Release Notes

**Status:** Tested stable on the development Mac, **not yet packaged or published as a GitHub Release**.

## New in v1.2: Dual BPM display

When the user turns the knob sending **CC 40** (Deck 1 tempo) or **CC 41** (Deck 2 tempo), **both loop screens** temporarily switch to BPM mode:

- Left screen shows the current **Deck 1** BPM.
- Right screen shows the current **Deck 2** BPM.
- Both screens display a small centered deck label at the top, the BPM value in large white digits in the center, and **BPM** centered at the bottom.
- The background is black, with **no track title, loop text, loop size or progress bar**.
- Turning either knob extends the shared viewing period.
- Both screens return together to their normal loop layouts after the chosen delay.

The macOS menu-bar app adds **Show BPM while adjusting tempo** (enable/disable) and a **1–10 second duration** setting (2 seconds by default).

The MIDI CC values trigger the displays; **actual BPM is read through djay's Accessibility information**, not derived from MIDI values.

## Preserved from v1.1

- MENU button swaps FX 1–4 / FX 5–8 and Hotcues 1–4 / 5–8 on both decks.
- 16 dynamic djay hotcue colors
- Bank 1 blue/orange and Bank 2 purple/red FX and underglow
- Playback-aware warning flashing at a configurable remaining-time threshold
- Five X1 MK3 displays, Neural Mix indicators, and center logo
- Start/Stop menu-bar controls and X1 menu-bar icon

## Availability

The latest public installable ZIP remains **[v1.1](https://github.com/fizzy2clou/Traktor-Kontrol-X1-MK3-Midi-HID-Bridge-for-Djay-Pro-MacOS-/releases/tag/v1.1)** until a new v1.2 distribution is uploaded. Do not treat the available v1.1 ZIP as containing BPM mode.

Before releasing v1.2 publicly, package the final tested bridge and menu-bar application, include the Two Banks djay mapping, and test the complete installer on another Apple Silicon Mac.