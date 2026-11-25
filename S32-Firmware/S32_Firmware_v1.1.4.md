## 1.1.4

### Improved
- Open side menus and the device cards on a rack now update by themselves when a value changes from outside (a knob macro, mapped MIDI, an LFO, the web editor or a snapshot recall), with no need to move the encoder.
- Step changes you make on the S32 (step values, pads, Randomize) now show in the web editor right away, and the editor's "show on the S32" lands on the Step Seq or Euclid setting you clicked, also when that screen is already open.

### Fixed
- A message box no longer appears over a stale screen: the screen behind it now follows the S32 (for example after you enter a rack, or when a menu closes).
- The web editor's view commands now close any open side menu first.
- A rack's **MIDI IN** no longer lists **MIDI2** as a **PORT**: the S32 has one MIDI input, **MIDI1**. Knobs, LFOs and MIDI mappings on MIDI IN PORT now move evenly over the real ports. A project or snapshot saved with MIDI IN on MIDI2 opens with it on MIDI1.
