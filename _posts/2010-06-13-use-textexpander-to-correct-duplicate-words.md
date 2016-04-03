---
layout: post
title: Use TextExpander to correct duplicate words
redirect_from: /home/2010/06/13/use-textexpander-to-correct-duplicate-words/index.html
---
<p>One of my favorite Mac programs is <a href="http://www.smileonmymac.com/TextExpander/index.html">TextExpander</a>.  I use it to expand shortcuts into full words and phrases, correct common misspellings, fill custom signatures in email, and even do cool tricks like <a href="http://e-musing.posterous.com/how-to-quickly-paste-just-text-from-your-mac">pasting text by typing an abbreviation</a>.
It’s an incredible tool that pays me back every time I use it by increasing my productivity and cutting down on mistakes.</p>
<p>Speaking of mistakes, one problem I seem to have over and over again is typing duplicate words (e.g. has has).  I think my fingers just move too fast.  It drives me nuts finding duplicate words in blog posts, emails, and anything I blast out to the world.</p>
<p><!--more-->It occurred to me recently that I could create a special snippet group in TextExpander specifically to deal with this problem.  Fortunately, Wikipedia had already published a nice list of <a href="http://en.wikipedia.org/wiki/Wikipedia:Lists_of_common_misspellings/Repetitions">common word repetitions</a>.  (How did we ever live without Wikipedia, right?)</p>
<p>The Wikipedia list is by no means comprehensive, but it's a great start. I was able to import most of what I needed by creating a text file in the following format:</p>
<pre>a a     a
an an   an
</pre>
<p>Basically, the first two words represent the TextExpander abbreviation, and the third word is what I want to end up with. A tab separates the abbreviation and final result.</p>
<p>After importing, I had to do some manual cleanup.  I found that I needed to have a space after each abbreviation.  For example, I don't want "on one sunny day" to turn into "on sunny day"  So it's important to distinguish between "on on" and "on on ".</p>
<p>I also set each snippet to adapt to the case of the abbreviation.  So if I try to start a sentence like "On on" it will get corrected to "On".</p>
<p>I'm so bad at this, it even came in handy while I was writing this post!</p>
<p>If you use TextExpander and want to add this as a group, just do the following:</p>
<ol>
<li>Download the group file that I created <a href="http://www.practicallyefficient.com/files/DuplicateWords.zip">here</a> and unzip on your Mac</li>
<li>Open TextExpander</li>
<li>Go to File &gt; Add new group from file</li>
<li>Select the DuplicateWords.textexpander file and click Open</li>
</ol>
<p>Feel free to share your own TextExpander tips and tricks.</p>
