---
layout: post
title: When Smart Sorting Smarts
redirect_from: /home/2015/02/26/smart-sorting/index.html
---
<p>I use <a href="http://www.cocoatech.com/pathfinder/">Path Finder</a> all day. I wouldn't even attempt to list all the reasons in a single blog post, but one little feature that I immediately appreciated when I started using Path Finder a few years ago was the way it sorted sub-folders above files in any given directory. This is definitely more of a Windows take on the visual file system, unlike OS X's Finder, which to my knowledge has always given folders and files equal preference in sorting (at least without <a href="http://www.howtogeek.com/67100/force-your-mac-to-put-folders-on-top-of-files-windows-style/">hacking</a> <code>.plist</code> files or installing <a href="http://apple.stackexchange.com/questions/289/how-can-you-get-finder-to-sort-by-name-but-also-sort-folders-before-files">add-ons</a>).</p>
  
       [caption id="" align="alignnone" width="909.0"]<img src="/img/img.png" alt="Example of how OS X Finder treats folders equally with files when sorting, while Path Finder places all sub-folders in a given folder up top. This particular folder has 159 objects. In the Finder view, the first "Published Copies" folder is the 145th item, which obviously requires a lot of scrolling to locate."/> Example of how OS X Finder treats folders equally with files when sorting, while Path Finder places all sub-folders in a given folder up top. This particular folder has 159 objects. In the Finder view, the first "Published Copies" folder is the 145th item, which obviously requires a lot of scrolling to locate.[/caption] 
  

<p>I just like folders up top because I mainly work out of the list view, and I think it's much more efficient to navigate through visual folder hierarchies when I don't have to scroll down to find sub-folders sprinkled among regular files.</p>

<p>I just recently realized that Path Finder can give sorting priority to other types of file system "objects." By default, Path Finder's settings give preference to package and app files, as well. This was actually causing some friction that I guess was mild enough for me to tolerate for a really long time without digging for a solution.</p>

<p>Most Mac users probably don't realize that a growing number of files that appear to be "files" are actually <em>packages</em> of files. Two common examples on my Mac: <code>.key</code> (Keynote files) and <code>.screenflow</code> (ScreenFlow project files). </p>

<p>The ScreenFlow package sorting was creating the most friction because I usually want to see a ScreenFlow project's exported <code>.mp4</code> file sitting next to its ScreenFlow project of the same name for folders sorted alphabetically. More importantly, I like to see the most recent <code>.mp4</code> files at the very top of my primary working ScreenFlow folder when sorting by <code>Date Modified</code> in Path Finder. If package files have priority over regular files and you sort by Date Modified, you'll see the package files grouped at the top. You'll have to scroll down to find where the files begin, with the most recent file appearing first.</p>

<p>Fortunately, the fix is easy. Just tell Path Finder not to give any preference to package files when sorting.</p>
  
      <img src="/img/path-finder-browser-preferences-pe.png" alt=""/>
  

<p>This makes a huge difference in my working ScreenFlow folder and lets me quickly grab the most recent <code>.mp4</code> files that I've exported simply by sorting by <code>Date Modified</code>.</p>
  
       [caption id="" align="alignnone" width="939.0"]<img src="/img/img.png" alt="Comparing the same folder in Path Finder—with and without giving priority to package files. Since all of the .mp4 files on the right were created after the ScreenFlow projects from which they came, the .mp4 files appropriately appear at the top."/> Comparing the same folder in Path Finder—with and without giving priority to package files. Since all of the .mp4 files on the right were created after the ScreenFlow projects from which they came, the .mp4 files appropriately appear at the top.[/caption]
