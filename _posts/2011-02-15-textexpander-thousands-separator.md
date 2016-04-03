---
layout: post
title: Use TextExpander to format numbers with a thousands separator
redirect_from: /home/2011/02/15/textexpander-thousands-separator/index.html
---
<p>I often use <a href="http://www.obdev.at/products/launchbar/index.html">LaunchBar’s</a> calculator to do <a href="http://www.practicallyefficient.com/2010/12/23/math-on-a-mac/">calculations</a>, and I often need to paste the result into an email or document.  If the number is greater than 1,000, I have to add commas manually.
In other words, LaunchBar’s calculator spits out something like 43897909, and I have to make it 43,897,909.  Not a big deal for most people, I guess, but I have to do it over and over again for certain work.</p>
<p>I wondered if TextExpander could put the commas in there for me. Fortunately it can.</p>
<p><em>Aside:</em> Yes, this is <em>another</em> TextExpander post. Sorry. It’s actually Brett Terpstra’s fault.  His <a href="http://brettterpstra.com/textexpander-experiments/">shell script tricks</a> are like a song I just can’t get out of my head. But hey, if it keeps Lady Gaga out. . .</p>
<p>Anyway. . . I made a slight modification to one of Brett’s shell scripts using <a href="http://www.justskins.com/forums/format-number-with-comma-37369.html">some code I found</a>.</p>
<p>Here’s what it looks like:</p>
<pre><code>#!/usr/bin/env ruby -wKU

# get the clipboard using pbpaste
clip = %x{__CF_USER_TEXT_ENCODING=$UID:0x8000100:0x8000100 pbpaste}
# print it out comma separated
print clip.gsub(/(\d)(?=\d{3}+(?:\.|$))(\d{3}\..*)?/,'\1,\2')
</code></pre>
<p>Just paste that piece of elegant code into TextExpander:</p>
<p><a href="/img/TextExpander-commas-pe2.png"><img class="aligncenter size-full wp-image-3461" title="TextExpander-commas-pe" src="/img/TextExpander-commas-pe2.png" alt="" width="341" height="174" /></a></p>
<p>I set up a snippet (.fc) to trigger it. Now, when I do some math in LaunchBar, I can press Cmd-C to copy the answer to my clipboard, then type .fc wherever I want to put the answer with the commas already inserted. Works great, and saves me a ton of time.</p>
