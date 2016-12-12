#Zeno’s Music Box
This Pure Data patch is a random sample player. Although quite simple, it can create some beautiful landscapes and generate music infinitely.

It will also fade in & out each sample, which is important to avoid clipping and also lends a more human feel to the performance. The ‘Global Rate’ will adjust the amount of time until the next sample is triggered and is fun to play with intuitively. The ‘Sample Stop’ will fade out the current sample and is useful for creating quiet moments. The blue boxes are related to reverb, which it vital to hiding the transitions between samples.

###Requires use of Pd-Extended
http://puredata.info/downloads/pd-extended/releases/0.43.4

###Watch a demo
[![Zeno’s Music Box Demo](https://img.youtube.com/vi/lKmvMRn6uU0/0.jpg)](https://www.youtube.com/watch?v=lKmvMRn6uU0)

###Want to add your own samples?
For example, you have 71 WAV’s you want to input. So let’s edit “ZenosMusicBox_NilsFrahm.pd”
- First you need to rename your WAV’s so that they are numbered sequentially.
  - *`Example_1.wav, Example_2.wav, Example_3.wav...`*
- Within Pd, edit the open message box with the relevant filename.
  - *Before: `open WAVs/NilsFrahm_$1.wav start`*
  - *After: `open WAVs/Example_$1.wav start`*
- Within Pd, edit the ‘Random’ object box to be a number which matches the amount of WAV’s you have.
  - *Before: `random 48`*
  - *After: `random 71`*
- Done! Just turn up the ‘output~’ volume and click the ‘Begin & End’ toggle to start playback.

###Credits
I’d like to give a shout out to the amazing musicians which I’ve cutup and sampled in this patch.
- Ayako Hotta-Lister - London No Yoru No Ame (Album: The Japanese Koto)
- Nils Frahm - Part II (Album: Electric Piano)
