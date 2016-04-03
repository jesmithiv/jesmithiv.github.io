---
layout: post
title: Using TextExpander and Notational Velocity for fast, efficient writing
redirect_from: /home/2010/07/13/using-textexpander-and-notational-velocity-for-fast-efficient-writing/index.html
---
<p>I’ve talked separately about <a href="http://www.smileonmymac.com/TextExpander/">TextExpander</a> and <a href="http://notational.net/">Notational Velocity</a> in the past, but it’s worth noting that the two really go well together.
My primary use of Notational Velocity is drafting blog posts and other articles.  For me, it’s basically a stripped down, no-nonsense word processor.  A better term would be word-taker or word-holder.  I write, and it quietly listens without tempting me to do a bunch of fancy formatting.</p>
<p>TextExpander lubricates the writing process even more by instantly expanding longer chunks of text that I would otherwise have to mindlessly pound out over and over.</p>
<p>I think it’s always best in life to focus on creating new, unique things and not spin your wheels performing tasks that are better handled by things without a cerebrum. TextExpander is a great way to automate  repetitious writing. By putting it in charge of the rote and the mundane, you free up your fingers for more creative expression.</p>
<p>Here are a few simple ways I’m using TextExpander with Notational Velocity…</p>
<p><!--more--></p>
<h2 id="fasternotecreationandsearch">Faster note creation and search</h2>
<p>If I’m starting a draft for this blog, I always start the note title with “draft [pe]”.  Since I have Notational Velocity set up to store notes as individual text files, this lets me sort my notes alphabetically to see all my drafts at a glance in Finder or make use of Spotlight and <a href="http://www.obdev.at/products/launchbar/index.html">LaunchBar</a> to search and retrieve files outside of Notational Velocity.</p>
<p>The [pe] part essentially creates a unique tag that lets me search only for practically efficient posts in the Notational Velocity search field.  The term [pe] is not likely to appear in the body of any other notes; it’s only in the title of my practically efficient posts. I got the idea of creating unique text in note titles after seeing Merlin Mann's <a href="http://www.kungfugrippe.com/post/453204090/q-trick">q trick</a>.</p>
<p>I’m a big believer in minimizing the friction between thinking and doing. So I use TextExpander to create that first little bit for me. If I type dpe, it expands to “draft [pe]” and I can then type a quick title for my note. This is much faster, and more importantly, less distracting than having to fumble for the [] keys.</p>
<h2 id="moreefficientwebwriting">More efficient web writing</h2>
<p>I’ve talked about MultiMarkdown in <a href="http://www.practicallyefficient.com/tag/multimarkdown/">other posts</a>.  Since I write almost exclusively in MultiMarkdown in Notational Velocity, I naturally take advantage of TextExpander to make the process even more efficient.</p>
<p>Here are a few examples of TextExpander snippets I use for MultiMarkdown syntax along with what they create:</p>
<ul>
<li><em>mma1</em>
<pre>[%|][]</pre>
<p>Creates a MultiMarkdown anchor (link) using the [] syntax and positions my cursor in the first bracket.</li>
<li><em>mma2</em>
<pre>[%|]()</pre>
<p>Creates a MultiMarkdown anchor (link) using the () syntax and positions my cursor in the first bracket.</li>
<li><em>mmap</em>
<pre>[%|](%clipboard)</pre>
<p>Creates a MultiMarkdown anchor (link) using the () syntax, pastes my clipboard between the (), and positions my cursor in the first bracket. I use this one constantly. It lets me quickly create a link if I’ve already copied the URL to my clipboard.</li>
<li><em>mmimg</em>
<pre>![alt text](/path/to/img.jpg "Title")</pre>
<p>Creates the MultiMarkdown image syntax.</li>
<li><em>mmlinks</em> - This one creates a vertical list link numbers:</li>
</ul>
<pre>        [1]:
        [2]:
        [3]:
        [4]:
        [5]:
        [6]:
        [7]:
        [8]:
        [9]:</pre>
<p>I usually put them at the end of a draft in which I’m using the [][] link syntax (e.g. [My Link][1] for a cleaner “foot note” style. This lets me quickly add up to 9 links before having to type out more numbers. The MultiMarkdown HTML converter will ignore any of these at the end that aren’t in use.</p>
<p><strong>Update... here's another:</strong></p>
<ul>
<li><em>mmc</em>
<pre>[%clipboard](%|)</pre>
<p>Often, I want to hyperlink a word or phrase I've already typed in my text editor. I use this TextExpander snippet along with LaunchBar's clipboard history to mimic the process of inserting a hyperlink in a blog editor like WordPress. The steps I follow are below. It's actually really fast once you do it a couple of times. Your fingers never leave the keyboard.</li>
</ul>
<ol>
<li>Copy the URL from your web browser (or wherever it is).</li>
<li>Highlight the text word you want to hyperlink in your text editor.</li>
<li>Copy the word with CMD+C.</li>
<li>Type <em>mmc</em> over the highlighted word. This will replace "your word" with [your word]() and put your cursor between ().</li>
<li>Finally, bring up LaunchBar's clipboard history with CMD+\ and arrow down to the URL you copied. Release the keys to insert the URL between the ().</li>
</ol>
<h2 id="otherhtml">Other HTML</h2>
<p>I also use the predefined group of HTML snippets that comes with TextExpander to quickly expand other HTML codes if necessary.</p>
<p><em>Please share your own tips and tricks for using TextExpander with Notational Velocity or other general writing.</em></p>
