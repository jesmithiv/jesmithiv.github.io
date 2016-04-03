---
layout: post
title: 'The right side of inertia: a backup workflow story'
redirect_from: /home/2010/10/29/the-right-side-of-inertia-a-backup-workflow-story/index.html
---
<p>What do these four things have in common?
<ol>
<li>You should save more money.</li>
<li>You should eat healthier foods.</li>
<li>You should tell your family you love them more often.</li>
<li>You should back up your data.</li>
</ol>
<p>Answer: They’re all things that people should do, but most don’t. Are most people fundamentally irrational? Maybe. But more likely, it’s just that adults don’t have anyone to make them do the things that they’re too inert to do on their on.</p>
<p>We all routinely trade long-term value for fleeting conveniences. It’s actually quite human and definitely predates the need for things like digital backups. The Greeks called it <a href="http://en.wikipedia.org/wiki/Akrasia">akrasia</a>, the state of acting against one’s better judgment.</p>
<p>Now, there’s no way I’m going to take on all four of the do’s up above (at least not today). So I’ll just address the last one.</p>
<p>I’m going to talk about characteristics of a good data backup plan, how I do it specifically, and <strong>most importantly</strong> why my workflow works for me: It fits into my life and creates a form of positive inertia. I know it works because I’ve been doing it long enough to be numb to it.</p>
<h2 id="characteristicsofagooddatabackupplan">Characteristics of a good data backup plan</h2>
<ul>
<li>It should be easy to execute so that it actually happens.</li>
<li>It should have redundancy (multiple copies of your data).</li>
<li>The frequency should balance practicality with your needs.</li>
<li>The process should be efficient in cost and time spent.</li>
<li>A copy of your data should be in at least two separate physical locations (e.g. home and office).</li>
<li>It should be easy to load your data onto a new computer if necessary.</li>
</ul>
<h2 id="coretoolsinmypersonalbackupstrategy">Core tools in my personal backup strategy</h2>
<ul>
<li>The cloud (Dropbox)</li>
<li>Time Machine + Time Capsule</li>
<li>Carbon Copy Cloner + USB hard drives</li>
</ul>
<p><a href="/img/backup-system-pe.png"><img class="aligncenter size-full wp-image-1889" title="backup-system-pe" src="/img/backup-system-pe.png" alt="" width="585" height="322" /></a></p>
<h2 id="dropbox">Dropbox</h2>
<p><a href="http://www.dropbox.com">Dropbox</a> syncs several folders containing my working documents.  It’s mostly text files, word processor files, spreadsheets, and PDFs. My 1Password keychain is also in Dropbox.</p>
<p>I find that Dropbox works damn near flawlessly to keep my files in sync. Benefits of Dropbox go well beyond being simply a backup system, but backing up is my focus today.</p>
<p>Benefits of Dropbox as a backup system:</p>
<ul>
<li>The basic (2 GB) version is free.</li>
<li>Versioning lets you easily restore files to any state in the last 30 days.</li>
<li>It’s fireproof (i.e. it’s offsite and can’t be destroyed by a local disaster).</li>
<li>Dropbox is very easy to implement and install on a new computer.</li>
<li>No manual intervention is required. It just works on its own.</li>
<li>Files can be accessed at any computer with an internet connection.</li>
</ul>
<p>Disadvantages of Dropbox as a backup system:</p>
<ul>
<li>Space is limited on the free version. More space = more money.</li>
<li>Items in shared folders can be deleted by others.</li>
<li>You can’t do a full system backup.</li>
<li>Requires internet connection (sometimes it’s sunny and there are no clouds).</li>
</ul>
<h2 id="timemachinetimecapsule">Time Machine + Time Capsule</h2>
<p>I run Time Machine hourly and back up over my WiFi network to a Time Capsule.  This gives me a running archive of all the data on my Mac – photos, music, files, application settings, etc.</p>
<p>Overall, I’ve been pleased with both Time Machine and the Time Capsule hardware. Both have run reliably for over two years. They’ve also been instrumental in getting me out of a few tight spots.</p>
<p>Benefits of Time Machine as a backup system:</p>
<ul>
<li>It will back up your entire hard drive.</li>
<li>Versioning allows restoration to previous states.</li>
<li>No manual intervention required. It just works on its own.</li>
<li>Data stays local (no cloud security issues).</li>
<li>Does not require internet connection.</li>
</ul>
<p>Disadvantages of Time Machine as a backup system:</p>
<ul>
<li>Space is limited to what’s available on the external hard drive you back up to.</li>
<li>By default Time Machine runs hourly. This bothers some people. It’s transparent to me, however.</li>
<li>You can’t create a bootable clone of your hard drive.</li>
<li>Restoring data to a new computer requires a few extra steps.</li>
<li>Does not sync multiple Macs.</li>
<li>Requires either a physical connection (e.g. USB) or wireless connection to Time Capsule.</li>
</ul>
<h2 id="carboncopyclonerexternalharddrives">Carbon Copy Cloner + external hard drives</h2>
<p>I use <a href="http://www.bombich.com/">Carbon Copy Cloner</a> (CCC) to create a full, bootable clone of my Mac hard drive.  Bootable means that I can actually boot my Mac off of the backup and see my entire system exactly as it was when the backup ran. (This is one of my favorite aspects of the Mac OS.)</p>
<p>It’s worth noting that many people use <a href="http://www.shirt-pocket.com/SuperDuper/">SuperDuper!</a> instead of CCC. It’s also a great choice, but I’ve always used CCC. It just works, and I haven’t had a reason to change.</p>
<p>I use a simple rotation system with two USB hard drives. I keep one of the hard drives at home.  I store the other offsite.  I back up to one on the 1st of each month and to the other on the 15th of each month. This gives me a 2-4 week-old full bootable clone of my Mac that I can use at any time.</p>
<p>Some would say that keeping a copy of my data offsite is being overly paranoid. I would say that it’s just common sense, if not a modern necessity.</p>
<p>As we store more and more of our lives in data, it’s important to make sure the data could survive things that happen every day in the world. Things that we don’t like to think about… like fires, theft, and floods. And fast forward 5-10 years from now. Eventually you’ll have a lifetime of photos stored digitally.  Imagine if you lost them. Sickening.</p>
<p>Some people use online services for the purpose of backing up large quantities of data. <a href="http://mozy.com">Mozy</a> and <a href="http://www.backblaze.com">BackBlaze</a> are good examples.</p>
<p>I chose my manual system because it avoids cloud data security issues and it’s also more cost effective. Buying a couple of USB hard drives is cheaper than paying a monthly fee indefinitely.</p>
<p>Restoring data from a physical drive that’s in your possession is also way faster than downloading it over the internet.</p>
<h2 id="adhocbackups">Ad hoc backups</h2>
<p>Anytime I do a major upgrade on my MacBook Pro, I make a full bootable clone of my hard drive beforehand.</p>
<p>I also use a PC for a few specific activities, but they occur infrequently.  Any data too large for Dropbox gets copied to an external hard drive or FTP server manually.</p>
<h2 id="theimportantpart:whythissystemworksforme">The important part: Why this system works for me</h2>
<p>In a nutshell, my backup workflow works because it’s become a mindless rhythm in my life. Dropbox and Time Machine work with virtually no assistance on my part. They do their thing without imposing any friction whatsoever on my work.</p>
<p>My external hard drive rotation is the most manual part of my backup workflow. To ensure that it happens on schedule, I’m assisted by my trusty task system, <a href="http://www.rememberthemilk.com">Remember the Milk</a>.</p>
<p>For the hard drive that I keep at home, I simply set a reminder once a month. For the drive I store offsite, I use several bite-sized tasks that happen over a two-day period:</p>
<ol>
<li>Get drive</li>
<li>Back up to drive</li>
<li>Store drive again</li>
</ol>
<p>Maybe this is too much detail, but I thought it was worth mentioning how I designate specific, actionable tasks to carry out the back up. By breaking the process into small, simple actions, I increase the chances that I will do those actions consistently in the long run.  And I have.</p>
<p>Positive inertia.</p>
<h2 id="whataboutyou">What about you?</h2>
<p>How do you keep your data backed up?</p>
<p>What practical balance did you strike?</p>
<p>Do you have any data loss horror stories to share?</p>
