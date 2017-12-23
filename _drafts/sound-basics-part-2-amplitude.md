---
title: Sound Basics Part 2 - Amplitude
description: null
comments: true
published: true
---

We now have an idea of [what is sound][part-1-what-is-sound]; namely, a disruption in a medium, such as air, that causes molecules to hit each other causing a propagation (wave) of that initial disruption to the ears of a listener.

This is a good foundation for us to build off of, but we usually do not speak of sound like this.  We speak of sound in terms of:

> How loud is it?

> What are the pitches in the melody I'm hearing?

> What is its timbre <sup>[[X]](#what-is-timbre)</sup>?

How does our molecular definition of sound relate to the basic questions above?  

**They are related by the physical properties of how the molecules move.**

In the first [part of our series][part-1-what-is-sound], we established the need to separate the notion of hearing from the physical aspects of sound.  As we move on to discuss the physical properties of sound, we will have to continue to maintain this mindset.  The properties of how the molecules move are:

**physical measurements** <sup>[[1]](#music-and-computers)</sup>

The things we hear, such as loudness, pitches and timbre are:

**psychophysical measurements** <sup>[[1]](#music-and-computers)</sup>
<br/><sub>*measurements of our perception*</sub>

We will discuss both physical and psychophysical measurements.

## From Air Molecules to Sine Waves
It's likely you have seen a variation of the following image in reference to sound:

<img src="https://upload.wikimedia.org/wikipedia/commons/0/02/Simple_sine_wave.svg" width="560" height="315">

We know that sound travels in a wave.  The air molecules move back and forth and collide with neighboring air molecules transferring the energy of the initial isrupution on to the ears of a listener.
But how does this common picture of sound relate to how sound actually moves?

[Professor Dan Russell's][professor-russell] animation is a good illustration of this <sup>[[X]](#russell-particle-motion)</sup>:

<img src="http://www.acs.psu.edu/drussell/Demos/waves/Lwave-Red-2.gif" width="600" alt="animation showing particle motion for a longitudinal pressure wave highlighting the difference between particle motion and wave propagation.">

Another good illustration of this would be a slinky <sup>[[X]](#russell-slinky)</sup>:
<iframe width="560" height="315" src="https://www.youtube.com/embed/y7qS6SyyrFU?start=16&end=21" frameborder="0" allowfullscreen></iframe>



There are different kinds of waves.  There are two of particular distinction.


## Pure Tones
What are pure tones?

Pure tones don’t exist naturally but every sound in the world is the sum of a multple of pure tones at different amplitudes. [kalenzaga-shazam]

### Sine Waves in Practice (Pure Tones)

We know that the sine wave is useful for modeling the motion of a soundwave, but does a single sine wave map directly to a sound?  No, a single sine wave is not a sound that actually exists, but it an artificial one [kalenzaga-shazam][wiki-pure-tones].  


Here is an example of what sine waves sound like:

<Ge Wang’s TED where he writes a CHUCK script to play random sound waves>


We call the sound associated with a single sine wave a “pure tone”.  This wave consists on one frequency [wiki-pure-tones].  If the sound associated with a sine wave does not actually exist in practice, what is the sine wave important in modeling sound?  Every sound can be represented as the sum of many pure tones at different amplitudes [wiki-pure-tones].  This insight seems to be related to the Fourier theorem.  

## Amplitudes
"In part 1, we established that sound is a disturbance of air molecules, or rather pressure.  A way to think about sound is as a sequence of time varying pressures" (music-and-computers)

Amplitude - The size of each cycle.  Remember the equilibrium we spoke of?  This is the distance of the wave from equilibrium. - related to loudness

## Sine Waves
How can we describe the motion of a sound wave using precise language?  This is where math and the sine wave comes in.  For ease let’s look at the movement of an individual molecule.  When a molecule is not moving (at rest) it has an initial pressure of 0, also known as equilibrium [music-and-computers].  When it moves, it will go forward a certain distance, return back to equilibrium and go in the opposite direction a certain distance .  Essentially the traveled distance of the molecule is zero since the two movements cancel each other out.  This back and forth movement is called oscillation (Describe what an oscilloscope is).  

A great illustration of this movement can be seen in the same Khan Academy video:
<iframe width="560" height="315" src="https://www.youtube.com/embed/-_xZZt99MzY?start=22&end=40" frameborder="0" allowfullscreen></iframe>

If you measure the distance the molecule travels from equilibrium (forward being a positive value and backwards being a negative value) and plot it over time on a graph, you get the form of a sinewave.  The form of this graph is called the waveform [wiki-waveform].  It turns out the sine function serves as a good foundational model for technically and formally representing the movement of a soundwave.

[cook-adruino-music]: https://www.safaribooksonline.com/library/view/arduino-music-and/9781484217214/9781484217207_Ch10.xhtml
[hass-amplitude]: http://www.indiana.edu/%7Eemusic/etext/acoustics/chapter1_amplitude.shtml
[hass-sound]: http://www.indiana.edu/%7Eemusic/etext/acoustics/chapter1_sound2.shtml
[hewitt-music]: https://www.safaribooksonline.com/library/view/music-theory-for/30000LTI00240/30000LTI00240_ch01lev1sec4.html
[jos-why-sinusoids]: https://ccrma.stanford.edu/~jos/mdft/Why_Sinusoids_Important.html
[kalenzaga-shazam]: http://coding-geek.com/how-shazam-works/
[music-and-computers]: http://cmc.music.columbia.edu/MusicAndComputers/
[part-1-what-is-sound]: {{ site.baseurl }}{% link _posts/2017-10-31-sound-basics-part-1-what-is-sound.md %}
[parviainen-amplitude]: http://teropa.info/blog/2016/08/30/amplitude-and-loudness.html
[professor-russell]: http://www.acs.psu.edu/drussell/
[schaedler-sound]: https://jackschaedler.github.io/circles-sines-signals/sound.html
[russell-slinky]: https://www.youtube.com/watch?v=y7qS6SyyrFU	
[nave-transverse-waves]: http://hyperphysics.phy-astr.gsu.edu/hbase/Sound/tralon.html#c1  
[omegatron]: https://commons.wikimedia.org/wiki/User:Omegatron
[omegatron-sine-wave]: https://upload.wikimedia.org/wikipedia/commons/0/02/Simple_sine_wave.svg

### Notes
[<a name="what-is-timbre">a</a>] Imagine a note is played on both a guitar and piano ... can you differeientate the instruments based on the sound even though the notes are the same?  Sure you can, that is because their timbre is different.  The timbre of the sound is its quality, the thing that makes it different from other sounds <sup>[[X]](#cook-adruino-music)</sup>.  


We need a way of understanding how these amplitudes, which are a physical measurement (like frequency), correspond to our perception of loudness, which is a psychophysical
[music-and-computers]

frequency and amplitude are not independent; they both contribute to our perception of loudness.
The relationship is described by something called the Fletcher-Munson curves
[music-and-computers]

amplitude and intensity are one component that contribute to loudness, in the next part of our series, we will introduce another physical property that contributes to sound.
[music-and-computers]

Physical Measurement			Psychoacoustic Measurement
Amplitude*		-> Intensity**	Loudness***

* How much something vibrates
** How much the medium is displaced
*** How loud we perceive it (affected by pitch and timbre)

frequency*						Pitch**

* How fast something vibrates
** How high or low we perceive it
[music-and-computers]

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

[<a name="russell-particle-motion">X</a>] Russell, Daniel. "Longitudinal Waves". Acoustics and Vibration Animations; Section: Longitudinal and Transverse Wave Motion. 26, August 1998. Animations Updated 5 August 2016. HTML Code Modified 18 March 2014. Accessed 20 October 2017.
> **License**  <br/>
> This work by [Dan Russell](http://www.acs.psu.edu/drussell/demos.html) is licensed under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License](http://creativecommons.org/licenses/by-nc-nd/4.0/).
Based on a work at http://www.acs.psu.edu/drussell/demos.html.

[<a name="kalenzaga-shazam">X</a>] Kalenzaga, Christophe. [“How does Shazam work.”][kalenzaga-shazam] Blog post. Coding Geek: A blog about IT, programming and Java. 23 May 2015. Accessed 28 September 2017.

[<a name="parviainen-amplitude">X</a>] Parviainen, Tero. ["Learn Web Audio from the Ground Up, Part 3: Controlling Amplitude and Loudness"][parviainen-amplitude] Blog. Tero Parviainen. 30 August 2016. Web. 12 December 2017.

[<a name="jos-why-sinusoids">X</a>] Smith, J.O. ["Why Sinusoids are Important."][jos-why-sinusoids] Under Section "Sinusoids and Exponentials: Sinusoids". In Mathematics of the Discrete Fourier Transform (DFT) with Audio Applications, Second Edition. Online Book; 2007 Edition. Accessed 12 Decemeber 2017.

[<a name="schaedler-sound">X</a>] Schaedler, Jack. ["Sound."][schaedler-sound] circles-sines-signals: A Compact Primer On Digital Signal Processing. 7 September 2017. Accessed 12 December 2017.

[<a name="hewitt-music">X</a>] Hewitt, Michael. [Music Theory for Computer Musicians][hewitt-music]. Boston, MA: Course Technology, CENGAGE Learning, 2008. Apr. 2008. Web. 12 Dec. 2017.

[<a name="hass-amplitude">X</a>] Hass, Jeffrey. ["Amplitude."][hass-amplitude] Introduction to Computer Music: Volume One. 2013. Accessed 12 December 2017.

[<a name="hass-sound">X</a>] Hass, Jeffrey. ["Chapter One: An Acoustics Primer 2. What is Sound?"][hass-sound] Introduction to Computer Music: Volume One. 2013. Accessed 13 December 2017.

[<a name="russell-slinky">X</a>] Russell, Daniel. [“Longitudinal Wave Propagation on a Slinky.”][russell-slinky] YouTube. 29 September 2012.

[<a name="nave-transverse-waves">X</a>]  Nave, Carl R. ["Transverse Waves."][nave-transverse-waves] HyperPhysics. 9 November 2016. Accessed 13 December 2017.

[<a name="omegatron-sine-wave">X</a>]  [Omegatron][omegatron]. ["File:Simple sine wave.svg."][omegatron-sine-wave] Wikimedia Commons, the free media repository. 12 Jan 2015. Accessed 22 Dec 2017. 