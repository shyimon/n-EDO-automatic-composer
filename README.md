# n-EDO Automatic Composer
## ⚠️ The project is currently a mess
The project hit its initial goal so i decided to upload it, but it's quite messy.
I'm not sure about the copyight issues that might emerge by putting amen break slices here, I'll keep an eye on that.

Also, the documentation is non-existent for now and the code is messy and mostly uncommented. The few comments and labels are in mixed language (some in italian, some in english). As stated, it's a mess. If you want to work or have fun with it, good luck.

## 🔧 What does this patch do?
* It generates a breakbeat you can control the randomness of with the parameter beat_randomness;
* It generates a harmony in triads with respects to the EDO scale chosen;
* It generates a melody in the same fashion.

You can control the BPM, the beat randomness, the EDO, and mix the four channels (amen break, synthesized drums, harmony and melody) and the master separately. You can also control the master frequency but it resets the melody envelope, i'll have to look into that.
Finally, you can start and stop the whole thing via the sequencer control toggle.

The patch is developed with controls from the Akai MIDImix in mind; even then, it's quite finnicky. You'll need to push 'send all' and mess around with some knobs to make it work properly, but here is a reference for the MIDI controls, I hope it helps

* `ctlin 1`: BPM, range 60 to 220
* `ctlin 3`: control master hz, range 150 to 300
* `ctlin 4`: controls the amount of melody and bass in the mix. Range from 'only melody' to 'only bass'
* `ctlin 9`: control beat randomness
* `ctlin 25`: the button starts the sequencer
* `ctlin 41`: the button stops the sequencer after finishing the current bar
* `ctlin 27`: push to decrese the number of notes the octave gets split into by 1; takes effect on next beat
* `ctlin 43`: push to increase the number of notes the octave gets split into by 1; takes effect on next beat
* `ctlin 49` to `ctlin 51`: the faders to control the mix; respectively they control the volumes of the amen break, the synth drums, the harmony and the melody/bass
* `ctlin 57`: fader to control the master volume
