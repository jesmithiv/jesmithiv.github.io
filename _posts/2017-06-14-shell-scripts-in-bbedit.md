---
layout: post
title: One-off shell script execution in BBEdit
---

I've been meaning to talk more about my "Sublime Text *and* BBEdit" workflow, and this is a powerful (if mundane) example. 

I don't write a ton of scripts on my Mac and generally don't spend much time in Terminal. But when I need a script, *I really need a script*. My work is very file-heavy. I juggle large numbers of `.tex` (LaTeX) files across several large folder structures. Every so often I need to copy a subset of files within one folder to another folder so that I can do things to them.

In most cases, I have a list of the files in a plain text `.tex` file, and I just need to do some file operations on them. Selecting them individually in Finder is tedious and error-prone, so the solution is usually a simple bash script with a bunch of `cp` commands.

The main friction with bash scripting for folks like me that don't live in Terminal is that you have to create a `.sh` script and then web search for now to make it executable (because I can never remember the `chmod` command).

Creating the shell commands is straightforward, especially in Sublime Text. After adding the necessary `#!/bin/bash` line with TextExpander and defining the "to" and "from" file paths as variables, the magic of Sublime Text's multiple cursors makes it easy to put `cp` commands and the folder path variables around each file to be copied.

![](/img/sublime-text-multiple-cursor-shell-commands.gif "Sublime Text")

Since Sublime Text won't execute these commands in an unsaved file that hasn't been given proper execute permissions, I simply copy this text into an untitled, unsaved BBEdit window and hit `⌘R`.

![bbedit-bash-pe.png](/img/bbedit-bash-pe.png "BBEdit")

I realize this post is a weird way to promote BBEdit, which is a powerful text editor that, in this case, I'm not even using as an editor. Hopefully I'll find some time to talk more about other ways I'm using it with Sublime Text. 

