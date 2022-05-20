# flipper-music-files
Music files in .fmf format for the Flipper Zero Music Player plugin

## How to use these files

1. Attach your Flipper to your computer and open qFlipper.
2. Click on the File manager tab, then SD Card, then music player. 
3. In there should be the file for Marble_Machine.fmf. Copy your new files into that folder, and the player should immediately be able to find them.

## Making Your Own Music

.fmf files should have the following format:

```
Filetype: Flipper Music Format
Version: 0
BPM: <integer beats per minute>
Duration: <default note duration>
Octave: <default octave>
Notes: <comma-delimited list of notes>
```

### Note Format

`<duration><note|rest><sharp><octave><dots>`

duration: number between 1 & 128, defaults to project duration. 4 is a quarter note, 2 is a half note.
note: A through G or P for pause (rest)
sharp: # or omitted
octave: between 1 & 16, defaults to project octave
dots: between 1 & 16 '.' characters. Each dot makes the note half again as long.

#### Examples:

8C4 - Eight note pitch of C, fourth octave

4A#5. - Dotted quarter note pitch of A sharp, fifth octave

2P - Half note rest
