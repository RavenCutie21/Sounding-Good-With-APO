# Sounding Good With APO for free

This transfers to any DAW, such as FL Studio, Ableton Live, or even Ardour, you do not need to use what I have listed.

For this we will obviously need [Equalizer APO](https://sourceforge.net/projects/equalizerapo/) we will also need three free plugins. Two of which are from a bundle, [REAPLUGS](https://www.reaper.fm/reaplugs/) for ReaEQ and ReaComp, and you will get an expander I use [ATKEXPANDER](https://www.kvraudio.com/product/atkexpander-by-matthieu-brucher), yes I know it's an older version but in my opinion it's better.

Better EQ and compressor than the one in reaplugs, EQ being [TDR Nova](https://www.tokyodawn.net/tdr-nova/), Compressor being [TDR Kotelnikov](https://www.tokyodawn.net/tdr-kotelnikov/)

Compressor settings, copy everything and right click in the plugin itself and press paste preset.
* <TDRKotelnikovGE thresholdParam="-25.0" peakCrestParam="3.0" softKneeParam="2.0" ratioParam="2.0" attackParam="7.0" releasePeakParam="50" releaseRMSParam="180" makeUpParam="0.0" dryMixParam="off" outGainParam="4.0" keyHPFrequencyParam="210" keyHPSlopeParam="3.0" keyStereoDiffParam="60" keyStereoBalanceParam="Center" fdrVisibleParam="Off" fdrActiveParam="On" fdrTypeParam="Bell A" fdrFrequencyParam="1300" fdrAmountParam="60" yingParam="Off" yangParam="Off" deltaParam="Off" bypassParam="Off" equalLoudParam="Off" qualityParam="Precise" modeParam="Stereo" grDispScaleParam="2" grDispModeParam="Gain Reduction"

you'll have to add "/>" at the end, so paste it somewhere else

When installing your plugins if you want to use my preset, please put them in the Equalizer APO Plugin Folder. 

C:\Program Files\EqualizerAPO\VSTPlugins

---------------------------------------------------------------

In Equalizer APO you make a chain after installing to your mic, the chain will be as follows,

* DEVICE (your mic)
* PREAMP (for gainstaging, this is just a very basic version of it, I use +12db as my mic volume is low in Windows ie 35 for already reduced background noise but i also am within 4inches of my microphone, check in OBS do not have your PEAK over -6db, ideally aim for -12db as this is perfect for doing any processing as it will add or remove more volume depending on what you do)
* ReaEQ (this is where you would EQ your voice, please refer to the section at the very bottom of this page.)
* ATK EXPANDER, (this we will have specific settings to get rid of as much or all of the background noise as possible without having our audio clip, ATTACK or the first dial make it around 5ms, Release or the second dial make it around 40-60ms, the third dial is what you play with last but what you do is you start from the lowest it can be aka right most side of the dial, and SLOWLY raise it up while monitoring your mic in say OBS, until the moment all background noise vanishes but if it clips your voice lower it so there is some as itll almost fully vanish in a moment, the fourth and fifth dials are all the way maxed.)
* ReaComp (compressor the most common settings for one are as follows, attack 3-5ms, release 100-250ms, ratio 4:1, threshhold -22db all the way to -16db, you do not need to touch anything else for this, just make sure your threshhold is above your normal speaking, so if your average is -20 make the compressor -18 or -16, you only want this to affect your voice when you get loud)
* PREAMP (this time we use negative db values, start with -12, if you are slightly too quiet slowly raise it back up in 0.50db increments, in OBS I aim for -14db as my loudest after all processing I test using plosive words like P's and B's, and having a negative value in this will also remove the rest of the background noise ideally, you can technically put the ATK expander after this, but this is just how I do it.)

Now if you really want to get rid of the final bit of background noise if you even have any, you can add reafir_standalone or any other noise removal plugin you can find, change the mode to subtract, and pull both dots all the way down to -90db. you shouldnt need to do this at all but it's just here incase your background noise was that bad.

If you are lazy you can skip the ATK expander and reafir, and use an AI based Noise Suppression at the end of your chain, either [Werman's RN Noise removal](https://github.com/werman/noise-suppression-for-voice) or [Goyo's AI Voice Seperator](https://goyo.app/) (really heavy but sounds the cleanest).

There will be an example preset (without any eq done, and without the atk threshhold being set) that you can download 

[HERE](https://github.com/YunaOneeChan/Sounding-Good-With-APO/blob/main/config.txt)

# The EQ Cheat Sheet and Extra Information

When actually doing the EQ process, please refer to the EQ Cheat Sheet below

![Cheat Sheet](https://github.com/YunaOneeChan/Sounding-Good-With-APO/blob/main/EQ%20Cheat%20Sheet.png)

Cutting out certain frequencies around 5kHz can make words sound crisper, or removing 200Hz can help with muting m sounds such as map or mat so that all other vowels can be heard easier. Boosting 1kHz and 3kHz will add brightness to male vocals without compromising articulation or crispness; boosting 2kHz and 4kHz will help female vocals cut through a mix. To help even out intonation across vowel types, it’s important to listen closely when choosing where to cut/boost either high or low-frequency ranges during the mixing process—for example: boosting 5 kHz for male vocals but cutting at 5 kHz for female vocals. Or vice versa. Females tend to have higher pitched voices, so you want them to cut out any frequencies below 300 Hz to prevent muddy-sounding vocals. 

------------------------------------------------------

Proximity effect, sibilance, nasal tone, brittleness, and harshness are all problems that can occur during recording. If not dealt with properly, they can ruin a vocal track. 

* Use a high-pass filter or low shelf to reduce the proximity effect. 

* Reduce Sibilance by cutting frequencies around 10kHz.*

* Reduce nasal tone by boosting frequencies around 200Hz and 3kHz. 

* Reduce brittleness by boosting frequencies between 500Hz and 8kHz. 

* Remove harshness by reducing the level of frequencies in the 5-8kHz range.

*Please note that sibilance can also be treated dynamically with a de-esser.

---------------------------------------------------

If the vocal is still lacking the sparkle you hoped for, here are 5 tips to help make it stand out.

* To fix vocal muddiness, try using a high-pass filter to remove the low end. 

* To add vocal sheen, use a boost around 4-5kHz. 

* To give vocal presence, use a shelf boost around 2-3kHz. 

* To add vocal crispness, use a boost at 10kHz. 

* Finally, to add air, use a high shelf boost at 12kHz or above.

--------------------------------------------------

You can also do these things to make your voice or vocals sound more full or warm

* Cut frequencies that cause vocal fatigue or hurt the ears (1 kHz).

* Boost frequencies that make the vocals warmer (500 Hz).

* Boost frequencies that make the vocals clearer (5 kHz).

* Add roundness with a mid boost around 500 Hz.

* Filter out frequency ranges to clear up sibilance (8 kHz).



# Headphones or IEM's

This is actually incredibly easy, please visit https://autoeq.app

This allows you to search for your headphones in a really large database and use pre-existing EQ profiles, like Harman, which is the most commonly enjoyed EQ profile, and what I would actually recommend most people to use, you can adjust it after to fix some of the stuff you wouldn't like but that's it. 

When using autoeq.app it should give you a file and tell you where to save it, you just INCLUDE its file

Just make sure your chain for your mic is saved as a seperate file and not config.txt as you will import it in a specific order

HEADPHONES > EQ PRESET > two comments of nothing > MICROPHONE > MIC CONFIG YOU MADE

You can remove the device section from my preset if you plan on getting a preset on your headphones.
