## 1.1.0

Projects saved with firmware 1.0 open on 1.1 after a quick update: opening one asks **UPDATE PROJECT TO CURRENT VERSION?**, or update them all at once with **Settings → MIGRATE ALL PROJECTS**. An updated project no longer opens on 1.0 firmware. Keep a copy first: download the project in the web editor before you update it. Your snapshot mappings keep their pads, and synced LFOs keep restarting when the clock starts.

### New
- **Rack BYPASS** silences a whole rack: notes, CC, clock and transport stop, and nothing you play reaches its devices. The rack keeps its settings. Find it under **RACKS** → hold **Select** on a rack → **BYPASS**. Map it to a knob, a MIDI control or an LFO, and choose with **IN SNAPSHOT** whether rack snapshots recall it. A bypassed rack is shaded in the rack list and its header reads **BYPASSED**.
- The new **RACK CTRL** knob macro turns a rack on and off: from the middle up the rack is bypassed, and **INVERT** swaps the ends. Perform shows the rack's name with **ON** or **OFF**, and the knob's Options open the rack with **EDIT THE RACK**.
- LFO **RE-TRIG** chooses when the wave restarts from its **PHASE** point: never (**OFF**), every time the LFO switches on (**ENABLE**), when the clock starts (**START**), or both (**BOTH**).
- One LFO can switch another LFO on and off: modulate its **ENABLED**.
- **MAP PAD** on a knob snapshot pad's Options gives that pad its own note, CC or Program Change. That pad then ignores the bank's mapping, so it can keep its own button.
- While a snapshot bank glides, the line under the header fills from left to right, so you can see when it lands. Arrange glides show it too.
- **Main Menu → SNAPSHOTS** opens **KNOBS**, **RACKS** and **LFOS**, so every snapshot bank is one step away.

### Improved
- Recalling a knob snapshot sets every device and LFO setting a knob controls to the knob's stored value, even when that device or LFO is **IN SNAPSHOT NO**. To keep one out of knob snapshots, set the knob's macro to **IN SNAPSHOT NO**. When one press recalls the knob bank with rack or LFO banks, the knob bank lands last, so your knobs have the final word.
- During a knob fade, a row that **ALLOW MORPH NO** holds keeps its bar still and blinks its value until it lands.
- Press the pad you're already on after changing something and it glides back over **FADE TIME**. Arrange does the same on every row; put **--** in a cell to leave that bank alone.
- Arrange plays exactly **LENGTH** rows, empty rows included, and **LENGTH** now goes down to **1** to repeat a single row.
- Mapping a whole knob snapshot bank to a note or Program Change starts at the number you send: it is pad **01** and the next 31 numbers follow, so note **E1** fills pads **01**–**32**.
- Snapshot mapping rows show what they are mapped to. Selecting a mapped row offers **LEARN AGAIN** or **REMOVE MAPPING** instead of removing it at once. In one bank the last key you learn takes over, and the S32 tells you which row lost it; other banks can still share that key.
- A setting takes one knob or one MIDI control: mapping it again replaces the old mapping, on the S32 and in the web editor.
- **Delay** on **SYNCED**: a tempo change also moves the echoes already playing.
- Dialogs with two buttons: turn the encoder to choose, and **Back** always cancels. Confirmations that delete, clear or overwrite something start on **BACK**.
- **IN SNAPSHOT** and **ALLOW MORPH** in Options edit like every other value: tap **Select**, turn, then tap **Select** or press **Back**. A single press no longer changes them.
- LFO **RATE** on **FREE** fine-tunes in 0.01 Hz steps, and turning fast still speeds up.

### Fixed
- A snapshot fade or morph that moves a setting down now lands exactly on the stored value instead of one step short.
- A snapshot recall that switches on an LFO that was off when the project loaded now makes it run.
- The MIDI output warning triangle in the header no longer blinks away when you click **Select**.
- **RANGE MIN** and **RANGE MAX** show their values when an LFO modulates another LFO's **WAVETABLE**, **SYNC** or synced **RATE**.
- Changing **IN SNAPSHOT** or **ALLOW MORPH** keeps the side menu's title.
- Unplugging and replugging a USB device while its power message is open no longer shows the message twice.
