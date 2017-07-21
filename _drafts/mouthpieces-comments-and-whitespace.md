---
title: Mouthpieces, Comments & Whitespace
description: In this post I explore the concept of learning seemingly basic lessons that catapult one's developement in their craft.  I take two exmaples taken from my life, one involving a mouthpiece and the other involving comments and whitespace.     
comments: true
---

Sometimes there is a lesson, exercise or some concept that you learn that just catapults your development forward.  It could be a small thing … something not so obviously influential; but once you absorb it, your craft just moves forward.

### Musical Catapult
I had such an experience practicing the saxophone.  I started out playing the saxophone in fourth grade [[1]](#1-note) and continued through high school.  I had no formal plans on how I would continue playing after high school so the summer after I graduated I asked my mother if I could get lessons [[2]](#2-note).  She set up four lessons with an instrumental music teacher in my local school system.  I met with Mr. Fogleman in his home and we went over many things, much of which I do not remember.  I do remember him showing me the software [Band-in-a-Box][band-in-a-box].  It can generate a musical rendition of virtually any chord progression of popular music [[3]](#3-citation).  Musicians play along with the computer generated accompaniment to practice.  I thought it was cool.   

But there was one lesson that really stood out [[4]](#4-note).  Mr. Fogleman took me to a piano and asked me to only bring my [mouthpiece][mouthpiece].  He proceeded to play his mouthpiece, that is, to make a buzzing sound on it.  He would play a note on the piano and then play the same note on his mouthpiece.  He did this for many notes.  When I attempted to play my mouthpiece, I could only play one note.  I couldn’t work my mouthpiece to play a variety of notes like my teacher could.  I went home and over the course of the next week I worked on this exercise often.  By the end of the week, I could play a full [chromatic scale][chromatic-scale] on the piano and match each note on my mouthpiece.  The next time I met with Mr. Fogleman, he noted that my sound on the saxophone changed.  He was impressed and told me to continue practicing it.  I could hear the change as well, my tone was more “professional” [[5]](#5-note). 

So what happened?  Was there something magical about making buzzing sounds with my mouthpiece and matching notes played at the piano?  Not exactly; the key was the adjustment needed in order to execute the exercise.  What Mr. Fogleman taught me was how to loosen my [embouchure][embouchure].  It's very difficult to play different notes on your mouthpiece with a tight embouchure, so you naturally have to loosen it in order to play different notes.  When you play with a tight embouchure, you tend to produce [a very thin tone which is very common when first learning to play][bob-reynolds-thin-tone-example].  As you gain more flexibility in your embouchure, you are able to facilitate more air through your mouthpiece and subsequently your horn which produces a much fuller sound.

### Software Catapult
Similar to the musical experience I had as a teenager, I learned a principle that moved my software craft & style forward.

I've always prided myself with writing clean, clear code.  I love the feeling when a design feels just "right".  Sometimes when I've written what I deemed to be "my best work" at the moment, I randomly would secretly go back from time to time and just read through and admire it.  It's always been my goal that if anyone ever had to maintain code I've written, it would be easy and painless for them to get up to speed on it.  I always tried to use the least amount of code possible that still was readable.

These are good goals, but were my habits the most effective way to achieve them?

#### Comments
In an attempt to be sympathetic to future maintainers, I used to write a lot of comments.  If there was a loop ... comment.  If there was a block of code ... comment.  I would comment/document all public and private methods.

#### Whitespace
For the sake of being able to quickly see the high level steps in a block of logic, I would use whitespace to separate expressions into groups.  If I had to loop through a collection of elements ... proceeding whitespace.  If I needed to perform conditional logic ... proceeding whitespace.  If I had a series of expressions performing operations on a variable ... proceeding whitespace.  

Below is code I actually wrote during my first computer science course in college [[6]](#6-note).  It actually exhibits some of the aforementioned things:

{% highlight java linenos %}
public Hangman(String[] words) {
    // Generates a random index value so a random word can be used	
    int randomIndexValue = (int)(Math.random()*words.length);
    stringGameWord = words[randomIndexValue];
		
    // Changes the Solution word letters to uppercase 
    stringGameWord = stringGameWord.toUpperCase();
    //Length of the word that is being guessed
    gameWordLength = stringGameWord.length();
    
    RandomWord();
}

private String RandomWord(){
    // Concatenates the need "_" symbols for the blanks spaces	
    for (int i = 0; i<gameWordLength; ++i){
        blankSpace = blankSpace + "_ ";	}

    //The blank space array is copied as an array so it can be used fill in the user's correct guesses
    blankSpaceArray = blankSpace.toCharArray();

    inputBoxMessage = "Please enter your guess \n" + blankSpace;
    ...
}
{% endhighlight %}

#### Code Smell: Whitespace & Comments
I started to change my thinking on these things some time ago when I came across a [blog post][yegor-bugayenko-empty-line-smell] by [Yegor Bugayenko][yegor-bugayenko].  He argued that whitespace is a [code smell][code-smell].  A method should do only one thing and do it well.  If you have whitespace in your method body, it's likely doing more than one thing.  This made a lot of sense.

If one is tempted to use whitespace, consider refactoring the logic into it's own method with a clear name.  This makes a world of difference and really cleans up your code.  This principle has served me well.

Then I wondered about comments.  If my use of whitespace was not ideal, then my use of comments was likely equally suspect; why would I need inline comments if my method was doing one thing and doing it well?  It turns out that [comments are also regarded as a code smells][code-smells-coding-horror].  Jeff Atwood has written on the topic numerous times [[7]](#7-note).  Atwood argues that "You should always write your code as if comments didn't exist." [7a](#7a-citation).  Your code should be simple and self-documenting.  Instead of commenting, refactor the logic into its own method with a clear name.  Though [there are exceptions][necessary-comments], comments should be the first resort in making code clearer.

It's better to treat guidelines as warning signs versus hard laws to follow, but it is good to consider refactoring when you have the urge to use whitespace and comments.  I also treat it as a warning sign if I can't understand what a method is doing after a quick glance.

#### College code revisted
Here is how I would rewrite the code snippet, from my first com sci college course, above:

{% highlight java linenos %}
public Hangman(String[] words) {
    gameWord = randomWord();
    gameWord = gameWord.toUpperCase();		
    userPrompt = "Please enter your guess \n" + wordPlaceHolder();
    ...
}

private String wordPlaceHolder() {
   final StringBuilder underscores = new StringBuilder();
   for (int i = 0; i < gameWord.length(); ++i) {
      underscores.append("_");
   }
   return underscores.toString();
}

private String randomWord() {
    final int index = (int)(Math.random() * words.length);
    return words[index];
}
{% endhighlight %}

### Notes
[band-in-a-box]: http://www.pgmusic.com/
[band-in-a-box-wiki]: https://en.wikipedia.org/wiki/Band-in-a-Box
[ben-bederson]: https://www.cs.umd.edu/users/bederson/
<!-- Need to replace with actual clip -->
[bob-reynolds-thin-tone-example]: http://www.bobbyowolabi.com 
[chromatic-scale]: https://en.wikipedia.org/wiki/Chromatic_scale
[code-smell]: https://en.wikipedia.org/wiki/Code_smell
[code-smell-coding-horror]: https://blog.codinghorror.com/code-smells/
[coding-without-comments]: https://blog.codinghorror.com/coding-without-comments/
[comments-tell-you-why]: https://blog.codinghorror.com/code-tells-you-how-comments-tell-you-why/
[when-good-comment-go-bad]: https://blog.codinghorror.com/when-good-comments-go-bad/
[embouchure]: https://en.wikipedia.org/wiki/Embouchure
[gary-bartz]: http://web.archive.org/web/20130604124040/http://garybartz.com/
[mouthpiece]: https://en.wikipedia.org/wiki/Mouthpiece_(woodwind) 
[music-is-just-music]: http://web.archive.org/web/20130317003848/http://irockjazz.com:80/2013/02/music-is-just-music-gary-bartz/
[necessary-comments]: http://blog.cleancoder.com/uncle-bob/2017/02/23/NecessaryComments.html
[yegor-bugayenko]: http://www.yegor256.com
[yegor-bugayenko-empty-line-smell]: http://www.yegor256.com/2014/11/03/empty-line-code-smell.html

[<a name="1-note">1</a>] Fourth grade was the first year students were eligible for the instrumental music program in my elementary school.

[<a name="2-note">2</a>] The first time I received music lessons. 

[<a name="3-citation">3</a>] Wikipedia contributors. ["Band-in-a-Box."][band-in-a-box-wiki] Wikipedia, The Free Encyclopedia. Wikipedia, The Free Encyclopedia, 19 May. 2017. Web. 25 May. 2017. 

[<a name="4-citation">4</a>] ["Music Is Just Music."][music-is-just-music] Interview by Gail Perry, Keli Denise, and Gary Bartz. IRock Jazz. N.p., 27 Feb. 2013. Web. 21 July 2017. 

[<a name="4-note">4a</a>] In an [interview][music-is-just-music] [[4]](#4-citation), [Gary Bartz][gary-bartz] stated "If a teacher teaches you one thing, they have done their job. If a teacher teaches you multiple things, they have done a heck of a job."  He stated this in the context of talking about one of his professors, Albert Holloway, who helped him "understand that I would not be able to learn or be inspired by any ONE person."     

[<a name="5-note">5</a>] I continued playing on and off through my adult years.  Whenever I received compliment, it was never, “you have good chops”, or anything about my technical proficiency / musical ideas.  It was always “you have a really good tone”.  What Mr. Fogleman showed me that day is to thank for that.  When I would receive this compliment, I used to feel bad.  I always felt like I got this compliment because I was so deficient in the other areas of my playing and I hadn’t put in the necessary time to grow in the other areas.  But hey, it's never too late to improve :-)

[<a name="6-note">6</a>] The course was CMSC 131: Object-Oriented Programming I - Spring 2004 taught by [Ben Bederson][ben-bederson].  I'd like to say my coding style was improved by the time I started working professionally, but I still was a comment and whitespace machine.   

[<a name="7-note">7</a>] Jeff Atwood has written on the topic of the misuse of comments: [Coding Without Comments][coding-without-comments], [Comments Tell You Why][comments-tell-you-why], [When Good Comments Go Bad][when-good-comment-go-bad] and [Code Smells][coding-horror-code-smells].

[<a name="7a-citation">7a</a>] Atwood, Jeff. [Coding Without Comments][coding-without-comments]. Blog. Coding Horror. Publish 24 July 2008. Web. 21 July 2017. 
