---
layout: post
title: rsync + Automator = free and easy backups for your Mac
redirect_from: /home/2011/03/18/rsync-automator/index.html
---
<p>One of the most basic types of backup is the folder sync.  Folder A lives on your Mac. Folder B is on an external hard drive.  You want to make Folder B look exactly like Folder A.
Granted, anyone could make this happen by dragging and dropping the contents of A to B.  If you have a lot of data, that’s going to take a while each time, though.</p><p>Fortunately, there’s a really easy, free way to make this happen with almost no effort (or geekery) on your part using two tools that are already on your Mac: rsync and Automator.</p><h2 id="rsync">rsync</h2><p><a href="http://en.wikipedia.org/wiki/Rsync">rsync</a> is a command line utility that works on lots of operating systems, including Mac OS X. It’s really great at backing up data and can do some powerful and mind-blowing things, most of which you need to know nothing about.</p><p>I’m using rsync in a very basic way.  For example, this command copies all of the contents of my Documents folder (under my Home folder, the ~ sign) to an external hard drive called “Lacie500”:</p><p><code>rsync -aE --delete ~/Documents/ "/Volumes/Lacie500/Documents/"
</code></p><p>It essentially does two things:</p><ol>
<li>Copies anything that has changed since the last copy</li>
<li>Deletes anything on Lacie500 that is no longer in the Documents folder on my Mac</li>
</ol><p>In other words, it makes the Documents folder on Lacie500 look exactly like the Documents folder on my Mac.</p><h2 id="rsyncautomator">rsync + Automator</h2><p>Since I didn’t want to have to run this command from Terminal each time, I created a very simple, single-action workflow using Automator.</p>
  
<img src="/img/run-shell-script-pe.png" alt=""/>
  

<p>As you can see, I’ve got it set up to mirror my Documents, Pictures, and Music folder.</p><p>I saved the Automator workflow as “sync.app” so so that I could just store it right on the external hard drive's root folder. That way, all I have to do is plug in the external hard drive, click on the hard drive in Finder, then double click the app. The sync just happens, and I never have to think about command line syntax again.</p><h2>Why this is useful</h2><p>For starters, backups happen if they’re easy. Automating backups is one way to make them really easy.</p><p>I have what I consider a&nbsp;<a href="http://www.practicallyefficient.com/2010/10/29/the-right-side-of-inertia-a-backup-workflow-story/">pretty decent backup strategy</a>&nbsp;involving Time Machine, Carbon Copy Cloner, and Dropbox. But as I keep accumulating miscellaneous hard drives (not sure how that happens), I want to make use of them. This is one way.</p><h2>Stuff I read as I wrote this</h2><ul><li><a href="http://www.macinstruct.com/node/85">How to Backup Your Mac Using Rsync</a></li><li><a href="http://www.bananica.com/Geek-Stuff/Synchronize-two-folders-on-a-Mac-with-Automator-and-Rsync/">Synchronize two folders on a Mac with Automator and Rsync</a></li></ul><p></p>
