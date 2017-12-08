---
title: Sound Basics Part 3 - How We Hear
description: 
comments: true
published: false
---

## Hearing Sound
Our eardrums are transducers, they turn one form of information into another like microphones and speakers (music-and-computers).  

(music-and-computers)
sound waves reach our ears and vibrate eardrums
sound energy is transferred through middle ear to inner ear
cochlea is located in inner ear
it is a snail shaped organ filled with fluid and is bisected by an elastic partition called the basilar membrane which is covered with hair cells.
When sound energy reaches the cochlea, it produces fluid waves that form a series of peaks in the basilar membrane, the position and size of which depend on the frequency content of the sound.

(music-and-computers)
Different sections of the basilar membrane resonate (form peaks) at different frequencies
Front Cochlea Peaking - high frequiencies
Back Cochlea peaking - low frequencies

These peaks match up with and excite certain hair cells which send nerve impuleses to the brain via the auditory nerve. (music-and-computers)

"Our ear has a drum that moves in sympathy with these waves, and a larget array of differently sized hairs converts those vibrations into verve impulses.  We can therefore perceive a sound" (#cook-arduino-music)

image from ((music-and-computers):
http://cmc.music.columbia.edu/MusicAndComputers/images/chapter1/basilar.jpg

(music-and-computers)
The nerve pulses that are sent to the brain are interpreted as sound.
The cochlea transforms sounds from their physical, time domain (amplitude vs time) to the frequency domain (amplitude vs frequency).  The latter domain is the one our brain can understand

"basilar membrane serves as a time-to-frequency converter, in order to prepare sonic information for its eventual cognition by the higher functions of the brain." (music-and-computers)

The analysis of sound is performed by looking at its fourier transform with is a mathematical thing.  Our ears perform a similar transform with its structure [Newmarch].

Sounds heard by the ear correspond to sine waves.  Harmonics correspond to sine waves with a frequency that is a multiple of the base sine wave [Newmarch].


When you hear sound, it is vibrations of your ear drum.  What causes the vibration of your ear drum?  Air molecules hitting your eardrum cause this vibration.  When the moves object (blowing into a saxophone, piano key, leaves in the wind, guitar string plucked) the surrounding air molecules are disturbed.  What results are air molecules rushing to your eardrum that is waiting to vibrate [music-and-computers].


Air molecules must be able to travel far and wide huh?  I can hear the keys being pressed as I type these words from quite a distance away.


Amplitude is just one characteristic of sound


Frequency - the rate at which the air pressure fluctuates [music-and-computers]


Analogy for the eardrum - children jumping on a trampoline.The trampoline is the eardrum, the children are air molecules.




Transducers

## Your Eardrum as a Function

Sound can be described as a function [music-and-computers].

Input = the time elapsed since the sound was initiated.

Function = how far and in what direction your eardrum moved.

In other words, time is the input, amplitude/pressure is the output [music-and-computers].

## How Our Ears Work

Sound waves (air molecules) reach out ears, their first stop is the eardrum.

## Links
DSP Guide: Chapter 22
http://www.smackmypitchup.com/smpu/?sec=content&id=31&topid=123
http://cmc.music.columbia.edu/MusicAndComputers/
http://www.silcom.com/~aludwig/EARS.htm
http://www.silcom.com/~aludwig/Brain.htm
https://ccrma.stanford.edu/~jos/sasp/Introduction_Overview.html


## References
[<a name="cook-adruino-music">X</a>] Cook, Mike, et al. “CHAPTER 10 The Anatomy of a Sound.” Arduino Music and Audio Projects, Apress, Springer Science Business Media, 2015.

[wiki-vibration]

Wikipedia contributors. "Vibration." Wikipedia, The Free Encyclopedia. Wikipedia, The Free Encyclopedia, 24 Sep. 2017. Web. 3 Oct. 2017. 

https://en.wikipedia.org/wiki/Vibration

[smack-my-pitch-up]

Tattoni, Guido. Chapter 1.1 “what is sound?”. Smack My Pitch Up. Self-Published Online (Date Unknown). Accessed 3 October 2017. 

http://www.smackmypitchup.com/smpu/?sec=content&id=72&topid=123

This work is published under a Creative Commons License.

[wiki-perception]

Wikipedia contributors. "Perception." Wikipedia, The Free Encyclopedia. Wikipedia, The Free Encyclopedia, 25 Sep. 2017. Web. 3 Oct. 2017

https://en.wikipedia.org/wiki/Perception

[computerphile-digital-audio]

David Domminney Fowler [Computerphile]. “How Digital Audio Works - Computerphile”. 26, October 2015. Accessed. 2 October 2017.

https://www.youtube.com/watch?v=1RIA9U5oXro

[wiki-pure-tones]

Wikipedia contributors. "Musical tone." Wikipedia, The Free Encyclopedia. Wikipedia, The Free Encyclopedia, 21 May. 2017. Accessed. 2 Oct. 2017.

[wiki-waveform]

Wikipedia contributors. "Waveform." Wikipedia, The Free Encyclopedia. Wikipedia, The Free Encyclopedia, 22 Sep. 2017. Accessed. 30 Sep. 2017

[wiki-sound]

Wikipedia contributors. "Sound." Wikipedia, The Free Encyclopedia. Wikipedia, The Free Encyclopedia, 24 Sep. 2017. Web. 29 Sep. 2017. 

https://en.wikipedia.org/wiki/Sound#Physics_of_sound

[thompson-mike]

Mike Thompson [self-titled]. “Did You Ever Wonder: How Far Apart Are Air Molecules?”. 26 March 2015. Accessed 29 September 2017. Retrieved from https://www.youtube.com/watch?v=NO9F2UJ1EcY

[ucar-what-is-air]

The University Corporation for Atmospheric Research. “What is Air?”. Article.  Kids’ Crossing.  25 March 2005. Accessed 29 September 2017.

URL

https://eo.ucar.edu/kids/sky/air1.htm

[kalenzaga-shazam]

Kalenzaga, Christophe. “How does Shazam work.” Blog post. Coding Geek: A blog about IT, programming and Java. 23 May 2015. Accessed 28 September 2017.

URL

http://coding-geek.com/how-shazam-works/

[audio-programmer-beginning-tutorial]

Hodge, Joshua [The Audio Programmer]. (2017, May 22). Audio Programming for Beginners Tutorial 00- Analog to Digital Conversion, Sample Rate & Bit Depth. Retrieved from https://www.youtube.com/watch?v=Ov3GXhorrJE

[Waters]

Waters, Dan. "Intro to Audio Programming, Part 1: How Audio Data is Represented." Blog post.  Game Theory: A blog by Microsoft Academic Developer Evangelist, Dan Waters. 22 Jun. 2009. Accessed 8 Sep. 2017.

URL

https://blogs.msdn.microsoft.com/dawate/2009/06/22/intro-to-audio-programming-part-1-how-audio-data-is-represented/

[Newmarch]

Newmarch, Jan. “1. Basic Concepts of Sound.” Linux sound programming, Apress, Berkeley, CA, 2017.

[music-and-computers]

Burk, Phil, et al. “Chapter 1: The Digital Representation of Sound, Part One: Sound and Timbre; Section 1.1: What Is Sound?” Music and computers: a theoretical and historical approach, Self-Published Online. 2011. Accessed 8 Sep. 2017.

Authors

Phil Burk, SoftSynth.com

Larry Polansky, Department of Music, Dartmouth College

Douglas Repetto, Computer Music Center, Columbia University

Mary Roberts

Dan Rockmore, Department of Mathematics, Dartmouth College 

URL

http://cmc.music.columbia.edu/MusicAndComputers/



