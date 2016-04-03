---
layout: post
title: Tightening Alfred file filters even more 
redirect_from: /home/alfred-file-filters/index.html
---


[Alfred][a] makes it [very easy][filter] to create a file filter that looks at one or more folders (not necessarily near each other) with specific extensions (e.g. PDF) and other attributes. I have several of these very simple Alfred workflows that I use all the time to locate reference PDFs and also PDFs that I've created.

It is by far the most efficient way I've found to pull up a file if I know it's general nature and just a piece of the file name. Spotlight is great, but it's too big a net in many cases. With Alfred, I can type a short keyword, a piece of the filename, and it's instantly in view without even leaving site of other windows I have open.

The only friction with these workflows happened when I was searching folders containing PDFs that I periodically duplicate and update by putting a new version number on the file name. For example, a folder could end up containing `ABC-v1.PDF` through `ABC-v10.PDF`. In most cases I want to go straight to v10. 

Fortunately I've long used the stock OS X file colors (which are now technically tags) to highlight the "active" version. I had always done this as a visual guide so that if I entered the folder with Finder, my eye would go straight to the important copy.

Very recently I discovered that Alfred file filters can also [filter on tags][tags]. By adding the `kMDItemUserTags` metadata field and setting the value to `Blue`, which is the color I use to denote active files, it restricts the Alfred workflow results to only `Blue`-tagged files. This cuts the results returned by Alfred even more so that in most cases I see only one or two PDFs after typing even the tiniest bit of the file name. It's so great.

I've always had a [special place in my heart][app] for application launchers, but Alfred has become this essential layer on top of OS X that makes the basic Mac file system a remarkably efficient content management system.  

[app]: http://www.practicallyefficient.com/home/2014/4/28/typing

[a]: https://www.alfredapp.com
[filter]: https://www.alfredapp.com/help/workflows/inputs/file-filter/

[tags]: https://www.alfredapp.com/blog/tips-and-tricks/3-ways-to-use-osx-tags-for-better-search/