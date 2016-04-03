---
layout: post
title: Financial statements, TextExpander, Hazel, and you
redirect_from: /home/2011/02/11/financial-statements-textexpander-hazel-and-you/index.html
---
<p>Maybe one day someone will invent a securer-than-email system for delivering financial statements directly to my computer, but we’re obviously not there yet. Not even close.
So for now, I’m stuck visiting each company’s web site to download the PDFs myself. It’s not fun, but I think it’s necessary to have good personal financial records in a time when banks are made more of 1s and 0s than brick and mortar.</p>
<p>Downloading PDF statements yourself is one of modern life’s menial, rote activities. It’s certainly not worthy of a blog post – unless of course it’s about how to make it better and more fun.</p>
<p>And, actually, that’s just what I’ve done using 1Password, TextExpander, and Hazel.</p>
<h2 id="firsttheneed">First, the need</h2>
<p>Around the 5th of each month, I download financial statements by visiting each site individually. Downloading isn’t that bad, especially if you use 1Password to unlock all those doors for you.<a id="fnref:f1" class="footnote" title="see footnote" href="#fn:f1">1</a></p>
<p>But the downloading itself introduces a potentially productivity-halting friction: Each statement lands in my downloads folder with different, often meaningless name (e.g. “estatement.pdf” or “justplaingobbledygook.pdf”).</p>
<p>Since my ultimate goal is to file these all into a single folder, I had to manually rename each one including a date (e.g. Bank ABC Savings 201101.pdf).</p>
<p>Typing this out each time was a big pain – a friction that sometimes caused me to skip it altogether.</p>
<p>Once renamed, I had to copy each PDF to its final destination: a folder called Statements inside a <a href="http://www.practicallyefficient.com/2010/07/28/create-a-file-vault-on-your-mac-with-secure-disk-images/">secure disk image</a>.</p>
<p>So long story short, 1Password was helping the workflow, but I was doing the same rote things over and over each month, and it sucked.</p>
<h2 id="automatingtheworkflowwithtextexpanderandhazel">Automating the workflow with TextExpander and Hazel</h2>
<p><strong>TextExpander</strong></p>
<p>Since I download most statements around the 5th of each month, I’m always getting last month’s statement.  In other words, if it’s February 5, I’m going to be renaming Bank ABC’s statement to “Bank ABC 201101.pdf.”</p>
<p>Fortunately, TextExpander is smart enough to do the date math for me (see <a href="http://blog.smilesoftware.com/2008/10/28/textexpander-date-and-time-math/">Smile’s tutorial</a>). TextExpander can subtract one month from the current date, then format it in all kinds of ways. In my case, I wanted the date to be “yyyymm”.</p>
<p>If you’re looking for an excellent return on your time, just have a look at the Date / Time Math menu in TextExpander sometime.</p>
<p><a href="/img/TextExpander-date-math-pe.png"><img class="aligncenter size-full wp-image-3324" title="TextExpander-date-math-pe" src="/img/TextExpander-date-math-pe.png" alt="" width="487" height="327" /></a></p>
<p>I now have a TextExpander snippet for each statement that I download. Example:</p>
<p><a href="/img/abc-savings-pe.png"><img class="aligncenter size-full wp-image-3325" title="abc-savings-pe" src="/img/abc-savings-pe.png" alt="" width="455" height="432" /></a></p>
<p>So now, instead of typing “ABC Savings 201101,” all I have to do is type .abc, and TextExpander does the math and typing for me.</p>
<h2 id="hazel">Hazel</h2>
<p>I have several <a href="http://www.noodlesoft.com/hazel.php">Hazel</a> rules that watch my downloads folder. One of them keeps an eye out for specific financial statements.  As soon as Hazel sees one, she sweeps it into my Statements folder.</p>
<p><a href="/img/hazel-move-statements-pe.png"><img class="aligncenter size-full wp-image-3326" title="hazel-move-statements-pe" src="/img/hazel-move-statements-pe.png" alt="" width="499" height="269" /></a></p>
<h2 id="recap">Recap</h2>
<ol>
<li>Download statement</li>
<li>Rename statement by typing snippet</li>
<li>Go do more enjoyable things</li>
</ol>
<p><em>If Hazel automation makes you happy, you should also visit David Sparks’s even more <a href="http://www.macsparky.com/blog/2009/6/3/sorting-and-moving-documents-with-hazel.html">sophisticated “statement” workflow with Hazel</a>.</em></p>
<div class="footnotes">
<hr />
<ol>
<li id="fn:f1">This part was a major nuisance before I started using <a href="http://agilewebsolutions.com/onepassword">1Password</a>.  Now, it’s not that bad: I just use a keyboard shortcut to trigger 1Password’s Go &amp; Fill search field, type the site name, and 1Password unlocks the door and lets me in.<a class="reversefootnote" title="return to article" href="#fnref:f1"> ↩</a></li>
</ol>
</div>
