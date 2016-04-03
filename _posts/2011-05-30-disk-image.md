---
layout: post
title: How to automatically eject a disk image
redirect_from: /home/2011/05/30/disk-image/index.html
---
<p>I constantly forget to eject secure disk images, and it bugs the hell out of me. For the longest time, I've wanted a way to make a secure disk image eject automatically after X minutes.</p>
<p>Elasticthreads <a href="http://twitter.com/#!/elasticthreads/status/73375191425748992">came to my rescue</a>, and I was able to whip up a very simple app in Automator using AppleScript:</p>
<pre><code>on run {input, parameters}

tell application "Finder"
        do shell script "hdiutil attach ~/Documents/Secure.dmg"
        delay 1800 --number of seconds
        eject disk "Secure"
end tell
    return input
end run
</code>
</pre>
<p>So instead of double clicking Secure.dmg to mount it—like I used to—I run this app, which mounts Secure.dmg for me (after giving me the usual password prompt).  After 30 minutes, or 1,800 seconds, it ejects Secure.dmg.</p>
<p>For me, 30 minutes is usually ample time to do what I need to do Secure.dmg.  And I can always eject it manually and quit the app in the menu bar.</p>
<p>If this is too paranoid and geeky for you, congratulations. Forget about it. Otherwise, let me know if you come up with a more elegant solution.</p>
