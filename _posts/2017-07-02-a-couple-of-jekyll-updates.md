---
layout: post
title: A couple of Jekyll updates
mathjax: true
---

Since [moving to Jekyll](http://www.practicallyefficient.com/2016/04/03/static-and-free.html) last year, I've done relatively little to tweak the inner workings of this site. After all, one of the most appealing things about having a static site is that it doesn't *need* to have a lot of moving parts. It just works.

But today I finally got around to a couple of housekeeping items that have been on my list: image captions and MathJax.

## Image captions

For image captions, I settled on a beautifully simple solution posted by [Andrew Wei on Stack Overflow](https://stackoverflow.com/questions/19331362/using-an-image-caption-in-markdown-jekyll):

	![](path_to_image)
	*image_caption*

This takes advantage of the fact that you can create CSS for combinations of HTML elements. In this case, I can use

	img + em { display: block; text-align: center;}

to target the `*image_caption*` text only and center it under images, which are also centered on this site by default. It works perfectly, and this isn't even Jekyll-specific. Anyone publishing in Markdown could do this. 

![](/img/einstein-simple.jpg "Einstein")
*Agreed.*


## Jekyll + MathJax

Adding MathJax took a little more time, but not much. It was worth it just to remind me of the brilliance of Jekyll's architecture. Even though the Jekyll site [mentions MathJax](https://jekyllrb.com/docs/extras/), it doesn't say enough to be of immediate use. It basically points to a blog post that entails switching from the default `kramdown` Markdown converter to `redcarpet`. Given that I'm happy with `kramdown` and not in the mood to backtest a bunch of blog posts with a different converter, I wanted to stick with `kramdown`.

A series of subsequent web searches lead me to a [Github issue thread](https://github.com/mmistakes/minimal-mistakes/issues/735) for a Jekyll theme that I'm not even using, but I found a really efficient implementation of MathJax there by user "mmistakes," who suggested adding a `mathjax` variable in each page's YAML front matter that could be set to `true` on a post by post basis.

The elegance of this solution is that the MathJax script will only be written into the HTML of posts that actually have MathJax in them. This seemed super appealing to me because it meant that I didn't have to worry about MathJax being triggered by some accidental combination of characters in an old blog post. 

I ended up adding

	 {% if page.mathjax %}
	<script type="text/javascript" async src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.1/MathJax.js?config=TeX-MML-AM_CHTML">
	</script>
	{% endif %}

to my `head.html` file, which contains Ruby instructions for building the contents of each page's `<head>` element. For any page where the YAML front matter has `mathjax: true`, the MathJax script will be included. I decided to always include it in the site's `index.html` file, which shows recent posts. And going forward, I can simply include it in the YAML front matter of any individual post. For example, this post's front matter is:

	---
	layout: post
	title: A couple of Jekyll updates
	mathjax: true
	---

I just finished up a project where I worked with MathJax a lot, and I continue to be impressed at how many LaTeX commands it handles. MathJax even has a special `enclose` library that handles special actuarial notation that eludes so many people. For example, 

	$$\require{enclose} {}_{17|}\ddot{a}_{x:\enclose{actuarial}{n}}^{(4)}$$

turns into:

$$\require{enclose} {}_{17|}\ddot{a}_{x:\enclose{actuarial}{n}}^{(4)}$$

Fun.


