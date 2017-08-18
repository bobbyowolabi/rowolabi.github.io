---
title: Audio Programming Jobs
description: 
comments: true
---

I've been thinking a lot about the field of audio and its prospects as a software engineer.

I've read a big chunk of [So Good They Can't Ignore][so-good-they-cant-ignore-you] by Cal Newport and I've taken away that for the vast majority of people, becoming highly skilled at something comes before passion.  We often try to find our passion first and then pursue it; however, when you examine passionate, successful people, it's often the case that their passion (and subsequent desirable lifestyle) came after investing in becoming a "craftsmen" in their field.  They built upon acquired career capital instead of starting from scratch in a new field.

I've read a big chunk of [Soft Skills: The software developer's life manual][soft-skills-sonmez] by John Sonmez and one of the things I've taken away is that [a software engineer needs to specialize][generalists-specialists].

What do you call a software engineer that works in audio?  An audio programmer?  An audio software engineer?  How about an audio digital signal processing (DSP) engineer?

What domains do such individuals work in? Music? Speech? Communications?  Academia?  Gaming?

Is it possible to live anywhere and do this work?  Can you work remotely?  Can you consult?

What technologies and concepts should one study?  [[1]](#1-note)  I admire the work and business that the folks of [AudioKit][audio-kit] are creating for themselves.  That could be a good place to start.  They recently wrote of [some project ideas][audio-kit-projects] that new folks can pursue.  I recently purchased [The Scientist and Engineer's Guide to Digital Signal Processing][dsp-guide-amazon] by Dr. Steven W. Smith.  It is [available online for free][dsp-guide-site].  I got excited after skimming through it because it was written in a very approachable way.  Should I start there?  What about taking the Stanford's [MOOC][mooc] course [Audio Signal Processing for Music Applications][audio-signal-processing-course].  Or how about the course [Physics-based Sound Synthesis for Games and Interactive Systems][physics-sound-synthesis-course]?

One way to start to answer these questions is to look at what the market says through job postings.  As Patrick McKenzie stated, most jobs actually aren't posted and most positions aren't filled through job postings [[2]](#2-note).  Nevertheless, analyzing the public record of the market can provide valuable insight.

### Research

I manually went through {{ site.data.audio-jobs | size }} job postings.  The following are my findings.


#### Titles
##### Frequency of Words in Titles
{% assign min_title_frequency = 4 %}
The following words appeared in the title of job postings at least {{ min_title_frequency }} times.
<canvas id="title-token-frequencies"></canvas>

#### Locations
CA - 49
WA - 21
MI - 6
MA - 21
GA - 2
TX - 5
IL - 3
FL - 5
UT - 2
CO - 1
IN - 1
MD - 1

UK - 12
India - 6
China - 4
Sweden - 2
Finland - 2
Germany - 2
Italy - 1
Belgium - 1
Taiwan - 1
Spain - 2
Poland - 1
Singapore - 1



#### Industries

#### Education 

#### Languages

<!-- todo, affiliate links? Need to update privacy notice if so -->
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
      <th>Description</th>
   </tr>
   {% for job in site.data.audio-jobs %}
      <tr>
         <td><a href="{{ job.URL }}">{{ job.Title }}</a></td>
         <td>{{ job.Company }}</td>
         <td>{{ job.Location }}</td>
         <td></td>         
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
   var chart = new Chart(ctx, {
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
</script>
