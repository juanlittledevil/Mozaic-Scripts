# APC40 Mozaic Script User Manual

## Requirements
- iPad with the Mozaic app by Bram Bros.
- AUM or any DAW that supports MIDI routing.
- APC40 (first gen) MK1

## Installation Steps
1. Load Mozaic.
2. Press the CODE button.
3. Clear the code editor.
4. Paste the contents of APC40.moz.
5. Press the UPLOAD button.
6. Save the preset for future use (e.g., name it APC or APC40).

Repeat the above steps for APC-OUT.moz, saving it as APC-OUT or similar.

## Configuration Steps (AUM)
1. Create a new blank project.
2. Create 9 AUDIO tracks.
3. Add a MIDI track and load two Mozaic instances: one with APC-IN and the other with APC-OUT.
4. Configure MIDI routing:
   - APC-IN (receives MIDI from the APC40, sends MIDI to the APC40)
   - APC-OUT (receives MIDI from APC-IN, sends MIDI to "MIDI Control (built-in)" of AUM)
5. Initialize the APC40 by pressing Shift + Tap Tempo. Pads should change color to yellow.
6. Faders should be auto-mapped; manually map transport buttons, tap tempo, etc.
7. Optionally map arm, solo, mute buttons (ensure "CYCLE" is disabled, and "INVERT" is selected for mute).
8. To map the Mixer View, edit the Mozaic script's MIDI Controls and assign a pad using MIDI learn for "Show plugin."
9. Save your project as "Default" to load your setup automatically.

## Functionality
- **Encoder Selection**: APC40's "TRACK SELECTION" buttons select the encoder channel.
- **Pad Matrix**: Configure clip launch pads for different MIDI channels.
- **Mode Selection**: Buttons labeled "5 Detailed View" toggle between modes with different pad colors.
- **Cross Fader**: Sends MIDI on channel 9.
- **Cue Level**: Sends fixed signals on channel 10 (CC 47) for mapping to various functions.
- **Bank Select Arrow Buttons**: Currently unused.
- **Nudge and Tap Tempo**: Send MIDI note values.
- **Clip-Stop Pads**: Similar to Scene Launch buttons; useful for mapping Mozaic scripts.

## Using Tips
- Use APC-OUT for mapping functionality within your DAW. Do not use MIDI from APC or APC-IN for mapping.
- The script stores values for each encoder, bank, and channel.
- Save AUM project or Mozaic preset to retain settings.

## Additional Script
- Consider using the "cc-banks.moz" script for easily mapping knobs to CC messages with Mozaic.

Enjoy your enhanced APC40 experience with the Mozaic script!
