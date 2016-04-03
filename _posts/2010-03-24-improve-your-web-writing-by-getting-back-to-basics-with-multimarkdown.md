---
layout: post
title: Improve your web writing by getting back to basics with MultiMarkdown
redirect_from: /home/2010/03/24/improve-your-web-writing-by-getting-back-to-basics-with-multimarkdown/index.html
---
<p>I recently discovered a great new tool for web writers called <a href="http://fletcherpenney.net/multimarkdown/">MultiMarkdown</a> thanks to a recent <a href="http://macpowerusers.com/2010/03/mpu-023-workflows-with-merlin-mann/">Mac Power Users podcast</a>.
Now on first glance, you’ll probably think that this is too nerdy/geeky for the common person, but it’s actually a gift to anyone who’s been troubled by the fact that it’s so darn hard to convert anything to clean HTML. If you’ve never had that thought, or never had the need to convert a document to HTML, you can safely move on. If you have, read on…</p>
<p>If you’re a blogger, you’ve probably experimented with different ways of composing your blog posts.  Perhaps you’ve tried word processors like Microsoft Word or other desktop apps because you don’t like editing in a browser (like me). Writing in these apps works fine (assuming you aren’t distracted by the superfluous amount of commands bordering your page), but for all the technology and ubiquity of the Web,  converting your composition to something that can be rendered on a web page is still a royal pain.</p>
<p>Microsoft Word, for example, is designed to generate an inordinate amount of additional HTML coding around even the simplest of HTML documents.  There was probably less code running the Apollo space craft than is contained in a Word-generated HTML file. And of course, once pasted into your blog editor of choice, it <em>never</em> looks the same as it did in Word.</p>
<p>Maybe you’ve also tried composing in a simple text editor like TextEdit on your Mac or even Notepad on your PC.  Again, the writing part is easy, but now you’re stuck having to type long HTML commands like anchors, breaks, paragraph codes, etc. over and over.  And if you need to create a table, just forget it.</p>
<p>The underlying problem is that you find yourself playing the role of a programmer at least as much as a writer. This can be a major distraction that ultimately affects the quality of your work.</p>
<p>MutltiMarkdown eases the woe of the common web writer by providing simple, intuitive shortcuts for HTML codes.  For example, a table can be created simply using the pipe symbol like this:</p>
<pre><code>|col 1|col 2|
|--|--|
|abc|def|</code></pre>
<p>The above bit of code turns into</p>
<table>
<col></col>
<col></col>
<thead>
<tr>
<th>col 1</th>
<th>col 2</th>
</tr>
</thead>
<tbody>
<tr>
<td>abc</td>
<td>def</td>
</tr>
</tbody>
</table>
<p>I really like the way MutltiMarkdown handles links too.  There are several different ways of typing a link.  The simplest is like this:</p>
<pre><code>[Google](http://www.google.com)</code></pre>
<p>If you have long URLs, you may want to use this footnote-like method:</p>
<pre><code>[Google][1]
[1]: http://www.google.com</code></pre>
<p>The second alternative above has the advantage of keeping your text even cleaner, so you don’t have long URLs cluttering up your paragraphs.  You can put the hyperlink number anywhere in your file (I like putting them in a stack at the bottom.)</p>
<p>Both methods generate the same result: <a href="http://www.google.com">Google</a>.</p>
<p>So in summary, with MultiMarkdown, you can focus on your writing, not your coding.  When you’re done drafting, you simply convert your text file to HTML using a script provided on the <a href="http://fletcherpenney.net/multimarkdown/">MultiMarkdown</a> website.</p>
<p>If you’re a Mac user, you’re in even more luck. Fletcher Penney, the author of MultiMarkdown, created <a href="http://fletcherpenney.net/multimarkdown/multimarkdown_drag_and_drop/">several apps</a> that let you simply drag and drop your MultiMarkdown text file to create HTML, RTF, and other formats.</p>
<p>Even better, there are a number of Mac apps that are compatible with MultiMarkdown like <a href="http://www.literatureandlatte.com/scrivener.html">Scrivener</a>, <a href="http://www.omnigroup.com/products/omnioutliner/">OmniOutliner</a>, and <a href="http://notational.net/">Notational Velocity</a>.</p>
<p>In summary, if you use MultiMarkdown to write your HTML-bound documents, you can</p>
<ol>
<li>Write in a simple text editor using the MultiMarkdown syntax.</li>
<li>Save the file like file.txt (or whatever file name you prefer).</li>
<li>Drag the text file to one of the apps that automatically translates the MultiMarkdown format into HTML.</li>
<li>Copy your HTML to your favorite blog editor (or wherever you want it).</li>
</ol>
<p>Let me know if you have any questions on MultiMarkdown or how you’re using it in the comments.</p>
<p>Also, be sure to check out the original <a href="http://daringfireball.net/projects/markdown/">Markdown</a> page and <a href="http://michelf.com/projects/php-markdown/extra/">PHP Markdown Extra</a> for extra syntax tips.</p>
