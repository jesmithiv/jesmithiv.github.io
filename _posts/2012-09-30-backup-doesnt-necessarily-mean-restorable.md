---
layout: post
title: Backup doesn't necessarily mean restorable
redirect_from: /home/2012/09/29/backup-doesnt-necessarily-mean-restorable/index.html
---
<p>If you use Time Machine, USB storage devices, or online options for routinely backing up your data, that’s fantastic. Good for you. You’re probably in a minority.</p>

<p>Unfortunately, your safety net may be little more than a cardboard cutout propped over cold concrete.</p>

<p>Here are a few things that happen in real life with alarming regularity… things you don’t want to happen when you <em>really</em> need to recover data.</p>

<h2 id="timemachine:lastbackup:delayed">Time Machine: “Last backup: delayed”</h2>

<p>Maybe you turned it off a few weeks ago to keep it from ruining a Skype call and forgot to turn it back on. Maybe something’s snarled on your network drive. Doesn’t matter now: you’re effed.</p>

<p><strong>How to avoid</strong>: Make a habit of looking in your menu bar to make sure Time Machine is running. Even better, go into Time Machine every so often and make sure you see a running daily archive of backups. Practice restoring a file or two to make sure it actually works.</p>

<h2 id="corruptusbharddrives">Corrupt USB hard drives</h2>

<p>Let’s face it: they’re cheap pieces of (mostly) plastic. They die. Backup programs can be imperfect at copying data. And if data on your Mac hard drive itself gets corrupted—even a little piece of it—that same problem will be cloned your external backup drives, just waiting to make you miserable at a time when your fists are already full of hair.</p>

<p><strong>How to avoid</strong>: Run Disk Utility to verify and repair external drives. It usually only takes a few minutes and can save you a ton of frustration.</p>

<h2 id="overlyselectiveonlinebackups">Overly selective online backups</h2>

<p>Maybe you got a little too checkboxy when you were deciding which folders to let slip into the clouds. Or maybe you didn’t fully understand which types of files your online system <em>includes</em> in its backup.</p>

<p>A recent personal revelation: Backblaze, a system I just started using, doesn’t include <code>.dmg</code> files. If you thought the important documents in your secure disk images would be in your Backblaze backup during a data crisis, you’d be wrong.</p>

<p><strong>How to avoid</strong>: Go into your online backup, and take some time to inventory key items like secure documents, photo libraries, home movies, or anything else that you <em>really</em> want to be able to recover in the future. Make sure everything you <em>think</em> is offsite is <em>really</em> offsite.</p><p><strong>Update:</strong> <a href="https://mobile.twitter.com/brandonpittman/status/252723226977906688">Brandon Pittman on Twitter</a> pointed out to me that the disk image file extension (dmg) is listed in Backblaze's excluded file type list by default. Removing that file extension tells Backblaze to include disk images. All is well again. My message above remains the same, however: know what's really in your backup.</p>
