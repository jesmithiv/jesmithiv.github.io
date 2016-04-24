---
layout: post
title: Outsmarting the smart dash
---

I like writing dashes—both the en dash (–) and the em dash (—). But I don't like the way OS X "smartly" converts certain patterns like `--` to `–`. I would rather have direct control over these patterns for at least two reasons:

1. If I'm writing something that will ultimately end up in a LaTeX document, I need to preserve `--` and `---` strings because LaTeX is designed to turn those into `–` and `—`, respectively, in the resulting PDF. LaTeX will usually choke on *actual* en and em dashes in the `.tex` file. People unfamiliar with LaTeX would probably see this as a limitation, but I truly believe it's a great feature because it ensures that all hyphens and dashes are composed of `-` as a base character, making it *very* apparent what I've typed in plain text.
2. Even if I'm writing something that won't end up in a LaTeX file, I can easily create en and em dashes manually by preceding the `-` key with `Opt` for an en dash and `Shift-Opt` for an em dash. Both work system-wide in OS X. 

In other words, I don't need OS X to be "smart" enough to make these symbols. I can instantly create them myself according to how they'll be used.

Before OS X Mavericks, you could explicitly turn off smart dashes in System Preferences. Beginning with Mavericks, however, dashes *and quotes* were forced to share a common check box.

![](img/keyboard-pref-pe.png)

I don't really mind curly quotes showing up in places because even if I'm writing something for a LaTeX file outside of a `.tex` environment (e.g. in an app like [Ulysses](http://www.ulyssesapp.com)), I will normally [run everything through Pandoc](http://www.practicallyefficient.com/2016/03/15/markdown-pandoc-latex.html) to generate proper LaTeX code. Pandoc is pretty good with translating quotation marks of all kinds into proper LaTeX syntax:

    ``quoted text''

It's not so good, incidentally, with en dashes, which are more ambiguous in meaning—some people use them in place of a subtraction symbol, while others use them in contexts where em dashes are more appropriate.

All that to say, it's unfortunate that you can't separately turn on/off smart dashes and quotes in System Preferences. Fortunately, though, you [still can through Terminal](http://superuser.com/questions/555628/how-to-stop-mac-to-convert-typing-double-dash-to-emdash) with:

	defaults write 'Apple Global Domain' NSAutomaticDashSubstitutionEnabled 0

This command turns off smart dashes, allowing you to preserve `--`, etc. in any document, but it allows smart quotes to continue functioning. Interestedly, System Preferences will show the smart dashes and smart quotes box *unchecked* after this change even though smart quotes still work.

For more on dash usage, see [The Punctation Guide](http://www.thepunctuationguide.com/em-dash.html). 

