---
layout: post
title: My adventure so far with Photos and other mythology
redirect_from: /home/photo-mythology/index.html
---
<p>So far, my move from Aperture to Photos has been mostly good. The new Photos app is a good fit for me. I don't do much professional editing, and I like having all of my photos available everywhere.</p>

<p>The only bumps I've experienced so far were related to the initial import from Aperture to Photos and the initial upload to iCloud Photo Library. I'm posting these anecdotes here in case it helps someone else. . . because as of the time I'm writing this, I did not find a lot of insight elsewhere online.</p>

<h2 id="theinitialuploadwasconfusingtomeatleast">The initial upload was confusing (to me at least)</h2>

<p>I don't have nearly as big of a photo library as a lot of people. I <em>only</em> have just over 10,000 photos and a little over 100 videos in my current iCloud Photo Library. I have a reasonably fast upload speed though my cable ISP (over 4 Mbps up), and online backups like Backblaze and Dropbox have always performed faster than I expected.</p>

<p>Even though I paused or turned off other online backup services during the initial iCloud Photo Library upload, it took much longer than I expected—approximately one week.</p>

<p>In the final days, I was able to speed up things by leaving my MacBook Pro awake and open as much as possible and also making sure the Photos app was open. Just based on my observations of network traffic, the iCloud upload services seemed to run faster when I did this.</p>

<p><strong>The biggest point of confusion for me, however, was the iCloud Photo Library sync behavior during the initial upload.</strong> Shortly after I initiated the upload on my Mac, I activated iCloud Photo Library on my iPhone as well. The iPhone upload time was negligible (presumably because those photos were already in the cloud), but it surprised me when I did not see recently taken iPhone photos on my Mac.</p>

<p>Photos taken on my iPhone did not sync to my Mac <em>at all</em> until the Mac's initial week-long upload finished. In the weeks since it has finished, however, everything has been syncing just fine, and I've had no syncing issues at all. None. </p>

<p>But as the heading above says, the initial part was just plain confusing and unexpected. The fact that the photos were not syncing days after my Mac and iPhone were both connected to iCloud Photo Library did not inspire confidence, but I'm good now.</p>

<h2 id="localphotolibrarysizesdontmakemuchsensetomeanymore">Local photo library sizes don't make much sense to me anymore</h2>

<p>At some point during the initial upload to iCloud Photo Library, my Mac decided that it no longer had enough disk space locally for my photos (even though my local disk was the original source of all these photos. Hmmm. Yeah.).</p>

<p>This optimization setting seems to work extremely well on my 64 GB iPhone. I was initially concerned that by activating iCloud Photo Library on my iPhone, it would gobble up storage, but that hasn't happened at all. I have tons of free space despite having access to all of my iCloud-based photos now.</p>

<p>Because this seemed to work so well on my iPhone, I didn't have a major problem allowing the same optimization black box to run wild and free on my MacBook Pro, where I'm constantly running out of disk space anyway. </p>

<p>And so everything finished, and everything seemed fine until. . .</p>

<p>I recently noticed that my local Pictures folder (home of the photo library files) had ballooned in size to over 85 GB, and I was once again running out of disk space. This made no sense to me because the space occupied by my photos and videos in iCloud was only about 55 GB. </p>

<p>And so—<em>I'm guessing</em>—not unlike ancient agriculturists at the mercy of the heavens, I raised a fist to the cloud, albeit while cursing about very different problems than they ever did. </p>
  
       [caption id="" align="alignnone" width="361.0"]<img src="/img/img.png" alt="Local space taken up by Pictures folder on Mac"/> Local space taken up by Pictures folder on Mac[/caption] 
  


  
       [caption id="" align="alignnone" width="465.0"]<img src="/img/img.png" alt="Size of photos and videos stored on iCloud servers"/> Size of photos and videos stored on iCloud servers[/caption] 
  

<p>Why were photos stored locally taking up 30 GB <em>more</em> disk space than the total size of the iCloud-based library, especially if my Mac was supposed to be optimizing for storage locally?</p>

<p>Well, I never got an answer to that question, but fortunately no data famine ensued, and after looking around <a href="http://apple.stackexchange.com/questions/180310/where-are-photos-stored-in-the-new-photos-app-after-importing-from-aperture">online a bit</a>, I decided I might as well try deleting my old Aperture and iPhoto library files. (I'm not sure why I had an iPhoto library since I had never used it.)</p>

<p>From my understanding, when you import to Photos from Aperture or iPhoto, it builds the new Photos library by making hard links to the source files in the older library files, but the import process does not actually delete the older library files. However, only one instance of your photos exists on your Mac; it's just that each library is pointing at that instance. Imagine that you have two shortcuts on your desktop, each pointing to the same 1 GB file. There's only one file, but it has more than one finger pointing at it. In theory, this should only take up 1 GB space on your disk, not 2 GB.</p>

<p>But anyway. . .</p>

<p>The key thing I realized is: Deleting the old library files <em>should</em> not actually delete any photos. (By the way, this is a great time for me to make it clear that it's not my fault if you wreck your own photo libraries.)</p>

<p>So I blew away the old migrated Aperture library and the iPhoto library that I never created in the first place even though <a href="https://support.apple.com/en-us/HT204476">Apple says</a> I shouldn't have to do that. This immediately freed up an enormous amount of space on my local disk. I also noticed that Photos kicked into high gear downloading a bunch of photos. </p>

<p>Even though the photo count and iCloud library size did not change at all from the 55.65 GB pictured above (indicating that I most likely did not harm any of my actual data), I'm guessing that it needed to do some rebuilding locally using cloud data. Within an hour, the download had finished, and I had gained over 40 GB of disk space locally.</p>
  
       [caption id="" align="alignnone" width="362.0"]<img src="/img/img.png" alt="Local Pictures folder after library deletions and iCloud download finished"/> Local Pictures folder after library deletions and iCloud download finished[/caption] 
  

<p>Staying with the overall theme of this post, this disk space issue was confusing initially, but everything seems fine now. I'm alive and well and in search of another First World problem to solve—most likely while consuming some unhealthy product made possible and affordable by mass agriculture. Clouds of all forms, be damned.</p>
