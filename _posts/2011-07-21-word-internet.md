---
layout: post
title: Think of Microsoft Word as the internet
redirect_from: /home/2011/07/21/word-internet/index.html
---
<p>Life has been very good to web writers who prefer to plain text. Just in the last year, we’ve seen a number of great tools that make creating HTML from plain text (specifically, Markdown) easy peasy.</p>
<p>As prevalent as the web is, however, there are still lots (read: LOTS) of people who still have to ship their writing in love-it-or-hate-it Microsoft Word. Many publishers know <em>nothing</em> other than Word, and try as you might, they won’t change.</p>
<p>Whenever I write articles for newsletters and other publications, editors expect me to send my words in Word—even when the articles will ultimately be published online (in HTML). It’s a silly state of affairs, but it’s the world today.</p>
<p>As always, adaptation is better than inaction. Fortunately, there’s a relatively easy way to write in Markdown but ship in Word.</p>
<p>When it comes to writing, I think of Word as the internet. It’s a destination, not a vehicle.</p>
<p>I’ll show you how to get there, but only after I satisfy my compulsion to gush about Markdown.</p>
<h2 id="markdownmonogamy">Markdown monogamy</h2>
<p>I’m at the point now where I can’t <em>not</em> write in gloriously naked plain text. In fact, it’s probably not a stretch to say that this site wouldn’t exist without <a href="http://daringfireball.net/projects/markdown/">Markdown</a>. Seriously. When I discovered John Gruber’s Markdown (and Fletcher Penney’s <a href="http://fletcherpenney.net/multimarkdown/">MultiMarkdown</a> variant), the volume of what I wrote exploded.</p>
<p>Virtually everything I’ve written in the last two years has its roots in plain text. And trust me, kids; it’s not some obsession with old school nerdery. Plain text is just infinitely more practical for at least three good reasons, which are enough for me.</p>
<p><strong>First, it’s everywhere:</strong></p>
<p>My life doesn’t allow me to sit in front of a full keyboard all day. But as long as my incubating ideas are in plain text, I can work on them any time life offers me the chance. That’s because I keep all of my drafts in Simplenote and Dropbox.</p>
<p>As long as I have an iOS device handy, I can proof and polish an article while I sit in the waiting room of a behind-schedule doctor’s office. I can jot down ideas as I read in a coffee shop. I can collect hyperlinks from my mobile RSS reader and put them directly into drafts. All without ever touching my Mac.</p>
<p>Try pulling off that mobile workflow in Word.</p>
<p><strong>Second, it causes me to <em>write</em>:</strong></p>
<p>I’ve said it before; I’ll say it again: Word is not a writing application. It’s a desktop publishing application. When I start a writing project of any size in Word, it feels like I’m starting to build a house by first worrying about wall colors.</p>
<p>With its ticker tape of attention-sabotaging features, Word constantly gives you a finish line illusion.</p>
<p>Words aren’t worthy of cosmetics until they say something. More importantly, each second you spend fiddling with the aesthetics of your document is a second spent not writing. Accumulated over just a few days, that can be a tremendous number of seconds.</p>
<p><strong>Third, it’s practically invincible:</strong></p>
<p>Plain text doesn’t die. Applications don’t drop support for plain text. Plain text is <em>the</em> most portable, <em>the</em> most searchable, <em>the</em> most light weight medium for your writing.</p>
<p>Okay, done gushing.</p>
<h2 id="goingfrommarkdowntoword">Going from Markdown to Word</h2>
<p>You don’t hear people talk about it a lot, but it’s quite possible—and relatively straightforward after some moderate geeking around.</p>
<p>I’ll walk you through these main steps:</p>
<ol>
<li>Install MultiMarkdown</li>
<li>Convert (Multi)Markdown to open document format (FODT)</li>
<li>Save FODT as DOC</li>
</ol>
<h2 id="step1:installmultimarkdown">Step 1: Install MultiMarkdown</h2>
<p>See <a href="http://fletcherpenney.net/multimarkdown/download/">Fletcher Penney’s site</a> for more details on downloading and installation. Specifically, you’ll need <code>mmd2ODF.pl</code>, which is included in the main package.</p>
<p>I recommend putting your MultiMarkdown things in <code>~/Library/Application Support/MultiMarkdown/</code>.</p>
<h2>Step 2: Convert to FODT</h2>
<p>I’m going to talk about two ways of using Fletcher’s <code>mmd2ODF.pl</code> script: 1) geekier 2) less geeky.</p>
<p><strong>Geekier</strong></p>
<p>If you’re handy in Terminal, doing the conversion is easy. Just modify ~/.bash_profile so that it has this line:</p>
<p><code>export “PATH=/Users/[YOUR HOME FOLDER NAME]/Library/Application Support/MultiMarkdown/bin:$PATH”</code></p>
<p>And, of course, replace [YOUR HOME FOLDER NAME] with the name of your home folder.<a id="fnref:1" class="footnote" title="see footnote" href="#fn:1">[1]</a> After reloading <code>.bash_profile</code>, you should be able to simply type:</p>
<p><code>mmd2ODF.pl yourmarkdownfile.txt</code></p>
<p>You’ll see <code>yourmarkdownfile.fodt</code> appear in the same folder.</p>
<p><em><strong>Tip</strong>: create a short TextExpander snippet to expand mmd2ODF.pl for you.</em></p>
<p><strong>Less geeky</strong></p>
<p>Just so you have no excuses, I’ll give you service that does all that Terminal business for you as long as you have MultiMarkdown installed in <code>~/Library/Application Support/MultiMarkdown/</code> like I said above.</p>
<p>Instructions:</p>
<ol>
<li>Download <a href="http://www.practicallyefficient.com/files/ConvertToODF.zip">ConvertToODF.zip</a> and unzip it</li>
<li>Copy ConvertToODF.workflow to <code>~/Library/Services</code></li>
<li>Open ConvertToODF.workflow in Automator, and replace <code>[YOUR HOME FOLDER NAME]</code> with the name of your home folder.<a id="fnref:2" class="footnote" title="see footnote" href="#fn:2">[2]</a></li>
<li>Save your changes</li>
</ol>
<p><img style="display: block; margin-left: auto; margin-right: auto;" title="convert-to-odf-pe.png" src="/img/convert-to-odf-pe.png" border="0" alt="Convert to odf pe" width="527" height="322" /></p>
<p>To use, simply select a Markdown file in Finder and run the service (Finder &gt; Services). Out should pop a .fodt file.</p>
<p>I recommend creating a keyboard shortcut for this service if you’re going to use it a lot. Go to System Preferences &gt; Keyboard &gt; Keyboard Shortcuts, and look in the Services section.</p>
<p><img style="display: block; margin-left: auto; margin-right: auto;" title="services-shortcut-pe.png" src="/img/services-shortcut-pe.png" border="0" alt="Services shortcut pe" width="527" height="231" /></p>
<h2 id="workingwiththefodtfile">Step 3: Saving FODT as DOC</h2>
<p>FODT is an open document format. The “F” is for flattened. Not important.</p>
<p>You can’t open FODT in Word, but you <em>can</em> open it in <a href="http://www.openoffice.org/">OpenOffice.org</a> or <a href="http://www.libreoffice.org/">LibreOffice</a>. Both are free, and both allow you to save in a Word format (.doc).</p>
<p>LibreOffice opens FODT automatically, but OpenOffice.org requires an add-on. I followed <a href="http://fletcher.github.com/peg-multimarkdown/index#multimarkdownandopendocument">Fletcher’s simple instructions</a> for installing the add-on in OpenOffice.org, and it works great.</p>
<p>Just open FODT in either program and save it as DOC. Done.</p>
<h2 id="whythisisworthyourtime">Why this is worth your time</h2>
<p>FODT preserves virtually all of the formatting you create in (Multi)Markdown. Things like italicized text, bold text, headings, and bulleted lists, appear as they should. That’s important because it minimizes the effort needed to polish the text at the finish line. In fact, you may not have to do anything at all.</p>
<p>Spending just a little time on the back end to convert Markdown to FODT then save FODT as DOC is a small price to pay for the efficiency you’re gaining during the plain text writing phase.</p>
<div class="footnotes">
<hr />
<ol>
<li id="fn:1">
<p>H/t to Brett Terpstra for help on this.</p>
<p><a class="reversefootnote" title="return to article" href="#fnref:1"> ↩</a> </li>
<li id="fn:2">
<p>For example, if your home folder is called Sam, the path would be <code>/Users/Sam/Library/…</code></p>
<p><a class="reversefootnote" title="return to article" href="#fnref:2"> ↩</a> </li>
</ol>
</div>
