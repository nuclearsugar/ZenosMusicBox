#Zeno’s Music Box
This Pure Data patch is a random sample player. Although quite simple, it can create some beautiful landscapes and generate music infinitely.

It will also fade in & out each sample, which is important to avoid clipping and also lends a more human feel to the performance. The `Global Rate` will adjust the amount of time until the next sample is triggered and is fun to play with intuitively. The `Sample Stop` will fade out the current sample and is useful for creating quiet moments. The blue boxes are related to reverb, which are vital to hiding the transitions between samples.

###Requires use of Pd-Extended
It's free and open source. Available for Mac, Windows, & Linux.<br>
http://puredata.info/downloads/pd-extended/releases/0.43.4

###Watch a demo
[![Zeno’s Music Box Demo](https://img.youtube.com/vi/iYXWX08sTWs/0.jpg)](https://www.youtube.com/watch?v=iYXWX08sTWs)

###Want to add your own samples?
Let's imagine that you have 71 WAV’s you want to input. 
- Rename the WAV’s to be numbered sequentially.
  - *`Example_1.wav, Example_2.wav, Example_3.wav...`*
- Open the patch within Pure Data: *ZenosMusicBox_NilsFrahm.pd*
- Edit the ‘open’ message box with the relevant filename.
  - *Before: `open WAVs/NilsFrahm_$1.wav start`*
  - *After: `open WAVs/Example_$1.wav start`*
- Edit the ‘random’ object box to be the total number of WAV's you're inputting
  - *Before: `random 48`*
  - *After: `random 71`*
- Done! Just turn up the ‘output~’ volume and click the ‘Begin & End’ toggle to start playback.

###Credits
I’d like to give a shout out to the amazing musicians which I’ve cutup and sampled in this patch.
- Ayako Hotta-Lister - London No Yoru No Ame (Album: The Japanese Koto)
- Nils Frahm - Part II (Album: Electric Piano)
