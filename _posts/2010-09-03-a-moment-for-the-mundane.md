---
layout: post
title: A moment for the mundane
redirect_from: /home/2010/09/03/a-moment-for-the-mundane/index.html
---
<p><a href="/img/undo-and-ccp-pe.png"><img class="alignright size-full wp-image-1261" title="undo-and-ccp-pe" src="/img/undo-and-ccp-pe.png" alt="" width="281" height="133" /></a>For all the increases in productivity computers brought mainstream society in the last thirty years, I think the there are two fundamental functions that stand out as the most game-changing:
<ol>
<li>Cut/copy/paste</li>
<li>Undo</li>
</ol>
<p>These features are so common, so mundane, so boring, it’s easy to take them for granted.  They are definitely the most pervasive and universal software features I can think of.  Virtually all programs allow cut/copy/paste and undo whether you’re on a Mac, in Windows, or in Linux.</p>
<p>Both undo and cut/copy/paste are <a href="http://en.wikipedia.org/wiki/Involuntary_muscle">involuntary muscles</a> in your workflows. They’re as basic as a heartbeat or a breath of air. They happen naturally without you having to think about them.</p>
<p>But if you <em>do</em> think about them for a moment, they are quite a powerful pair.  And in many ways, they represented the first step away from the natural, physical world into virtual worlds.</p>
<p>It would be great if we had an undo button for “real life” – you know, that endearing term we assign to events occurring in the spaces between our screens. But we don’t. We also can’t clone and move physical objects with a click or tap of our finger.</p>
<p>So the introduction of cut/copy/paste and undo was, in many ways, remarkable. They represent true and lasting innovation.</p>
<p>I’m going to talk a little about how I use these taken-for-granted features in obvious and not-so-obvious ways (e.g. automating MultiMarkdown writing workflows).</p>
<p>But more importantly, I would like you to think about how you could better leverage  these and other mundane aspects of your workflow to create new and powerful efficiencies.</p>
<p><!--more--></p>
<h2 id="undo">Oops</h2>
<p>The basic undo button is a great way to get out of jams.  You can almost always backtrack whether you’re in a spreadsheet, word processor, or text editor.  Even browser-based blog editors have undo features now.  Command-Z is second nature.</p>
<p>Undo can also be used to make quick ad hoc comparisons.  For example, using undo/redo in a spreadsheet is a handy way to see the impact on results before and after a change.</p>
<p>We are starting to see more sophisticated forms of undo emerge. Versioning is one example.  My favorite versioning service is <a href="http://www.dropbox.com">Dropbox</a>.  Dropbox tracks every little micro change you make when saving files and allows you to restore previous states with a few clicks.  Google Docs provides similar versioning.</p>
<p>And if you think about it, every time you make a backup of your system or files, you’re also creating an undo option. The ability to instantly jump out of a corner you’ve been painted into is very empowering.</p>
<p><strong>The best part about undo is its safety net nature.</strong> It lets you take greater risks in your workflows and focus on moving forward without the fear that you can’t go back.</p>
<p>Being calculating is good, but it’s also an impediment to progress.</p>
<h2 id="cutcopypasteinyourworkflow">Being practically efficient with cut/copy/paste</h2>
<p>I don’t think you can overuse cut/copy/paste.  It can be used to transfer anything from a single character of text to an entire novel rich with photos and fancy fonts.</p>
<p>Here are a few ways that you can wring a few more droplets of value out of cut/copy/paste:</p>
<ul>
<li><strong>Avoid human RAM syndrome</strong> – a condition where people temporarily and unnecessarily store numbers and text in their heads while working at a computer.  If you need to compare a number to another, copy one number into a little text file and align it next to the other window.  You’ll be amazed at how much clearer your mind is when doing this.</li>
</ul>
<ul>
<li>Use <strong>clipboard history tools</strong>.  I personally use LaunchBar’s clipboard history.  Being able to copy several disjointed chunks of text and then paste them in any order is a boon to productivity.  I use it like crazy when writing web content with links.</li>
</ul>
<ul>
<li><strong>Combine cut/copy/paste with TextExpander</strong>.  Use the clipboard variable to insert the last-copied bit of text in a snippet.</li>
</ul>
<p><strong>Here’s an example of how I use the last two points to speed up writing in MultiMarkdown:</strong></p>
<p>I do almost all of my web writing in <a href="http://fletcherpenney.net/multimarkdown/">MultiMarkdown</a>.  I use TextExpander and LaunchBar to insert links really fast.  It’s something I do a lot, so I wanted the most streamlined method possible.</p>
<p>Before I found MultiMarkdown, I was accustomed to normal blog editors and word processors – both of which let you highlight a word, then click some button to paste a link.  In a lot of ways, this feels more natural to me because I usually don’t know what I want to hyperlink until I’ve written it.</p>
<p>I wanted to replicate this process in MultiMarkdown.  Here’s how I do it:</p>
<p>For starters, set up a TextExpander snippet that expands to:</p>
<pre>[%clipboard](%|)</pre>
<p>I use “mmc” as my snippet.</p>
<ol>
<li>Type text that you want to hyperlink (happens naturally as you write)</li>
<li>Go copy the URL (e.g. from your web browser)</li>
<li>Come back to your text, and select the part you want to hyperlink, and copy it (Command-C).</li>
<li>Type “mmc” – to trigger the TextExpander snippet. This turns “some text” into [some text]() and puts your cursor between the ().</li>
<li>Finally, I just drop the link in the slot using LaunchBar’s clipboard history (Command-\).</li>
</ol>
<p>It will blow your mind how fast this goes in practice:</p>
<ol>
<li>Select text</li>
<li>Copy URL</li>
<li>Type “mmc”</li>
<li>Paste URL</li>
</ol>
<p>I have similar snippets set up to bold and italicize text:</p>
<pre><code>mmb: **%clipboard**
mme: *%clipboard*</code></pre>
<p>Select, copy, type snippet.</p>
<p>Again, I think it’s more natural to highlight something you’ve already typed, then apply formatting.  It’s like painting the text with a brush.</p>
<h2 id="more">Assume nothing, trust no one</h2>
<p>Okay, really just that first part. I guess I got carried away.</p>
<p>I would encourage you to ponder more of the mundane tools in your workflow toolbox. <strong>Spend some time taking nothing for granted</strong>.  You might find a whole new set of workflow condiments that have been hiding right in your cupboard.</p>
<p>If you have any stories of how you made something mundane into something remarkable (even if it is totally specific to your workflow), share it in the comments.</p>
