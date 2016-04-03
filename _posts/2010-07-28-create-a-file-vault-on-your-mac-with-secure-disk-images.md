---
layout: post
title: Create a file vault on your Mac with secure disk images
redirect_from: /home/2010/07/28/create-a-file-vault-on-your-mac-with-secure-disk-images/index.html
---
<p><em>This is part 3 of a 3-part series on Mac data security: <a href="http://www.practicallyefficient.com/tag/perils-of-persistent-data/">Perils of persistent data</a>.</em>
<p style="text-align: center;">* * *</p>
<p>Macs come with all kinds of useful utilities pre-loaded.  One of the best is Disk Utility, which lets you do everything from repairing and formatting a hard drive to creating “virtual” drives right on your Macintosh hard drive.</p>
<p>We can take advantage of Disk Utility’s ability to create virtual hard drives for the purpose of making vaults for sensitive data.  This is what’s known as a <strong>secure disk image</strong>.</p>
<p>Secure disk images are ideal for storing sensitive information on your Mac for several reasons:</p>
<ol>
<li>They are <strong>easy to create</strong>.</li>
<li>They can be <strong>password protected.</strong></li>
<li>They can be <strong>secured with 128-bit or 256-bit AES encryption</strong>. Highly secure, both.</li>
<li>They can be <strong>any size you want</strong> and even <strong>automatically expand</strong> as more data are added.</li>
<li>They are <strong>portable.</strong> The disk image appears as a file on the system. Just drag and drop it onto another disk if you want. You can even email them if small enough.</li>
<li>When opened, secure disk images <strong>look like any other drive in your Finder sidebar</strong>, and you can <strong>eject</strong> them when you’re done to seal the vault again.</li>
</ol>
<p>The following is a quick tutorial on creating secure disk images.</p>
<p><!--more--></p>
<h2 id="howtocreateasecurediskimage">How to create a secure disk image</h2>
<p>Apple’s website has a nice <a href="http://support.apple.com/kb/ht1578">tutorial</a> on creating a secure disk images.</p>
<p>Here’s an even quicker overview:</p>
<ol>
<li>Open Disk Utility.</li>
<li>Click the New Image button.</li>
<li>Fill out the fields in the window that pops up.</li>
</ol>
<p>In the example below, I’ve chosen to name the image “Secure,” but you could call it anything you want – and save it anywhere you want. Just think of it as a special file.</p>
<p><a href="/img/secure-disk-image-pe.png"><img class="aligncenter size-full wp-image-789" title="secure-disk-image-pe" src="/img/secure-disk-image-pe.png" alt="" width="530" height="453" /></a></p>
<p>Here’s an explanation of each field:</p>
<ul>
<li><strong>Name</strong>: This is the name of the drive that will appear your Finder sidebar when the secure disk image is open.  Call it anything you like.</li>
<li><strong>Size</strong>: This is the maximum size the drive can become.  Be sure to make it big enough for your needs.</li>
<li><strong>Format</strong>: As long as you’re only planning to use this drive on your Mac, I recommend the Extended (Journaled). If you want to share the image with someone using Windows or Linux, you may want to use a different format.</li>
<li><strong>Encryption</strong>: By selecting either 128-bit or 256-bit here, you’re basically telling Disk Utility to password protect the secure disk image.  I recommend 128-bit since it provides plenty of security and runs faster than 256-bit.</li>
<li><strong>Partitions</strong>: Here, you can create multiple partitions within the secure disk image.  Single partition will probably be just fine for most uses.</li>
<li><strong>Image Format</strong>: The default here is “read/write disk image,” but I’ve chosen “sparse disk image” instead.  A sparse disk image automatically expands as you add more and more data.  It will expand up to amount you put in the <strong>Size</strong> field.</li>
</ul>
<p>After you click the <strong>Create</strong> button, you’ll be prompted to enter a password.  This is a key step.  Your secure disk image is ONLY as secure as your password.  Make it a good one.  You may want to check out my <a href="http://www.practicallyefficient.com/tag/passwords/">series on passwords</a> for tips.</p>
<p>By default, the password window will have “Remember password in my keychain” checked.  <strong>You do NOT want to check this box.</strong></p>
<p><a href="/img/secure-disk-image-password-pe.png"><img class="aligncenter size-full wp-image-791" title="secure-disk-image-password-pe" src="/img/secure-disk-image-password-pe.png" alt="" width="446" height="340" /></a></p>
<p>Checking that box defeats the purpose of everything you’ve just gone through.  If the password is stored in your Mac keychain, you will never be prompted for it.  Anyone who double clicks your secure disk image, will just walk right in.</p>
<p>The only way to secure your data is to put it behind a strong password, but you want to make sure that you will get prompted for it every time.</p>
<p>A few more secure disk image tips:</p>
<ul>
<li>You can keep a shortcut to your secure disk image in your Finder sidebar for quick access (mine is called Secure.dmg).</li>
</ul>
<ul>
<li>You should get in the habit of only opening your secure disk images when you need to.  I only open mine when I need to put files in or look at files inside.  When I’m done, I eject.</li>
</ul>
<h2 id="apaidalternativetousingdiskutility">A paid alternative to using Disk Utility</h2>
<p>Agile Web Solutions, maker of 1Password (my favorite password manager for the Mac) recently acquired the maker of <a href="http://agilewebsolutions.com/knox">Knox</a>.</p>
<p>Knox costs $34.95 and is designed to streamline the process of making secure disk images on your Mac.  It offers several options for organizing information like email, receipts, and anything else you want to hide from prying eyes.</p>
<p>I have not tried Knox myself, but I have a lot of confidence in Agile Web Solutions.  1Password is a brilliant application, and Agile definitely seems dedicated to security solutions for the Mac.</p>
<h2 id="seriesrecap">Series recap</h2>
<p>This concludes my little mini series on making your Mac more secure. I hope you found it helpful. I'm sure there's a lot I can learn from you too. Let me know.</p>
