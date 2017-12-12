---
title: Sound Basics Part 2 - Properties of Sound
description: 
comments: true
published: false
---

We now have an idea of [what sound is][part-1-what-is-sound]; namely, a disruption in a medium, such as air, that causes molecules to hit each other causing a propagation (wave) of that initial disruption to the ears of a listener.

This is a good foundation for us to build off of, but we usually do not speak of sound like this.  We speak of sound in terms of:

> How loud is it?

> What are the pitches in the melody I'm hearing?

> What is its timbre <sup>[[X]](#what-is-timbre)</sup>?

How does our molecular definition of sound relate to the basic questions above?

They are related by the physical properties of how the molecules move.

In the first [part of our series][part-1-what-is-sound], we established the need to separate the notion of hearing from the physical aspects of sound.  As we move on to discuss the physical properties of sound, we will have to continue to maintain this mindset.  The properties of how the molecules move are:

**physical measurements** <sup>[[1]](#music-and-computers)</sup>

The things we hear, such as loudness, pitches and timbre are:

**psychophysical measurements** <sup>[[1]](#music-and-computers)</sup>
<br/><sub>*measurements of our perception*</sub>

## Mental Model for Sound Movement



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

[hass-amplitude]: http://www.indiana.edu/%7Eemusic/etext/acoustics/chapter1_amplitude.shtml
[jos-why-sinusoids]: https://ccrma.stanford.edu/~jos/mdft/Why_Sinusoids_Important.html
[music-and-computers]: http://cmc.music.columbia.edu/MusicAndComputers/
[part-1-what-is-sound]: {{ site.baseurl }}{% link _posts/2017-10-31-sound-basics-part-1-what-is-sound.md %}
[parviainen-amplitude]: http://teropa.info/blog/2016/08/30/amplitude-and-loudness.html
[schaedler-sound]: https://jackschaedler.github.io/circles-sines-signals/sound.html
[cook-adruino-music]: https://www.safaribooksonline.com/library/view/arduino-music-and/9781484217214/9781484217207_Ch10.xhtml
[hewitt-music]: https://www.safaribooksonline.com/library/view/music-theory-for/30000LTI00240/30000LTI00240_ch01lev1sec4.html 

### Notes
[<a name="what-is-timbre">a</a>] Imagine a note is played on both a guitar and piano ... can you differeientate the instruments based on the sound even though the notes are the same?  Sure you can, that is because their timbre is different.  The timbre of the sound is its quality, the thing that makes it different from other sounds <sup>[[X]](#cook-adruino-music)</sup>.  

### References
[<a name="music-and-computers">1</a>]
Burk, Phil, et al. “Chapter 1: The Digital Representation of Sound, Part One: Sound and Timbre; Section 1.2: Amplitude and Loudness?” [Music and computers: a theoretical and historical approach][music-and-computers], Self-Published Online. 2011. Accessed 29 Nov. 2017.
> **Authors**<br/>
> Phil Burk, SoftSynth.com<br/>
> Larry Polansky, Department of Music, Dartmouth College<br/>
> Douglas Repetto, Computer Music Center, Columbia University<br/>
> Mary Roberts<br/>
> Dan Rockmore, Department of Mathematics, Dartmouth College<br/>

[<a name="cook-adruino-music">X</a>] Cook, Mike, et al. [“CHAPTER 10 The Anatomy of a Sound.” Arduino Music and Audio Projects][cook-adruino-music], Apress, Springer Science Business Media, 2015.

[<a name="parviainen-amplitude">X</a>] Parviainen, Tero. ["Learn Web Audio from the Ground Up, Part 3: Controlling Amplitude and Loudness"][parviainen-amplitude] Blog. Tero Parviainen. 30 August 2016. Web. 12 December 2017.

[<a name="jos-why-sinusoids">X</a>] Smith, J.O. ["Why Sinusoids are Important."][jos-why-sinusoids] Under Section "Sinusoids and Exponentials: Sinusoids". In Mathematics of the Discrete Fourier Transform (DFT) with Audio Applications, Second Edition. Online Book; 2007 Edition. Accessed 12 Decemeber 2017.

[<a name="schaedler-sound">X</a>] Schaedler, Jack. ["Sound."][schaedler-sound] circles-sines-signals: A Compact Primer On Digital Signal Processing. 7 September 2017. Accessed 12 December 2017.

[<a name="hewitt-music">X</a>] Hewitt, Michael. [Music Theory for Computer Musicians][hewitt-music]. Boston, MA: Course Technology, CENGAGE Learning, 2008. Apr. 2008. Web. 12 Dec. 2017.

[<a name="hass-amplitude">X</a>] Hass, Jeffrey. ["Amplitude."][hass-amplitude] Introduction to Computer Music: Volume One. 2013. Accessed 12 December 2017.

