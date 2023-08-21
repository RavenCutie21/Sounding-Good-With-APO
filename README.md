# Sounding Good With APO for free

For this we will obviously need [Equalizer APO](https://sourceforge.net/projects/equalizerapo/) we will also need three free plugins. Two of which are from a bundle, [REAPLUGS](https://www.reaper.fm/reaplugs/) for ReaEQ and ReaComp, and you will get an expander I use [ATKEXPANDER](https://www.kvraudio.com/product/atkexpander-by-matthieu-brucher), yes I know it's an older version but in my opinion it's better.

When installing your plugins if you want to use my preset, please put them in the Equalizer APO Plugin Folder. 

C:\Program Files\EqualizerAPO\VSTPlugins

-------------------------

In Equalizer APO you make a chain after installing to your mic, the chain will be as follows,

- DEVICE (your mic)
- PREAMP (for gainstaging, this is just a very basic version of it, I use +12db as my mic volume is low in Windows ie 35 for already reduced background noise but i also am within 4inches of my microphone)
- ReaEQ (this is where you would EQ your voice, every voice is different so I won't explain what to do. please find a video for this.) Do not cut out the mids here please, as every voice needs this section otherwise you'll be drowned out in the background. 
- ATK EXPANDER, (this we will have specific settings to get rid of as much or all of the background noise as possible without having our audio clip, ATTACK or the first dial make it around 5ms, Release or the second dial make it around 40-60ms, the third dial is what you play with last but what you do is you start from the lowest it can be aka right most side of the dial, and SLOWLY raise it up while monitoring your mic in say OBS, until the moment all background noise vanishes but if it clips your voice lower it so there is some as itll almost fully vanish in a moment, the fourth and fifth dials are all the way maxed.)
- ReaComp (compressor the most common settings for one are as follows, attack 3-5ms, release 100-250ms, ratio 4:1, threshhold -22db all the way to -16db, you do not need to touch anything else for this)
- PREAMP (this time we use negative db values, start with -12, if you are slightly too quiet slowly raise it back up in 0.50db increments, in OBS I aim for -12db on normal speaking, and having a negative value in this will also remove a ton of background noise, you can technically put the ATK expander after this, but this is just how I do it.)

Now if you really want to get rid of the final bit of background noise if you even have any, you can add reafir_standalone or any other noise removal plugin you can find, change the mode to subtract, and pull both dots all the way down to -90db. you shouldnt need to do this at all but it's just here incase your background noise was that bad.

If you are lazy you can skip the ATK expander and reafir, and use an AI based Noise Suppression at the end of your chain, either [Werman's RN Noise removal](https://github.com/werman/noise-suppression-for-voice) or [Goyo's AI Voice Seperator](https://goyo.app/) (really heavy but sounds the cleanest).

There will be an example preset (without any eq done, and without the atk threshhold being set) that you can download 

[HERE](https://github.com/YunaOneeChan/Sounding-Good-With-APO/blob/main/config.txt)
