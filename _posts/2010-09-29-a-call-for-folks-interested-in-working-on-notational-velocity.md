---
layout: post
title: A call for folks interested in working on Notational Velocity
redirect_from: /home/2010/09/29/a-call-for-folks-interested-in-working-on-notational-velocity/index.html
---
<p><strong>Update</strong>: Most of the wishes in my Notational Velocity wish list have now been granted by Brett Terpstra and others. My current choice for Notational Velocity is Brett's <a href="http://brettterpstra.com/code/notational-velocity-alt">nvALT</a>.
<p style="text-align: center;">* * *</p>
<p>The most popular PE posts by far continue to be several that I wrote earlier this year on Markdown, MultiMarkdown, and Notational Velocity and how I use them in my writing workflows:</p>
<ul>
<li><a href="http://www.practicallyefficient.com/2010/06/01/notational-velocity-multimarkdown-and-simplenote/">Building a better writing workflow with Notational Velocity, MultiMarkdown, and Simplenote</a></li>
<li><a href="http://www.practicallyefficient.com/2010/06/01/notational-velocity-multimarkdown-and-simplenote/"></a><a href="http://www.practicallyefficient.com/2010/06/01/notational-velocity-multimarkdown-and-simplenote/">My MultiMarkdown writing workflow with LaunchBar and Hazel</a></li>
<li><a href="http://www.practicallyefficient.com/2010/08/09/my-spreadsheet-to-multimarkdown-table-workflow/">My spreadsheet to MultiMarkdown table workflow</a></li>
<li><a href="http://www.practicallyefficient.com/2010/07/13/using-textexpander-and-notational-velocity-for-fast-efficient-writing/">Using TextExpander and Notational Velocity for fast, efficient writing</a></li>
<li><a href="http://www.practicallyefficient.com/2010/09/03/a-moment-for-the-mundane/">A moment for the mundane</a> (a TextExpander/Markdown workflow)</li>
</ul>
<p>These workflows are made possible by <span style="text-decoration: line-through;">three</span> four key individuals. I owe them a huge thanks because I use their creations like crazy. These guys are:</p>
<ul>
<li><strong>John Gruber </strong>and <strong>Aaron Swartz</strong>, creators of <a href="http://daringfireball.net/projects/markdown/">Markdown</a> [Edit: apologies to <a href="http://www.aaronsw.com/">Aaron</a> for not including him originally here]</li>
<li><strong>Fletcher Penney</strong>, creator of <a href="http://fletcherpenney.net/multimarkdown/">MultiMarkdown</a> (an extension of Markdown)</li>
<li><strong>Steven Frank</strong>, who <a href="http://en.wikipedia.org/wiki/Fork_(software_development)">forked</a> Notational Velocity to create a <a href="http://github.com/panicsteve/nv/downloads">version with a live-updating HTML preview pane</a></li>
</ul>
<p>I’ve had several email exchanges with Steven about my personal interest in working on Notational Velocity. He’s been really helpful and responsive.</p>
<p>But the reality is that I’m not a programmer. Moreover, I just can’t find the time to get myself up to speed enough to do anything meaningful with the Notational Velocity source code myself. But I definitely have a few ideas on how it could be enhanced to add even more value to my writing workflows.</p>
<p>Given all the interest in (Multi)Markdown and Notational Velocity here at PE through comments, emails, and search traffic, I thought I would just throw out some of my own ideas for future enhancements.</p>
<h2 id="howicanhelpyou">How I can help you</h2>
<p>If you are interested in extending Notational Velocity further, feel free to use the ideas in this post, leave comments here, or contact me.</p>
<p>If you implement any of these ideas (or others that come along later) to create a new stable version of Notational Velocity, I can help you in the following ways:</p>
<ul>
<li>Promote your work with a blog post</li>
<li>Provide a permanent link to your work on this site</li>
<li>Provide design feedback based on my own use</li>
<li>General beta testing</li>
</ul>
<p>So without further rambling, here is my wishlist…</p>
<h2 id="ideasforextendingnotationalvelocity">4 ideas for extending Notational Velocity</h2>
<p>Each of these is intended to enhance Notational Velocity as a web writer’s tool while keeping the interface as minimalist as possible:</p>
<ol>
<li>Move HTML preview pane into a ‘fly-out’ drawer</li>
<li>View HTML source</li>
<li>Export as HTML</li>
<li>Add support for MultiMarkdown</li>
</ol>
<h3 id="idea1:movemarkdownpaneintoafly-outdrawer">Idea 1: Move HTML preview pane into a ‘fly-out’ drawer</h3>
<p>If you’ve ever used a program like <a href="http://www.cocoatech.com/">Path Finder</a>, you’re familiar with the fly-out drawers that expand and collapse on each side of the main interface.</p>
<p>When I write in Steven’s version of Notational Velocity, I often keep the HTML preview pane at the bottom hidden until I’m ready to review things.  As I edit, I find myself going back and forth between the two panes as I edit what I’ve written.</p>
<p>I think that if the HTML preview pane was on the right side (and the same height as the Notational Velocity writing area), it would be easier to go back and forth. A “right to left” flow is also consistent with core Mac design principles that can be found in everything from file menus to iOS apps.</p>
<p>Here is an unartistic sketch of how an HTML 'fly-out' drawer might be implemented on the right side of the main Notational Velocity window:</p>
<p><a href="/img/NV-mockup-pe.png"><img class="aligncenter size-full wp-image-1630" title="NV-mockup-pe" src="/img/NV-mockup-pe.png" alt="" width="534" height="435" /></a></p>
<p>The user would have the option of keeping the drawer hidden or exposed by clicking a discreet button somewhere, or perhaps through a keyboard shortcut.</p>
<p>Synchronous scrolling between the writing area and drawer pane would be a bonus too.</p>
<h3 id="idea2:viewhtmlsource">Idea 2: View HTML source</h3>
<p>I’ve already written about how I use Hazel to automate the conversion of Markdown to HTML.  If I could view the HTML source underlying the HTML pane in Notational Velocity, I could cut Hazel out of my workflow. (It won’t hurt her feelings; I promise.)</p>
<p>I’m pretty sure that the HTML preview pane is a web browser, so perhaps just adding “View Source” menu option (like a regular web browser) would suffice.</p>
<h3 id="idea3:exportashtml">Idea 3: Export as HTML</h3>
<p>As an alternative to Idea 2, a menu option that lets the user export the current note as an HTML file would also be great.</p>
<h3>Idea 4: Add support for MultiMarkdown</h3>
<p>This one is self-explanatory, I think. By adding support for MultiMarkdown, not just Markdown, the HTML preview pane would be capable of displaying MultiMarkdown-specific items like HTML tables.</p>
<h2 id="fromhere">From here</h2>
<p>As I said above, I’m really grateful to everyone that’s played a role in creating these great tools.  Steven Frank’s version of Notational Velocity is awesome, and it’s changed how I write for the better.</p>
<p>If you like or dislike my ideas above, let me know.  If you have your own, let me know those too. Let’s worth together to make Notational Velocity as great as it can be.</p>
<p><strong>A few more resources:</strong></p>
<ul>
<li>The official home of Notational Velocity, <a href="http://notational.net/">notational.net</a></li>
<li><a href="http://github.com/scrod/nv/tree/">The main Notational Velocity source code</a></li>
<li><a href="http://github.com/panicsteve/nv/downloads">Steven Frank's version of Notational Velocity</a></li>
<li><a href="http://git-scm.com/">Git</a> (required for working with Notational Velocity source code)</li>
</ul>
