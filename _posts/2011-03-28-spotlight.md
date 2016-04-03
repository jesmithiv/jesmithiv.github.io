---
layout: post
title: The powerful, mystical Spotlight. On steroids.
redirect_from: /home/2011/03/28/spotlight/index.html
---
<p>Your Mac comes with an extraordinary search system called Spotlight. It’s so great, so fast, so near perfection, and <a href="http://www.youtube.com/watch?v=N-2C2gb6ws8">oh so coveted</a> by certain unnamed Apple competitors.
How on earth can it be so good, you ask? Well, it’s hard to say. But some have speculated that it runs on only the purest tears collected from Apple’s most prized unicorns. Alas, no one has ever seen one of these creatures, which are said to be stabled in a secret location outside of Cupertino.</p>
<p>Until someone – most likely a Gizmodo reporter – finds that stable, I’m okay just calling it magic and using it to find stuff really fast.</p>
<h2 id="spotlightonsteroids">Spotlight on steroids</h2>
<p>I have to confess that until very recently, I didn’t know you could include file attributes in Spotlight searches.  When I found out, it blew my mind, and I began to scour the web for tips and tricks.</p>
<p>This post is more or less what I found. I’m sure there’s more.  Addend me in the comments.</p>
<h2 id="fileattributes">File attributes</h2>
<p>Your Mac stores a lot of metadata for your files. Just do ‘Get Info’ on a file and take a look at all that stuff.  Much of those attributes are fair game in Spotlight searches. Simply include an attribute in a Spotlight search followed by a colon (:).</p>
<p><code>AttributeType:attribute</code></p>
<p>Here are a few common attribute types:</p>
<ul>
<li>Name (i.e. the file name)</li>
<li>Kind (e.g. App, Text, PDF, Spreadsheet, Document, Image, Movie, Music, Folder, Message, and more)</li>
<li>Modified</li>
<li>Created</li>
</ul>
<p>Special file types like music have even more. You can use things like “by” to search music by artist. Experiment; explore. You can’t hurt anything.</p>
<p>I find that just using the name attribute is a powerful way to narrow searches.  It cuts out any hits that come from matching content.  I usually remember some piece of file names, and I almost always know what kind they are.  Like, say I was trying to track down my Nikon manual:</p>
<p><code>name:nikon kind:pdf</code></p>
<p>That's probably enough to take me straight there.</p>
<h2 id="powerfuldatesearches">Powerful date searches</h2>
<p>The ‘Modified’ and ‘Created’ attributes can accept all kinds of dates.  You can use things like:</p>
<ul>
<li>Yesterday</li>
<li>Today</li>
<li>Tomorrow (kidding)</li>
<li>To search before a date, &lt;1/1/2011</li>
<li>To search after a date, &gt;1/1/2011</li>
<li>To search in a date range, 1/1/2011-3/13/2011</li>
</ul>
<p>Suppose you wanted to see every text file you modified in the month of March containing the word “monkey”:</p>
<p><code>monkey kind:text modified:3/1/2011-3/31/2011</code></p>
<h2 id="booleanstuffandmore">Boolean stuff and more</h2>
<p>Like a web search field, Spotlight supports boolean operators like AND, OR, and NOT.  You can also use a minus sign (-) to exclude terms.  For example:</p>
<p><code>chocolate recipes -coconut</code></p>
<p>Use quotation marks to enclose phrases and parentheses to enclose search terms:</p>
<p><code>chocolate AND "peanut butter" NOT (almonds OR coconut)</code></p>
<h2 id="othertips">Other tips</h2>
<ul>
<li>Check your Spotlight Preferences if you don’t see the files you expect to see when doing searches.  You may be excluding that file type from Spotlight’s index.</li>
<li>Spotlight <a href="http://www.practicallyefficient.com/2010/12/23/math-on-a-mac/">does math</a> too. Just type an expression, and it’ll evaluate it for you right there.</li>
</ul>
<h2 id="otherarticlesonspotlightsearch">Other articles on Spotlight search</h2>
<ul>
<li><a href="http://reviews.cnet.com/8301-13727_7-20011417-263.html">Enhance Spotlight searches with hidden features</a></li>
<li><a href="http://docs.info.apple.com/article.html?path=Mac/10.5/en/15155.html">Specifying criteria in the Spotlight search field</a></li>
<li><a href="http://d-bitblog.blogspot.com/2010/08">Spotlight Search by File Attributes</a></li>
</ul>
<p><script type="text/javascript">// <![CDATA[
window.onload = function(){var div = document.getElementById('contentdiv'),oldscroll = 1439;div.scrollTop = oldscroll;}
// ]]</p>
