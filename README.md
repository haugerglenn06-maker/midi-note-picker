# MIDI Note Picker

A JSFX MIDI filter for REAPER. Pick exactly which MIDI notes are allowed through
by clicking keys on a piano keyboard. Only the selected notes pass – nothing in
between, unlike range-based note filters.

Perfect for splitting a drum kit into one track per drum: choose 36 for the kick,
or 42 + 44 + 46 for a hi-hat track where closed and open hats choke each other.

## Features
- Clickable 5-octave piano keyboard – click or drag to select notes
- Overview strip of all 128 notes and octave buttons
- Built-in General MIDI drum and percussion presets
- Learn mode: select notes by playing them
- Follows your MIDI keyboard's octave changes (works with any controller size, with calibration)
- Shows incoming notes and the GM drum name for each key
- Optional MIDI channel filter and pass-through of other MIDI (CC, pitch bend …)
- No stuck notes – note-offs always pass when their note-on did
- Selection is saved with the project and in FX presets

## Installation with ReaPack
1. In REAPER: **Extensions → ReaPack → Import repositories…**
2. Paste:
   ```
   https://raw.githubusercontent.com/haugerglenn06-maker/midi-note-picker/main/index.xml
   ```
3. **Extensions → ReaPack → Browse packages**, search for *MIDI Note Picker* and install.

## Manual installation
Copy `MIDI/midi_note_picker.jsfx` to your REAPER `Effects` folder
(Linux: `~/.config/REAPER/Effects/`), then press F5 in the FX browser.

## Tip
Use it as **track input FX** so only the selected notes are recorded on each track.

## Author
Glenn Hauger

Questions, bug reports and feature requests: please open an issue at https://github.com/haugerglenn06-maker/midi-note-picker/issues

## License
MIT – see [LICENSE](LICENSE).
