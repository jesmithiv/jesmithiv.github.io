---
layout: post
title: Static and free 
---

My time with Squarespace ended today. It was never an entirely happy marriage between us, and it’s not worth spilling every detail why, but I will say that the main thing that ultimately drove me from Squarespace for good was its poorly implemented Markdown editor.

I feel that I should qualify that “poorly” because I really do mean *poorly for me*, and I don’t have any fantasies that I’m a typical Squarespace user or that I know more about Squarespace’s user base than Squarespace knows. I fully believe Squarespace has designed its user interface with its primary customers in mind.

But as it stands now, Squarespace is not a place for lovers of Markdown, and that is who I’ve been for years and likely always will be. Even though Squarespace was among the first major blogging platforms to welcome Markdown-based blogging, I don’t think the Markdown functionality in Squarespace ever got past “add-on” status. It is a window within a window within other windows and will likely never be front and center in the user experience. 

All of these things have been said before about Squarespace, and I can’t think of anything to add to [Claus Wilke’s take on it](http://serialmentor.com/blog/2015/8/6/goodbye-squarespace/):

> While Squarespace posts can in principle be written in Markdown, Squarespace’s Markdown capabilities are limited and buggy. In particular:
> - Code blocks are buggy. Specifically, Squarespace doesn’t properly escape special characters in code blocks. This can make embedding code into Markdown posts a big headache.
> - Images cannot be inserted directly from the Markdown.
> - To insert images, one has to break the Markdown into two parts and insert an image block in between. As one does so, Squarespace rewrites the Markdown and turns all inline links into reference-style links. While this doesn’t alter the page output in any way, I prefer to use software that doesn’t randomly rewrite my source code.
> - The online Markdown editor Squarespace provides is slow and buggy. For longer pieces of text, the cursor is often displayed at the wrong location, so that it becomes difficult to edit the text at all.

### Life and content go on... to Jekyll

It’s fitting to quote Claus above because he was writing about why he moved from Squarespace to [Jekyll](https://jekyllrb.com)—footsteps that I’ve now followed.

As blog nerds and GitHub power users know, Jekyll is a popular static blogging platform that lets you write and maintain all post content in Markdown. Like other static frameworks, Jekyll basically builds a database-free, static HTML website from Markdown and other configuration files. Though the setup takes some nerdery, the final result is as basic and pure a thing as you can find on the internet: a folder structure of HTML files.

Jekyll is not the first static platform I’ve attempted to move to, and I’m grateful my previous attempts to move to other static frameworks failed because I can’t think of a better place to be than Jekyll now—although many, many good static site options now exist. 

Ultimately I chose Jekyll over other options because:

- Jekyll is very popular and well developed.
- GitHub—the center of the developer universe—loves Jekyll and uses Jekyll to power virtually all of its user-editable pages.
- Since GitHub is so Jekyll-friendly, I was able to [host the whole site there for free](http://jmcglone.com/guides/github-pages/). At some point I may move to my own server, but it’s super convenient to have a powerhouse like GitHub take care of running Jekyll to re-build the site when something changes, not to mention the obvious local syncing benefits with any GitHub repository. 
- Jekyll’s framework for Markdown files with YAML front matter is substantially the same as other popular static platforms making it easy to switch to something else down the road if necessary.

A static site is very close to the antithesis of Squarespace in terms of user skill set required. Many people will rightly question the value I’m gaining by simply being able to write and maintain my site directly in Markdown. If that were the only criterion, I think fair arguments could be made against my moving.

But for me, the value of the move is much longer-term in nature.

- I got to sharpen my Shell and Python scripting skills while cleaning up my old posts to make them Jekyll-ready.
- Converting all of my older posts into Markdown files means I now truly own the things I’ve written and can easily move them anywhere. They’re out of the black box.
- I learned a little Ruby, which is what Jekyll runs on.
- I learned much more about GitHub than I used to know and plan to put that knowledge to work for other projects.
- I learned more CSS tricks and discovered the power of [SASS](http://sass-lang.com), which actually makes me not hate working with CSS anymore. So useful.
- I’m in the process of learning some cool tricks in iOS that I plan to use for iOS-based publishing.
- I no longer rely on first-party apps for publishing. 

### Overview of how I moved

There’s no such thing as a boilerplate list of steps for moving from Thing A to Thing B on the internet. To each his own sub-steps. And it’s in those sub-steps where both dragons and fun be alike. But for those that care, here are the primary steps I took over the course of several nights and weekends:

1. I exported my Squarespace site to a WordPress XML file (the only option).
2. I used [this godsend of a Ruby script](https://gist.github.com/evanwalsh/6131008) by Evan Walsh to convert the XML file into individual Markdown files. This was a major leap forward, but in reality this is where the real the fun began.
3. I wrote several Python scripts to clean up the Markdown file names and insert YAML fields for things like redirects. This was a major step, and I think I’m going to put these in a different post because they were fun to make and worth saying more about on their own.
4. I installed Jekyll on my Mac so I could build the site locally on my Mac and experiment with things. I highly recommend this even though GitHub can build it for you too.
4. I spent a lot of time reading the Jekyll documentation and learning how to work with the Jekyll framework, which can seem intimidating at first if you’re not a web developer, but it quickly collapses into a beautifully intuitive framework. It’s so worth the time to learn if you want to empower yourself with a static site.
5. I spent a few nights tweaking the CSS of the stock Jekyll theme to make it look like I think Practically Efficient should look. 
6. I moved the files to my GitHub account, flipped a few [DNS switches](https://help.github.com/articles/setting-up-a-www-subdomain/), and was done. 

Other good resources:

- "[Build a Blog With Jekyll and GitHub Pages](https://www.smashingmagazine.com/2014/08/build-blog-jekyll-github-pages/)"
- "[How I Created a Beautiful and Minimal Blog Using Jekyll, Github Pages, and poole](http://joshualande.com/jekyll-github-pages-poole/)"

You may be wondering about images. Fortunately I have local copies of nearly every image I've ever posted, so I didn't need to pull those off Squarespace. 


### Some thank you’s framed in bigger pictures

Even though I didn’t solicit much direct help in this move, I’m so grateful for the inspiration I’ve gotten from [Gabe Weatherhead](http://www.macdrifter.com), [Ryan Irelan](http://ryanirelan.com), and [Dr. Drang](http://leancrew.com/all-this/). They’re all much handier than I am with static blogging and web things in general, but I’ve been influenced heavily by what they’ve done. In particular, I’m convinced I would not have the basic Python skills I have now if it weren’t for all the exposure I’ve gotten to it through Dr. Drang’s posts. 

Thank you all for being *you*. 

Even though indie blogging has been relegated to third-, fourth-, maybe fifth-class citizen status on the internet in the last few years, I’m still grateful it lives on through the people who won’t let it go. I've seen so many talented, passionate bloggers move on to other mediums like podcasting or get sucked into aggregator-ish, socially-charged platforms like Facebook and Medium to chase the high of extra-instant attention, only to find that individual thoughts quickly wash away in a relentless social tsunami that leaves no trace of individual identity or permanence.

If static sites increase the longevity of indie web writing, that’s just one more reason to support static blogging and the individuals that freely share information that empowers others. 


 
