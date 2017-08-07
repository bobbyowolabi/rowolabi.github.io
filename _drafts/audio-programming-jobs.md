---
title: Audio Programming Jobs
description: 
comments: true
---

I've been thinking a lot about the field of audio and its prospects as a software engineer.

I've read a big chunk of [So Good They Can't Ignore][so-good-they-cant-ignore-you] by Cal Newport and I've taken away that for the vast majority of people, becoming highly skilled at something comes before passion.  We often try to find our passion first and then pursue it; however, when you examine passionate, successful people, it's often the case that their passion (and subsequent desirable lifestyle) came after investing in becoming a "craftsmen" in their field.  They built upon acquired career capital instead of starting from scratch in a new field.

I've read a big chunk of [Soft Skills: The software developer's life manual][soft-skills-sonmez] by John Sonmez and one of the things I've taken away is that a software engineer needs to specialize.

I've done a lot of reading and researching.  Some of the links I've come across can be found [here](#audio-links).

What do you call a software engineer that works in audio?  An audio programmer?  An audio software engineer?  How about an audio digital signal processing (DSP) engineer?

What domains do such individuals work in? Music? Speech? Communications?  Academia?  Gaming?

Is it possible to live anywhere and do this work?  Can you work remotely?  Can you consult?

What technologies and concepts should one study?  I admire the work and business that the folks of [AudioKit][audio-kit] are creating for themselves.  That could be a good place to start.  They recently wrote of [some project ideas][audio-kit-projects] that new folks can pursue.  I recently purchased [The Scientist and Engineer's Guide to Digital Signal Processing][dsp-guide-amazon] by Dr. Steven W. Smith.  It is [available online for free][dsp-guide-site].  I got excited after skimming through it because it was written in a very approachable way.  Should I start there?  What about taking the Stanford's [MOOC][mooc] course [Audio Signal Processing for Music Applications][audio-signal-processing-course].  Or how about the course [Physics-based Sound Synthesis for Games and Interactive Systems][physics-sound-synthesis-course]?

One way to start to answer these questions is to look at what the market says through job postings.  As Patrick McKenzie stated, most jobs actually aren't posted and most positions aren't filled through job postings [[1]](#1-note).  Nevertheless, analyzing the public record of the market can provide valuable insight.

### Research

I went through {{ site.data.audio-jobs | size }} job postings.


#### Titles
{% for job in site.data.audio-jobs %}
   {% assign title = job.Title | replace: ",", " " | replace: ")", " " | replace: "(", " " | replace: "/", " " | downcase | split: " " | join: ", " %}
   {% if forloop.first == false %}
      {% assign title_tokens = title_tokens | append: ", " %}
   {% endif %}
   {% assign title_tokens = title_tokens | append: title %}
{% endfor %}

{% assign title_tokens = title_tokens | split: ", " | sort %}
{% assign current_token = "" %}
{% for title_token in title_tokens %}
   {% if current_token == title_token %}
      {% assign count = count | plus: 1 %}
   {% else %}
      {% if current_token != "" %}
         {% assign results = results | append: current_token | append: ":" | append: " " | append: count | append: "; " %}
      {% endif %}      
      {% assign current_token = title_token %}
      {% assign count = 1 %}
   {% endif %}   
{% endfor %}

{% assign results = results | split: "; " %}
{% for result in results %}
   {{ result }}
{% endfor %}

* highest word frequency

* Different Title Combinations
ex: software engineer, research, dsp, etc



#### Locations


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


### Notes
[<a name="1-note">1</a>] McKenzie wrote, '"Read ad.  Send in resume.  Go to job interview.  Receive offer." is the exception, not the typical case, for getting employment: Most jobs are never available publicly, just like most worthwhile candidates are not available publicly [(see here)][finding-great-developers] ...' [[1a]](#1-citation)

[<a name="1-citation">1a</a>] McKenzie, Patrick. [Don't Call Yourself A Programmer, And Other Career Advice][dont-call-yourself-a-programmer-patio11]. Blog. Kalzumeus Software Blog. Publish 29 October 29 2011. Web. 28 July 2017. 

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

### Audio Links
