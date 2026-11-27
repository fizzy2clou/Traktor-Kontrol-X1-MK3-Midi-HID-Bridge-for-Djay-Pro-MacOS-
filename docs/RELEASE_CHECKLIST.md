# Release Checklist — v1.2

**Current state:** Stable and working on the development Mac. **GitHub still distributes v1.1** until the v1.2 app is packaged and uploaded.

- [x] Test CC 40 trigger for Deck 1 tempo and CC 41 for Deck 2 tempo
- [x] Verify either tempo knob causes both loop screens to show their respective deck BPM
- [x] Verify fullscreen white BPM text on a black background without the usual loop UI
- [x] Verify both screens return to their normal loop views together
- [x] Confirm v1.2 works in the developer's controller setup
- [ ] Package the latest tested **v1.2** macOS app; do not inadvertently package an earlier v1.2 patch
- [ ] Verify the menu-bar app retains BPM enable/disable and its 1–10 second timeout
- [ ] Include **X1 MK3 Bridge Two Banks.djayMidiMapping**, the bridge executable, Accessibility helper, HID descriptor, icons, installer and documentation
- [ ] Test the complete packaged v1.2 install on a second Apple Silicon Mac
- [ ] Verify both banks, all 16 cue colors, Neural Mix screens, underglow and warning behavior after installation
- [ ] Confirm only one bridge instance runs at a time
- [ ] Review redistribution rights, branding and third-party dependencies
- [ ] Consider Apple Developer ID signing and notarization
- [ ] Create and publish GitHub Release **v1.2** with the actual tested v1.2 distribution ZIP
- [ ] Update README to replace the v1.1 download link once v1.2 is live