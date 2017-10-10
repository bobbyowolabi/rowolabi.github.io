---
title: Sound Basics Part 1 - What is Sound?
description: The first part of a series exploration sound. 
comments: true
---

A lot of times when sound is described, a graph of a sound wave is shown.  The term analog may pop up.  The sine function is discussed … wasn’t that about angles of a triangle?  We are told sound is simply changes in pressure.  This all is somehow represented in digital form as 0s and 1s.  What does all of this mean?  How can looking at a sine graph help me understand and describe the sound of a saxophone versus a laughing baby?  I want to present these concepts through the eyes of a true beginner.  I hope to achieve this by asking questions of a beginner.

### What is Sound?

In attempting to understand sound, it’s important to separate ourselves from the experience of hearing because it is different from what sound is at it’s core.  Our hearing of sound is merely an interpretation our body performs for us of a specific kind of physical event.  We often call these physical events signals.  At a high level, the following occurs [wiki-perception]:
1. Our ears receive information (signals)
1. Our body interprets this information (our nervous system) 
1. Our senses are stimulated (we hear it via our sensory system)

*What are the signals our ears received?*

*How is it that we “hear” this information?*

*["If a tree falls in a forest and no one is around to hear it, does it make a sound?"](https://en.wikipedia.org/wiki/If_a_tree_falls_in_a_forest)*

I hope that through our exploration of this topic, we’ll be able to provide more insight into the questions above.

### What Comprises Sound?
Sound Involves Three Actors [music-and-computers]:
1. An Object
1. Medium
1. Listener

At its core, this boils down to physics and perception [music-and-computers].  The first two things, an object & medium are where the physics occurs; the listener is where the perception occurs [music-and-computers]. 

The Interaction of the Actors Produces Sound [music-and-computers]:
The Movement of an Object
The Transmission of the Result of the Movement Through a Medium
A Listener Perceives the Transmission of the Movement as Sound

“All things that make sound move, and in some very metaphysical sense, all things that move (if they don’t move too slowly or too quickly) make sound.” [music-and-computers]

### The Production of Sound
#### What is the result of the movement that we are hearing?
Before diving right into the result of the movement, let’s start at the molecular level and work our way back up.

There are 3 different phases of matter: solids, liquids and gases.  Matter, for the purposes of our discussion, is made up atoms that bond together to form molecules.  Solids have their molecules tightly packed together.  They keep their shape and not much gets through them.  Liquids have their molecules spaced further apart.  Things can move through them but there is some resistance.  Then we have gases.  Gases have molecules that are relatively far apart.  Objects, including us, can easily move through this medium [thompson-mike].  It is this movement that results in the production of sound.  Air is comprised of invisible gases that are all around us.  It is made up of certain molecules mainly nitrogen and oxygen.

Let’s get back to our original question, what is this “result of the movement” that we are hearing?  Focusing on the medium of air, the result of the movement we hear are air molecules hitting each other.  But what does this mean?  If I am sitting listening to the sound of a ball being kicked during a game, the fact that molecules are hitting each other as a result of the kick doesn’t aid in understanding this phenomenon.  How do these air molecules hitting each other arrive to my ear so I can perceive it as sound?   How is it that two listeners can hear the same sound when situated in opposite directions of the object?  Do these air molecules go around and visit each listener?

The following is a clip from the Khan Academy and gives a good illustration of how the air molecules interact when sound is produced:

<iframe width="560" height="315" src="https://www.youtube.com/embed/-_xZZt99MzY?start=07&end=13" frameborder="0" allowfullscreen></iframe>

As an object moves, it pushes and pulls at the surrounding air thus causing the air molecules to indeed hit each other, producing something called pressure.  The physical act of the molecules hitting each other is not pressure, but rather, the force that is exerted when they collide with themselves and other objects is what we call pressure.  [ucar-what-is-air]  

As seen in the video, this disturbance [Waters] in the air causes the molecules move back and forth and hit other molecules that move back and forth causing a transmission of the initial pressure through the air to arrive to the ears of a listener.  This forwards and backwards movement towards a listener’s ear is described as a wave [computerphile-digital-audio].

<Talk about vibration, propagation>

Listen to David Domminney Fowler describe this motion: link (0 - 14/15 seconds)
### Waves
#### Sound Waves
The physical act of pressure being transmitted through the air produces a “wave” referred to as a soundwave.  The molecules themselves don’t actually travel with the sound [wiki-sound] but merely transport it a short distance to a neighboring molecule.  It’s this transport at a higher level in terms of groups of molecules that comprise the physical phenomenon of a wave.

#### Sine Waves
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

##### Sine Waves in Practice
We know that the sine wave is useful for modeling the motion of a soundwave, but does a single sine wave map directly to a sound?  No, a single sine wave is not a sound that actually exists, but it an artificial one [kalenzaga-shazam][wiki-pure-tones].  

Here is an example of what sine waves sound like:
<Ge Wang’s TED where he writes a CHUCK script to play random sound waves>

We call the sound associated with a single sine wave a “pure tone”.  This wave consists on one frequency [wiki-pure-tones].  If the sound associated with a sine wave does not actually exist in practice, what is the sine wave important in modeling sound?  Every sound can be represented as the sum of many pure tones at different amplitudes [wiki-pure-tones].  This insight seems to be related to the Fourier theorem.  

### Conclusion
There are different physical signals around us, one of them is sound.  It is a vibration that propagates through a medium and can be decrypted by our ears.  Light is also a vibration, but we can’t hear it because our ears weren’t designed to do so.  Our eyes were designed to interpret that vibration [kalenzaga-shazam].  Human ears can hear pure tones from 20 Hz to 20,000 Hz [kalenzaga-shazam], while light is composed of sine waves from 4 x 10^14 Hz to 7.9 10^14 Hz.
Are there mediums that cannot transmit waves?
Yes, in space.

<Talk about releasing early> - masters of scale

### References
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

