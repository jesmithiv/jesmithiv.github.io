---
layout: post
title: My MultiMarkdown writing workflow with LaunchBar and Hazel
redirect_from: /home/2010/05/19/my-multimarkdown-writing-workflow-with-launchbar-and-hazel/index.html
---
<p><img class="alignnone" src="/img/feather-pen.jpg" alt="" width="400" height="500" />
<em>[Photo by <a href="http://www.flickr.com/photos/monster/3431407135/">Monster</a> via Flicker]</em></p>
<p>My intention with this blog is providing clear, not-so-geeky explanations and ideas on using technology to improve your life.  However, I’m going to momentarily shift toward the geeky end of the spectrum in this post and talk about my writing workflow with MultiMarkdown.  I’ve noticed that a significant portion of the traffic I get from search engines are people looking for information on MultiMarkdown, which I wrote about in an <a href="http://www.practicallyefficient.com/2010/03/24/improve-your-web-writing-by-getting-back-to-basics-with-multimarkdown/">earlier post</a>.</p>
<p>I owe much of my awareness of the programs I use in this workflow to the <a href="http://macpowerusers.com/">Mac Power Users (MPU) podcast</a>, an excellent resource on a variety of things Macintosh.  If you are a Mac user of any experience level, I guarantee that you will learn a lot by listening to MPU.</p>
<p>My writing workflow utilizes several tools that I discovered through MPU.  However, I feel that I’ve created my own unique combination of these tools in a way that suits me.  Maybe it can help you too.</p>
<p><!--more-->
Most of my workflow is centered around <a href="http://fletcherpenney.net/multimarkdown/">MultiMarkdown</a>, but it becomes even more useful with the following additional ingredients…</p>
<ul>
<li><a href="http://www.obdev.at/products/launchbar/index.html">LaunchBar</a></li>
<li><a href="http://www.noodlesoft.com/hazel.php">Hazel</a></li>
</ul>
<p>This post is essentially a recap of my journey with MultiMarkdown (so far) and how I’ve implemented the tools above.</p>
<h2 id="whymultimarkdown">Why MultiMarkdown</h2>
<p>Obviously, people wrote long before computers.  And in some ways, the pre-computer world was a better one for writers.  There were fewer distractions, fewer traps between thoughts and text.  The writer was not encumbered by decisions as to font choice and line spacing.  Those decisions came later, and they were the domain of the publisher.  The writer’s job was simply to move a pen across a page.</p>
<p>Now, I don’t use pen and paper, at least not very often.  But I do use the closest computer substitute there is: the text editor.  My choice is simply TextEdit, the basic text editor that comes with Mac OS X.  I know that many Mac gurus prefer more feature-rich editors like <a href="http://macromates.com/">TextMate</a>, and with the <a href="http://fletcherpenney.net/multimarkdown/multimarkdown_bundle_for_textm/">MultiMarkdown bundle</a>, I’m sure that it’s a powerful tool. I may test drive that setup at some point, but right now I’m trying to keep things simple: black words on a white background; nothing more.</p>
<p>Writing MultiMarkdown in TextEdit makes me feel closer to a purer state of content creation and the art of writing.  It liberates my brain from making visual decisions as I write.</p>
<p>In the <a href="http://www.practicallyefficient.com/2010/03/24/improve-your-web-writing-by-getting-back-to-basics-with-multimarkdown/">summary</a> I wrote of MultiMarkdown earlier, I discussed the basic syntax, which is mostly derived from <a href="http://daringfireball.net/projects/markdown/">Markdown</a>, created by John Gruber.</p>
<p>I think writing in Markdown or MultiMarkdown is fairly straightforward.  Where some people may be intimidated is the process of converting MultiMarkdown to HTML (or whatever publishing format you desire).  The most basic way of doing this conversion is using a Terminal command like:</p>
<pre><code>mmd2XHTML.pl file.txt</code></pre>
<p>Terminal commands often intimidate people for various reasons.  So if this step makes you fearful, it’s likely you won’t try MultiMarkdown.  I mean, what’s the point of using a tool that you perceive to be difficult? That’s logical enough, and I won’t attempt to assuage your fears of Terminal.</p>
<p>Fortunately, Fletcher Penney, creator of MultiMarkdown, provided a nice to solution that curbs the geekiness of this step a bit.  Using his <a href="http://fletcherpenney.net/multimarkdown/multimarkdown_drag_and_drop/">drag and drop apps</a>, you can simply plop your MultiMarkdown text file onto the appropriate app.  A little progress window will appear, and magically your file will be converted to HTML, PDF, RTF, etc. The new file will be sitting right next to your text file in Finder.</p>
<p>Drag and drop is nice, and maybe it’s suitable for most people.  But I wanted something even more seamless.</p>
<h2 id="launchbarmultimarkdown:aprettydarnefficientworkflow">LaunchBar + MultiMarkdown: a pretty darn efficient workflow</h2>
<p>LaunchBar seems to find its way into just about all of my Mac workflows.  It’s an indispensable layer on top of the core OS that I use so much now that I take it for granted–until I’m on a computer without it.  Like its aging predecessor, <a href="http://www.blacktree.com/">Quicksilver</a>, LaunchBar ensures that launching an app, opening a file, performing a quick calculation, and myriad other actions are only a few keystrokes away.</p>
<p>Initially, I was using LaunchBar to process MultiMarkdown for HTML conversion:</p>
<ol>
<li>CMD+SPACE to invoke LaunchBar</li>
<li>Locate my MultiMarkdown text file</li>
<li>TAB</li>
<li>Type “multi” (or less) to find  MultiMarkdown2XHTML.app</li>
<li>RETURN</li>
</ol>
<p><img src="/img/LaunchBar-MultiMarkdown.png" alt="LaunchBar-MultiMarkdown" /></p>
<p>This sequence tells LaunchBar to open the text file with MultiMarkdown2XHTML.app.  It works really well, and once I got this down, I thought I had found the ultimate solution for quickly processing MultiMarkdown files.</p>
<p>Then, I discovered a new tool.</p>
<h2 id="hazel:notjustamaidbutawritinghelper">Hazel: not just a maid but a writing helper?</h2>
<p>For me, Hazel was one of those Mac apps that I heard mentioned every so often but just never got around to investigating, at least not until recently.  Brief descriptions of Hazel usually don’t win it any glamor points.  It’s beauty is not beheld until seen in action.  And like so many great apps, it adds value by staying out the way and doing its thing.</p>
<p>At first blush, Hazel appears to simply be a way to keep your Mac tidy by emptying the trash, cleaning up your downloads folder, and doing other automated file/folder actions.  It’s worth buying just for these benefits alone.</p>
<p>However, Hazel is capable of much more.  Its framework allows for so many different automations that it truly begins to mold itself to person using it.  <a href="http://www.noodlesoft.com/forums/">Hazel’s forum</a> is filled with interesting uses.  MPU also did <a href="http://macpowerusers.com/2010/04/mpu-025-geeking-out-with-hazel/">a really good episode on Hazel</a> not long ago.</p>
<p>After playing with Hazel a bit and thinking about things you do on a regular basis, it’s likely that ideas will start popping in your head.</p>
<p>With my LaunchBar approach, I would typically write a decent first draft in TextEdit first.  Then, I would preview what I had written by invoking LaunchBar to generate an HTML file.  In this editing phase, I found that I was invoking LaunchBar a lot.  I often find many typos and decide to do heavy tweaking while editing.  This means frequently going back and forth between the MultiMarkdown text file and the web browser (invoking LaunchBar in between).</p>
<p>Repetition often indicates opportunity for automation.</p>
<p>Hazel is good at keeping up with all kinds of file attributes, some of which aren’t even monitored by OS X.  When I noticed the “Date Last Matched” variable, a light bulb came on.  I created the following Hazel rule for each folder where I compose blog drafts:</p>
<p><img src="/img/hazel.png" alt="Hazel rule" /></p>
<p>By saying “Date Last Modified is after Date Last Matched,” it tells Hazel to act on the file any time it changes.  Within a second or two of saving each draft, Hazel runs the text file through MultiMarkdown2XHTML.app, and out pops an HTML version of the document.</p>
<p>So when I’m ready the view the draft in a web browser, all I have to do is find the HTML file, double click it, and view.  As I make changes and save them in the text file, all I have to do is refresh the browser page (F5 in Firefox).</p>
<p>This really streamlined my writing workflow.  By letting Hazel worry about making HTML, it freed up even more time and energy to focus where the writing happens: TextEdit.</p>
<p>When I’m finally done, I simply open the HTML file in TextEdit and copy the code into WordPress, or other blogging platform.</p>
<p>Bonus: I also created another Hazel rule to delete the XHTML version of the file that MultiMarkdown2XHTML.app creates since I don’t need it.</p>
<h2 id="conclusion">Conclusion</h2>
<p>I don’t claim to write well.  Writing, like most things in life, is something you can improve on but never perfect.  My general goal with writing is to do it better than the last time.</p>
<p>Taking steps to ensure that I focus my energy as efficiently as possible while writing helps make my writing better, I think.</p>
<p>For me, MultiMarkdown + Hazel is a pretty powerful marriage.  In this case, power means simplicity.  It provides an extremely efficient, simple interface that lets me focus on writing in plain text.  It also forces me to put off formatting. (And sometimes I don’t have to do any formatting at all when I’m done.)  I also don’t have to trip over HTML mark-up as I write, and I don’t have to spend <em>any</em> time converting MultiMarkdown to HTML.</p>
<p>If you like to write on a regular basis, you may want to give MultiMarkdown a try.  By liberating yourself from ADD-inducing word processors and clumsy web-based blog editors, you may find that you produce higher quality content (text).</p>
<p>Please share your writing workflow tricks in the comments.</p>
