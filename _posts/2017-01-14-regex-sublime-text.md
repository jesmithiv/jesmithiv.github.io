---
layout: post
title: Regular expressions and Sublime Text
---

Regular expressions seem very difficult to learn at first, but once you get the hang of them, they are powerful tools. I'm using them more and more in Python scripts and also find/replace workflows in [Sublime Text](https://www.sublimetext.com).

Since I have several regular expressions that I use over and over (and over) again, I decided to store them in [TextExpander](https://smilesoftware.com/textexpander) for quick reference. I prefix each snippet with `rx`, which lets me use the TextExpander global shortcut to bring up a TextExpander search box anywhere in macOS so I can just grab the one I need.

![](/img/rx-te-pe.png "TextExpander and Regular Expressions")

Using regular expressions to find text in Sublime Text is easy, but remember to press the `.*` button on the far left of the find/replace form first.

![](/img/sublime-text-regex-pe.png "Sublime Text and Regular Expressions")

Regular expressions are even more powerful when you learn the "replace" syntax in Sublime Text. In the screenshot above, the regular expression `^.*\{frame\}` is designed to find lines containing the LaTeX Beamer `frame` environment and match all text from the beginning of the line through the closing `}` to the right of `frame`. 

By enclosing this search term in parentheses, I'm telling Sublime Text that I want to use it as a variable in my replace term. The variable is called `$1`. (You can separate multiple search terms with commas, to get `$1`, `$2`, etc.)

Therefore my replace term `% $1` will effectively insert the `%` (LaTeX comment symbol) at the beginning of each matched line. This comments out all lines containing the `frame` environment so that LaTeX will ignore them---something that's very useful in one of my LaTeX workflows.

But anyway, if you use Sublime Text a lot and want to take your find/replace routine to the next level, regular expressions are your friend. 

[RegExRX](https://itunes.apple.com/us/app/regexrx/id498370702?mt=12) is a really handy Mac app for building and testing regular expressions. 