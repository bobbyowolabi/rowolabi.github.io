---
title: Sound Basics Part 2 - Properties of Sound
description: 
comments: true
published: false
---

We now have an idea of [what sound is][part-1-what-is-sound]; namely, a disruption in a medium, such as air, that causes molecules to hit each other causing a propagation (wave) of that initial disruption to the ears of a listener.

This is a good foundation for us to build off of, but we often speak of sound in terms of:

> How loud is it?

> What are the pitches in the melody I'm hearing?

> Why does it sound like it (aka timbre)?  What is its color?

How does our molecular definition of sound relate to the basic questions above?

They are related by the physical properties of how the molecules move.

In the first [part of our series][part-1-what-is-sound], we established the need to separate the notion of hearing to the physical aspects of sound.  As we move on to discuss the physical properties of sound, we will have to continue to maintain this mindset.  The properties of how the molecules move are:

**physical measurements** <sup>[[1]](#music-and-computers)</sup>

The things we hear, such as loudness, pitches and timbre are:

**psychophysical measurements** <sup>[[1]](#music-and-computers)</sup>
<br/><sub>*measurements of our perception*</sub>

##


What are pure tones?

Pure tones don’t exist naturally but every sound in the world is the sum of a multple of pure tones at different amplitudes. [kalenzaga-shazam]

## Amplitudes
"In part 1, we established that sound is a disturbance of air molecules, or rather pressure.  A way to think about sound is as a sequence of time varying pressures" (music-and-computers)

## How Do Amplitudes 

## Amplitude vs Loudness


## Frequency
We often describe sounds as being high (Flute) or low (Tuba).  Does the pattern of varying amplitudes repeat?  If so, we are in the realm of frequency.  Frequency is how quickly does the pattern of varying pressures repeat?  (music-and-computers)

## Sine Waves
How can we describe the motion of a sound wave using precise language?  This is where math and the sine wave comes in.  For ease let’s look at the movement of an individual molecule.  When a molecule is not moving (at rest) it has an initial pressure of 0, also known as equilibrium [music-and-computers].  When it moves, it will go forward a certain distance, return back to equilibrium and go in the opposite direction a certain distance .  Essentially the traveled distance of the molecule is zero since the two movements cancel each other out.  This back and forth movement is called oscillation (Describe what an oscilloscope is).  

A great illustration of this movement can be seen in the same Khan Academy video:
<iframe width="560" height="315" src="https://www.youtube.com/embed/-_xZZt99MzY?start=22&end=40" frameborder="0" allowfullscreen></iframe>

If you measure the distance the molecule travels from equilibrium (forward being a positive value and backwards being a negative value) and plot it over time on a graph, you get the form of a sinewave.  The form of this graph is called the waveform [wiki-waveform].  It turns out the sine function serves as a good foundational model for technically and formally representing the movement of a soundwave.


Let’s define the components of a sine wave:

Cycle

Frequency - the number of cycles per second.  It is measured in Hertz (Hz)

Amplitude - The size of each cycle.  Remember the equilibrium we spoke of?  This is the distance of the wave from equilibrium. - related to loudness

Wavelength

Distance Traveled Through Medium/Period


We’ll talk more about the ear later in our exploration, but it is these characteristics of a soundwave that our ears take as input to produce sound for us [kalenzaga-shazam].  Human ears can hear pure tones from 20 Hz to 20,000 Hz [kalenzaga-shazam].

### Sine Waves in Practice

We know that the sine wave is useful for modeling the motion of a soundwave, but does a single sine wave map directly to a sound?  No, a single sine wave is not a sound that actually exists, but it an artificial one [kalenzaga-shazam][wiki-pure-tones].  


Here is an example of what sine waves sound like:

<Ge Wang’s TED where he writes a CHUCK script to play random sound waves>


We call the sound associated with a single sine wave a “pure tone”.  This wave consists on one frequency [wiki-pure-tones].  If the sound associated with a sine wave does not actually exist in practice, what is the sine wave important in modeling sound?  Every sound can be represented as the sum of many pure tones at different amplitudes [wiki-pure-tones].  This insight seems to be related to the Fourier theorem.  

[part-1-what-is-sound]: {{ site.baseurl }}{% link _posts/2017-10-31-sound-basics-part-1-what-is-sound.md %}


[music-and-computers]: http://cmc.music.columbia.edu/MusicAndComputers/


## Music Theory
[kalenzaga-shazam]
http://www.smackmypitchup.com/smpu/?sec=content&id=31&topid=123
http://www.silcom.com/~aludwig/Phase_audibility.htm


## Links
http://teropa.info/blog/2016/08/19/what-is-the-web-audio-api.html
http://cmc.music.columbia.edu/MusicAndComputers/

https://books.google.com/books/about/Audio_Effects.html?id=mlHSBQAAQBAJ&printsec=frontcover&source=kp_read_button#v=onepage&q&f=false

http://www.smackmypitchup.com/smpu/?sec=content&id=31&topid=123

http://www.passmyexams.co.uk/GCSE/physics/sound-waves.html

http://www.silcom.com/~aludwig/musicand.htm

http://www.acs.psu.edu/drussell/demos.html

https://www.chirp.io/

What is Audio Programming? An Introduction

The Audio Programmer on the ADC

Audio Programming for Beginners Tutorial 00- Analog to Digital Conversion, Sample Rate & Bit Depth

http://exploresound.org/explore-sound-home/what-is-acoustics/terms-definitions/

http://teropa.info/blog/2016/08/04/sine-waves.html

Frequencies & sound explained #1 - Basic sound theory

Sound Properties (Amplitude, Period, Frequency, Wavelength) | Physics | Khan Academy
Great Explanation, actually talks about how the air molecules move

How Digital Audio Works - Computerphile

http://jackschaedler.github.io/circles-sines-signals/


### References

[<a name="music-and-computers">1</a>]
Burk, Phil, et al. “Chapter 1: The Digital Representation of Sound, Part One: Sound and Timbre; Section 1.2: Amplitude and Loudness?” [Music and computers: a theoretical and historical approach][music-and-computers], Self-Published Online. 2011. Accessed 29 Nov. 2017.
> **Authors**<br/>
> Phil Burk, SoftSynth.com<br/>
> Larry Polansky, Department of Music, Dartmouth College<br/>
> Douglas Repetto, Computer Music Center, Columbia University<br/>
> Mary Roberts<br/>
> Dan Rockmore, Department of Mathematics, Dartmouth College<br/>

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




