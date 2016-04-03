---
layout: post
title: How to turn Hazel into a security guard for your Mac
redirect_from: /home/2010/07/27/how-to-turn-hazel-into-a-security-guard-for-your-mac/index.html
---
<p><em>This is part 2 of a 3-part series on Mac data security: <a href="http://www.practicallyefficient.com/tag/perils-of-persistent-data/">Perils of persistent data</a>.</em>
<p style="text-align: center;">* * *</p>
<p><a href="/img/hazel.php"><img class="size-full wp-image-774 alignright" title="hazeltitle" src="/img/hazeltitle.png" alt="" width="217" height="254" />Hazel</a> is one of the most boring, yet amazing applications for the Mac in existence. Even if used lightly, it can yield huge benefits to anyone that likes to be more organized without having to lift their own fingers.</p>
<p>I’ve talked before about how I use Hazel geekery to <a href="http://www.practicallyefficient.com/2010/05/19/my-multimarkdown-writing-workflow-with-launchbar-and-hazel/">automate web writing</a>. I’m also using it to securely delete files that have sensitive financial data.</p>
<p>For me, Hazel is more than a maid. She’s a security guard too.</p>
<p>In this post, I'll discuss how I use Hazel to securely delete</p>
<ul>
<li>Quicken files</li>
<li>Files with a color label</li>
<li>Files copied to a specific folder</li>
<li>Files containing specific words</li>
</ul>
<p><!--more--></p>
<h2 id="shreddingquickendownloadfiles">Shredding downloaded Quicken files</h2>
<p>I use Quicken Essentials for Mac (QEM) to keep up with my basic personal finance information.  By default, I have all of my web browsers set to download files to my Downloads folder.  So every time I let QEM download account information, it puts a QFX file inside Downloads.</p>
<p>For a while, I didn’t think anything of this.</p>
<p>One day, I decided to crack open one of those files to see what is inside.  (They can be viewed in any text editor.)  I was a little surprised to see that each one contained a full account number for the associated account.</p>
<p>I don’t really care that much about someone seeing the balances or transactions in my checking account, but I’d rather not leave a trail of account numbers lingering on my hard drive.</p>
<p>Before I used Hazel, I had been letting these QFX files pile up in my Downloads folder – along with a lot of other junk.</p>
<p>It’s really easy to configure Hazel to clean out your Downloads folder on a regular basis. Just like any other folder, when Hazel “deletes” files, it simply moves the files to the Trash folder on your Mac.  It doesn’t permanently remove the files from your system.</p>
<p>For permanent file and folder removal, the primary option Hazel offers is secure deletion of the Trash folder contents (all at once).</p>
<p><a href="/img/hazel-securetrash-pe.png"><img class="aligncenter size-full wp-image-758" title="hazel-securetrash-pe" src="/img/hazel-securetrash-pe.png" alt="" width="595" height="296" /></a></p>
<h2 id="effectingtheselectivesecuredelete">Effecting the selective, secure delete</h2>
<p>Personally, I don’t want Hazel to do a secure delete each time it empties my Trash folder, mainly because it adds run time. But really, it just reeks of OCD, overkill, hyper-paranoia behavior.  And sometimes I send a lot of media files to the Trash at once, so I don’t want the system unnecessarily chewing away on those.</p>
<p>I wanted a more surgical zapping approach (because that’s not obsessive at all, right?) where I single out specific files that I want to be securely deleted.  Turns out, it’s easy.</p>
<p>Instead of telling Hazel to move “sensitive” files to the Trash, I tell it to fire off a super-simple little shell script that I stumbled across in a <a href="http://www.noodlesoft.com/forums/viewtopic.php?f=3&amp;t=384&amp;start=0&amp;hilit=secure">thread</a> over at Hazel's forum.</p>
<pre><code>srm -frm $1</code></pre>
<p>Here’s an explanation of what this command does:</p>
<ul>
<li>srm is the secure remove command common to all Unix and Unix-like systems, including Macintosh.</li>
<li><em>f</em> forces the removal of the file (no questions asked).</li>
<li><em>r</em> tells srm to be recursive (remove contents of subfolders).</li>
<li><em>m</em> is the “medium” security option.  It tells srm to do a 7-pass delete, meaning that it wipes over the file 7 times – like a cross-cut paper shredder.  Most of the time, I think this is plenty.  If you leave off m, srm will do a 35-pass delete and take a lot longer to run.</li>
<li>$1 represents the file(s) to be shredded</li>
</ul>
<p><strong>Now is a good time to issue the standard secure delete disclaimer: there is no undo on this action. It will delete the file permanently. No going back. But remember, that’s the goal here, right?</strong></p>
<p>If you’re comfortable with those powerful, little letters above, all you have to do is paste the command into the “Run shell script” box in the “Do the following” section of your Hazel rule.</p>
<p><a href="/img/hazel-shredqfx-pe.png"><img class="aligncenter size-full wp-image-762" title="hazel-shredqfx-pe" src="/img/hazel-shredqfx-pe.png" alt="" width="585" height="267" /></a></p>
<p>This rule instructs Hazel to zap any file with a QFX extension about 2 minutes after it lands in the Downloads folder.  With Hazel in control, I no longer have to even think about getting rid of these pesky files. They just go away – securely.</p>
<h2 id="securelyshreddingmiscellaneousfilesthatlandinyourdownloadsfolder">Securely shredding miscellaneous files that land in your Downloads folder</h2>
<p>I routinely download bank statements, and just like their paper ancestors, they have my full account number printed clearly at the top of the page.</p>
<p>Unlike the Quicken files I just mentioned, most of the financial statements I download are in PDF format.  I don’t want to set up a rule to annihilate every PDF file in my Downloads folder since I work with tons of other non-sensitive PDF.</p>
<p>The naming scheme banks use for downloadable statements aren’t consistent either.  I’ve decided that the best way to get rid of PDF containing account numbers is simply mark them for execution using a gray color label.</p>
<p><a href="/img/hazel-shredgray-pe.png"><img class="aligncenter size-full wp-image-765" title="hazel-shredgray-pe" src="/img/hazel-shredgray-pe.png" alt="" width="585" height="244" /></a>I like the color label approach because I can use it on more than one file at once.  If I download, say, 3 statements, I can quickly color them for death by selecting all 3, then choosing the gray color label under Finder’s File menu. (I would love to find a keyboard shortcut for bringing up the color label selector, but I haven’t yet.)</p>
<h2 id="usinghazeltocreateashredbin">Using Hazel to create a shred bin</h2>
<p>Hazel can watch any folder on your Mac and do all sorts of things as files are added and changed. You can take advantage of Hazel’s voyeuristic ways by creating a folder specifically for shredding any files that land in it. Think of it like the paper shredder sitting next to your regular trash can at home.</p>
<p>We can use the same simple shell script we used above to create a rule for zapping anything we drag and drop into our Shred folder:</p>
<p><a href="/img/hazel-shredany-pe.png"><img class="aligncenter size-full wp-image-781" title="hazel-shredany-pe" src="/img/hazel-shredany-pe.png" alt="" width="585" height="289" /></a></p>
<p>The Shred folder approach has the advantage of being available anywhere.  I put a shortcut to mine in my Finder sidebar so that I can simply drag files into it from any folder.</p>
<p>Remember, the Shred folder is an abyss.  Anything you toss into it (intentionally or not) is gone for good.</p>
<p><a href="/img/hazel-shred-folder-sidebar-pe.png"><img class="size-full wp-image-768  aligncenter" title="hazel-shred-folder-sidebar-pe" src="/img/hazel-shred-folder-sidebar-pe.png" alt="" width="131" height="122" /></a></p>
<h2 id="securedeletingbasedonfilecontents">Secure deleting based on file contents</h2>
<p>Suppose you bank with Bank ABC.  Every statement you download from Bank ABC’s site has their name on it.</p>
<p>For a really hands-off solution, you could create a Hazel rule to annihilate any file containing Bank ABC maybe 5 or 10 minutes after being downloaded.  This would give you plenty of time to copy it to a secure location or do something else with it.</p>
<p><a href="/img/hazel-shredifcontains-pe.png"><img class="aligncenter size-full wp-image-766" title="hazel-shredifcontains-pe" src="/img/hazel-shredifcontains-pe.png" alt="" width="585" height="312" /></a></p>
<h2 id="nextup">Next up</h2>
<p>In the next and final part of this series, I’ll describe the process I use for long-term storage of sensitive files.</p>
