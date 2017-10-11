# [bobbyowolabi.com][blog]
*The Intersection of Audio, Coding & Music*

## About
This is my personal blog where I share about my exploration of "audio programming", software engineering and music.

## Site Generator
This site is built with [jekyll][jekyll].

### Plugins
* jekyll-paginate
* jekyll-sitemap

## Template
I created this site based off of the [Monochrome][template] template created by [@dyutibarma][dyutibarma].

## Dependencies
* Font Awesome
* Chart.js
* Google Analytics
* Disqus

## Citation Methodology
Efforts will be made to carefully cite sources in the posts of this blog.

### Markdown Citation Strategy
1. **Define URLs at the End of the Markdown File**

   This allows for the body of the markdown to be free of long URLs thus increasing readability.
   
   *Inline:* `I found the [online app][id-link] to be extremely helpful.`
   
   *End of File:* `id-link: URL`

1. **Use Anchors to Provide Context / Additional Information**

   This is very much in the style of the "Notes" section at the end of [Graham's essays](http://paulgraham.com/articles.html)
   
   *Inline:* `Using comments in the body of your code should be avoided; only comment your public interfaces. [[id]](#id-note)`
   
   *End of File:* `[<a name="id-note">id</a>] This is a subject that people often disagree on ...`

1. **Use Anchors to Provide Citations**

   Provide citation of sources such as blog posts, videos, articles, etc.
   
   *[Blog Post Citation Format:][1]* 
   
   `Last Name, First Name. Title Medium Type. Title of Blog. Publish Date. Web. Access Date. URL`
   
   *Inline:* `The author states that test driven development is the only approach that guarantees a comprehensive test suite [[id]](#id-citation)`
   
   *End of File:* `[<a name="id-citation">id</a>] Doe, John. "Thoughts on Testings." Blog post. The Blog of John. 29 Sept. 2016. Web. 3 Apr. 2017. <http://theblogofjohhn.com/2016/09/thoughts-on-testing.html>.` 
   
## License
> Copyright © 2017-Present Robert B. Owolabi.

Code Released Under [MIT License](license.md).


[1]: https://www.easybib.com/guides/citation-guides/mla-format/how-to-cite-a-blog-mla/
[blog]: https://www.bobbyowolabi.com
[dyutibarma]: https://github.com/dyutibarma
[jekyll]: https://jekyllrb.com/
[template]: https://github.com/dyutibarma/monochrome
