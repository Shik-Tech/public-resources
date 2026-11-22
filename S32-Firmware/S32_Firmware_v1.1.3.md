## 1.1.3

### Improved
- You can remove a rack's MIDI IN or CLOCK at any time. The S32 reminds you with **RACK n NEEDS MIDI IN OR CLOCK FIRST** when you remove it and each time you open that rack, and a new MIDI IN or CLOCK goes straight to the top. A CLOCK at the top of a rack now stays there when you move devices.
- An **S32 LFO** macro now calls its setting row **PARAMETER**, and lists the LFO's settings in the same order as the LFO page.

### Fixed
- Loading a project now keeps every device in each rack. Before, devices placed above a rack's MIDI IN or CLOCK could disappear on load.
- **DUPLICATE RACK** now copies every device, in the same order, and the rack's **BYPASS** and **IN SNAPSHOT** setting.
- **CLEAR RACK** now also turns the rack's **BYPASS** off and its **IN SNAPSHOT** back on, like a new rack.
- Picking another LFO in an S32 LFO macro now resets MINIMUM and MAXIMUM to the setting's range.
- A fast turn of a macro's mode from SNAP or MORPH to MIDI DEVICE PARAMETER now resets the knob's range.
- Updating an older project from the Library now opens it, like any other project.
- Changing Arrange **LENGTH** to 256 no longer sends the playhead back to row 16.
