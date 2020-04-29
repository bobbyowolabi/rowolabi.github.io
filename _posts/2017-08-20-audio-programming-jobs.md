---
title: Audio Programming Jobs
description: In this post, I look at 151 job postings of positions related to the field of audio with an emphasis on software engineering. 
comments: true
permalink: /:title
---

I've been thinking a lot about the field of audio and its prospects as a software engineer.

I've read a big chunk of [So Good They Can't Ignore You][so-good-they-cant-ignore-you] by Cal Newport and I've taken away that for the vast majority of people, becoming highly skilled at something comes before passion.  We often try to find our passion first and then pursue it; however, when you examine passionate, successful people, it's often the case that their passion (and subsequent desirable lifestyle) came after investing in becoming a "craftsmen" in their field.  They built upon acquired career capital instead of starting from scratch in a new field.

I've read a big chunk of [Soft Skills: The software developer's life manual][soft-skills-sonmez] by John Sonmez and one of the things I've taken away is that [a software engineer needs to specialize][generalists-specialists].

What do you call a software engineer that works in audio?  An audio programmer?  An audio software engineer?  How about an audio digital signal processing (DSP) engineer?

What domains do such individuals work in? Music? Speech? Communications?  Academia?  Gaming?

Is it possible to live anywhere and do this work?  Can you work remotely?  Can you consult?

What technologies and concepts should one study?  [[1]](#1-note)  I admire the work and business that the folks of [AudioKit][audio-kit] are creating for themselves.  That could be a good place to start.  They recently wrote of [some project ideas][audio-kit-projects] that new folks can pursue.  I recently purchased [The Scientist and Engineer's Guide to Digital Signal Processing][dsp-guide-amazon] by Dr. Steven W. Smith.  It is [available online for free][dsp-guide-site].  I got excited after skimming through it because it was written in a very approachable way.  Should one start there?  What about taking the Stanford's [MOOC][mooc] course [Audio Signal Processing for Music Applications][audio-signal-processing-course].  Or how about the course [Physics-based Sound Synthesis for Games and Interactive Systems][physics-sound-synthesis-course]?

One way to start to answer these questions is to look at what the market says through job postings.  As Patrick McKenzie stated, most jobs actually aren't posted and most positions aren't filled through job postings [[2]](#2-note).  Nevertheless, analyzing the public record of the market can provide valuable insight.

### Research

I manually went through [{{ site.data.audio-jobs | size }} job postings](#data).  Below are my findings:


#### Frequency of Words in Titles
{% assign min_title_frequency = 4 %}
The following words appeared in the title of job postings at least {{ min_title_frequency }} times.
<canvas id="title-token-frequencies"></canvas>

#### Locations
<iframe src="https://www.google.com/maps/d/embed?mid=15iWFbSMQD8Xs7caPrpaQ1HBpyLI" width="100%" height="480"></iframe>

<br/>
The following are the top six locations by number of job postings:
1. California, USA - 49
1. Washington, USA - 21
1. Massachusetts, USA - 21
1. United Kingdom - 12
1. Michigan, USA - 6
1. India - 6


#### Industries
The analysis of the job postings by industry was somewhat subjective.  I determined a position's industry by looking at the company's listed [industry][wikipedia-industries] on it's wikipedia page.  I also considered focus areas in the job posting's description.

<canvas id="industries-chart"></canvas>

#### Education - Degree
<canvas id="education-chart"></canvas>

#### Education - Field
<canvas id="education-field-chart"></canvas>

#### Languages
<canvas id="languages-chart"></canvas>

#### Top 6 Audio Related Skills by Number of Postings:
1. DSP - 106
1. Speech - 48
1. Audio Formats (Transcoding, Codecs) - 41
1. Transducers (Microphones, Speakers, etc) - 40
1. Real-time Concepts - 35
1. Sound Design, Sound Engineering, Acoustics - 34

#### Top 8 DSP Related Skills by Number of Postings:
1. Noise - 30
1. Echo Control - 22
1. Filtering - 21 
1. Sound Effects - 12
1. Reverb - 12
1. Equalization - 9
1. Fixed Point; Floating Point - 9
1. Compression - 8




[audio-kit]: http://audiokit.io/
[audio-kit-projects]: http://audiokitpro.com/project-ideas/
[audio-signal-processing-course]: http://online.stanford.edu/course/audio-signal-processing-music-applications-0
[dont-call-yourself-a-programmer-patio11]: http://www.kalzumeus.com/2011/10/28/dont-call-yourself-a-programmer/
[dsp-guide-amazon]: https://www.amazon.com/Scientist-Engineers-Digital-Signal-Processing/dp/0966017633
[dsp-guide-site]: http://www.dspguide.com/
[finding-great-developers]: https://www.joelonsoftware.com/2006/09/06/finding-great-developers-2/
[mooc]: https://en.wikipedia.org/wiki/Massive_open_online_course
[physics-sound-synthesis-course]: http://online.stanford.edu/course/physics-based-sound-synthesis-games-and-interactive-systems-0
[so-good-they-cant-ignore-you]: https://www.amazon.com/dp/1455509124
[soft-skills-sonmez]: https://www.amazon.com/Soft-Skills-software-developers-manual/dp/1617292397
[generalists-specialists]: https://simpleprogrammer.com/2017/06/19/generalists-specialists/
[wikipedia-industries]: https://en.wikipedia.org/wiki/Category:Industries
   
### Notes
[<a name="1-note">1</a>] At first glance, asking this question appears to go against the mindset of striving to be an excellent engineer not bound by a stack.  Patrick Mckenzie makes the claim that one is "... not defined by your chosen software stack".  He says that "If a Python shop was looking for somebody technical to make them a pile of money, the fact that I’ve never written a line of Python would not get held against me."  Talented engineers are rare — vastly rarer than opportunities to use them — and it is a seller’s market for talent right now in almost every facet of the field.  Everybody at Matasano uses Ruby.  If you don’t, but are a good engineer, they’ll hire you anyway.  (A good engineer has a track record of — repeat after me — increasing revenue or decreasing costs.)  Much of Fog Creek uses the Microsoft Stack.  I can’t even spell ASP.NET and they’d still hire me. [[A]](#A-citation)

I think what Mckenzie is saying makes sense.  I don't think my original question "What technologies and concepts should one study?" is in contradiction to his sentiment.  Part of the reason to specialize (thus learning a stack or domain) is in order to market yourself [[B]](#B-citation).  How will people know that you are an excellent engineer?  Specialization helps one market themselves and expand their network.  My theory is when your reputation is established in the community, then it will likely be eaiser to be in a situation where you are hired to work on technologies you aren't familiar with as Mckenzie expresses.

[<a name="2-note">2</a>] McKenzie wrote, '"Read ad.  Send in resume.  Go to job interview.  Receive offer." is the exception, not the typical case, for getting employment: Most jobs are never available publicly, just like most worthwhile candidates are not available publicly [(see here)][finding-great-developers] ...' [[A]](#A-citation)

[<a name="A-citation">A</a>] McKenzie, Patrick. [Don't Call Yourself A Programmer, And Other Career Advice][dont-call-yourself-a-programmer-patio11]. Blog. Kalzumeus Software Blog. Publish 29 October 29 2011. Web. 28 July 2017.

[<a name="B-citation">B</a>] Sonmez, John. [Should Software Developers Be Generalists or Specialists?
][generalists-specialists]. Blog. Simple Programmer. Publish 19 June 2017. Web. 13 August 2017.


### Data
<table>
   <tr>
      <th>Title</th>
      <th>Company</th>
      <th>Location</th>
   </tr>
   {% for job in site.data.audio-jobs %}
      <tr>
         <td><a href="{{ job.URL }}">{{ job.Title }}</a></td>
         <td>{{ job.Company }}</td>
         <td>{{ job.Location }}</td>
      </tr>
   {% endfor %}
</table>

<script src="js/Chart.bundle.min.js"></script>
{% for job in site.data.audio-jobs %}
   {% assign title = job.Title | replace: ",", " " | replace: ")", " " | replace: "(", " " | replace: "/", " " | downcase | split: " " | join: ", " %}
   {% if forloop.first == false %}
      {% assign title_tokens = title_tokens | append: ", " %}
   {% endif %}
   {% assign title_tokens = title_tokens | append: title %}
{% endfor %}

{% assign title_tokens = title_tokens | split: ", " | sort %}
{% for title_token in title_tokens %}
   {% if current_token == title_token %}
      {% assign count = count | plus: 1 %}
   {% else %}
      {% if current_token != "" and current_token.size > 1 and count > min_title_frequency %}
         {% assign labels = labels | append: '"' | append: current_token | append: '" ' %}
         {% assign data = data | append: count | append: " " %}
      {% endif %}      
      {% assign current_token = title_token %}
      {% assign count = 1 %}
   {% endif %}   
{% endfor %}

<script>
   var ctx = document.getElementById('title-token-frequencies').getContext('2d');
   var titleChart = new Chart(ctx, {
       type: 'bar',
       data: {
           labels: [ {{ labels | split: " " | join: ", " }} ],
           datasets: [{
               label: "Job Titles",
               backgroundColor: 'rgb(255, 99, 132)',
               borderColor: 'rgb(255, 99, 132)',
               data: [ {{ data | split: " " | join: ", " }} ],
           }]
       },
       options: {}
   });

   ctx = document.getElementById('industries-chart').getContext('2d');
   var titleChart = new Chart(ctx, {
       type: 'horizontalBar',
       data: {
           labels: [ "Games", "Music", "Communications", "Electronics", "Broadcast Media", "Mobile", "Health", "Social Networking", "Artificial Intelligence", "Voice / Speech", "Online Shopping", "Research & Development", "Audio Technology", "Semiconductors", "Home Automation", "Virtual Reality", "Internet", "Computer Hardware", "Computer Software", "Automotive", "Education", "Client Services" ],
           datasets: [{
               label: "Positions",
               backgroundColor: 'rgb(255, 99, 132)',
               borderColor: 'rgb(255, 99, 132)',
               data: [18, 25, 28, 69, 4, 13, 2, 2, 1, 21, 8, 23, 42, 36, 1, 11, 9, 43, 42, 4, 2, 2],
           }]
       },
       options: {}
   });   

   ctx = document.getElementById('languages-chart').getContext('2d');
   var titleChart = new Chart(ctx, {
       type: 'horizontalBar',
       data: {
           labels: [ "C", "C++", "Matlab", "Python", "C#", "Java", "Swift", "Objective-C", "Assembly", "HTML", "CSS3", "Javascript", "Go", "Perl", "Tcl", "TensorFlow", "Torch", "Octave", "Verilog", "Ruby", "Shell Scripting", "VB" ],
           datasets: [{
               label: "Positions",
               backgroundColor: 'rgb(255, 99, 132)',
               borderColor: 'rgb(255, 99, 132)',
               data: [94, 91, 48, 37, 11, 15, 3, 9, 18, 1, 2, 4, 1, 7, 2, 5, 1, 2, 2, 2, 1, 1],
           }]
       },
       options: {}
   });

   ctx = document.getElementById('education-chart').getContext('2d');
   var titleChart = new Chart(ctx, {
       type: 'bar',
       data: {
           labels: [ "Bachelors", "Masters", "PhD", "Postdoctoral", "Equivalent Experience"],
           datasets: [{
               label: "Positions",
               backgroundColor: [ 
                'rgb(255, 99, 132)',
                'rgb(201, 203, 207)',
                'rgb(255, 159, 64)',
                'rgb(255, 205, 86)',
                'rgb(75, 192, 192)'],
               borderColor: 'rgb(255, 99, 132)',
               data: [84, 89, 37, 3, 25],
           }]
       },
       options: {}
   });
   ctx = document.getElementById('education-field-chart').getContext('2d');
   var titleChart = new Chart(ctx, {
       type: 'horizontalBar',
       data: {
           labels: [ "Computer Science", "Electrical Engineering", "Computer Engineering", "Engineering", "Related Field", "Mathematics", "Physics", "Digital Audio Signal Processing", "Software Engineering", "Music Technology", "Acoustics", "Statistics", "Audio Engineering", "Business", "Mechanical Engineering", "Electronic Engineering"],
           datasets: [{
               label: "Positions",
               backgroundColor: 'rgb(255, 99, 132)',
               borderColor: 'rgb(255, 99, 132)',
               data: [82, 65, 27, 15, 46, 9, 15, 17, 3, 1, 15, 1, 5, 2, 5, 4],
           }]
       },
       options: {}
   });
</script>
