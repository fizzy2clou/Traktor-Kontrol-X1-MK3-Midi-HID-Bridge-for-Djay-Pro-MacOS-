# v1.1 Release Checklist

- [ ] Generate `X1_djay_Bridge_v1.1_Distribution.zip` on the working Apple Silicon Mac using the previously provided release kit.
- [ ] Verify the ZIP includes the macOS `.app`, install/uninstall scripts, documentation, and `X1 MK3 Bridge Two Banks.djayMidiMapping`.
- [ ] Check bundled resources: Rust bridge executable, Accessibility helper, HID descriptor, display assets, and white menu-bar template icon.
- [ ] Scan all published files for credentials, keys, and local/private data.
- [ ] Review dependencies and third-party logos/trademarks for redistribution rights.
- [ ] Test install from ZIP on a second Apple Silicon Mac.
- [ ] Test virtual MIDI ports and mapping selection in djay.
- [ ] Test MENU Bank 1 and Bank 2 outgoing notes and incoming LED feedback.
- [ ] Test 16 cue-point colors on both decks.
- [ ] Test all five displays, pause detection, warning threshold, and both bank underglow palettes.
- [ ] Test Start, Stop, Quit, and reinstall/uninstall workflow.
- [ ] Create GitHub Release tag `v1.1`; attach the tested ZIP.
- [ ] Mark release as prerelease until additional Mac compatibility is validated.
- [ ] Consider Developer ID signing and notarization for broader distribution.
