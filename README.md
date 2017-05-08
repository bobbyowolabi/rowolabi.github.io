## About

[The blog of Bobby Owolabi](https://rowolabi.github.io), made with Jekyll.

## Template used

[Monochrome](https://github.com/dyutibarma/monochrome)

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
   
updated inline links; came up with convention id#-citation|link|note. I define all the links at the bottom of the page using the convention id#-link. This allows me to simply put [link-text][id#-link] in the body of the post and not have any URLs appear in the body of the post markdown. 


## License
Released under [MIT License](license.md).
