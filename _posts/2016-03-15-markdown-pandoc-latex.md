---
layout: post
title: Markdown to LaTeX via Pandoc
redirect_from: /home/2016/3/15/markdown-pandoc-latex/index.html
---

I have become a huge fan of [Pandoc](http://pandoc.org) for converting Markdown to LaTeX code. It’s especially useful for outline-heavy text because it lets me avoid the more cumbersome `itemize` and `enumerate` environments in LaTeX during the writing process.

My Markdown to LaTeX workflow has gone through several refinements and is now as efficient as ever. I simply write a block of text in Markdown, copy it, and run a Terminal command:

	pbpaste | pandoc -f markdown -t latex | sed -e 's/\\tightlist//'  | pbcopy

This command sends my clipboard contents to `pandoc`, which converts the Markdown to LaTeX. It then pipes the `pandoc` result to a `sed` command, which removes the `\tightlist` command from the LaTeX code produced by `pandoc` since I have no use for it in my final code. The final result ends up back on my clipboard via the final `pbcopy` command so that I can just paste it anywhere—often right on top of the Markdown I originally copied. 

I usually run short Terminal commands like this by turning them into plain text TextExpander snippets and [running them through Alfred](https://www.alfredapp.com/help/features/terminal/) preceded by `>`. There are arguably [better ways](https://www.moncefbelyamani.com/create-aliases-in-bash-profile-to-assign-shortcuts-for-common-terminal-commands/) of doing this.

