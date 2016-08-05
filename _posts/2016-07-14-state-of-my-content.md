---
layout: post
title: On the current state of my content
---

In the last year I've had a huge renewed interest in both journaling and thought capture. I've also been moving out of Evernote for all-purpose information storage. 

My current system can be broadly split into two conceptual components:

1. Plain text notes and writing
2. Everything else with reference or research value 

The apps and tools I primarily use are:

- The Mac file system
- [Alfred][alfred] and Spotlight for Mac search
- [Dropbox](https://www.dropbox.com/)
- [Drafts][drafts], [nvALT][nvALT], and [1Writer][1w] for thought capture and plain text writing
- [DEVONthink][dt] for non-plain-text media organization and search
- Apple Notes for certain reference information mainly accessed from my phone 

The rest of this post is how I got here. 

[dt]: http://www.devontechnologies.com/products/DEVONthink/overview.html


## The elephant that ate too much

For ages (in internet time), [Evernote][ev] was my searchable junk drawer—a place for the digital debris of my life with a low but *importantly* non-zero information density. Evernote makes it so easy to put *everything* in. It even OCRs images, making their text searchable without any additional effort on my part. It's so great at what it does. And I'm leaving it.[^f1]

[ev]: https://evernote.com/?var=c

As I've aged with Evernote, I've become more aware of its self-spamming effect. Just like email spam requires infinitesimal effort on the part of the spammer to affect infinite inboxes, Evernote puts no gating at all on self-storage. It's a 24-hour digital hoarding rave, and there's no bouncer at the door.

I've got gigs and gigs of HTML, PDF, images, and other debris inside my Evernote database. Ten years from now, it's likely to be terabytes and terabytes. 

I know that a lot of people wouldn't see this as a problem. I mean, disk space is cheap, and search is great. All true.

What digs at me is that I don't end up creating enough with my accumulated junk. Sure, it's useful to be able to locate the serial number of an obscure dishwasher part on page 61 of a PDF manual I stored five years ago, but that's purely a reference kind of value. It's not creative.


## Creativity doesn't lend itself to automation 

Before the concept of "information capture" was such an internet-ism, people captured information mainly through journaling and manually filing paper—newspapers, magazines, books, etc.

And history shows that people managed to do some really amazing things with these archaic systems. I mean, anyone who wrote a book, produced a movie, delivered a historic speech, or published anything before the year 2000, probably used a lot of paper and not much else. 

Some people still do use paper, including my friend [Ryan Irelan][ryan], who uses an index card system for filing and organizing his ideas ([YouTube](https://youtu.be/34iWYR1U6aE))

<iframe width="560" height="315" src="https://www.youtube.com/embed/34iWYR1U6aE" frameborder="0" allowfullscreen></iframe>

Non-digital systems probably seem like all *disadvantage* today because of the effort they require of the filer. But one person's wasted time is another person's opportunity to impose creative order. When you have to physically touch your information to review and search it, you interact with it differently. You impose friction and constraint—necessary conditions for all forms of creativity.

**The more manual and active your system, the more *you* become embedded in the system itself rather than a passive observer of it.**

I don't think that I will ever adopt a pure paper index card system like Ryan uses. But I really love the essence of it, and I think it should serve as a check on any digital system I use. 

As I've been moving out of Evernote, I've been paying much more attention to the types of notes and information that I've collected and stored. It's a bit like peeling back geological layers and seeing the things I was especially interested in at various points in the past. I've deleted a lot of things that I never should've stored in the first place, and I've also come across really interesting things that I had forgotten I stored—things that have triggered ideas and things that have revealed important patterns. 

**Key lesson learned: stored information should be reviewed regularly. Otherwise, it stays in a frozen state.** 


## Designing a better capture system

For thought capture, I've mostly moved back to an all-plain-text approach—a truth I guess I had to rediscover after being lured briefly back into the seductive proprietary rich text universe that exists in the App Store. 

99 percent of all rich-text-like needs in a plain text environment were solved by John Gruber's last update to Markdown over ten years ago, and countless Mac and iOS text editors make it even easier. 

Today, I capture most thoughts and notes in [Drafts][drafts] simply because my iPhone is with me most often. On my Mac, [nvALT][nvALT] is still the king of all note-taking apps. Drafts and nvALT fundamentally have the same benefit in common: they impose zero friction on capturing thoughts, and they force me to translate thoughts into unformatted ASCII. The beauty of plain text will forever be its simplicity and mobility. It is usable and retrievable anywhere when stored in a place like Dropbox. 

Plain text also puts a common denominator on all notes I create myself. Plain text is easy to combine, delete, rephrase, and search. Text files are extremely versatile. At one extreme, just the filename itself could represent a short note without any content in the body of the file. At the other extreme, a single plain text file can serve as a filing cabinet for years of journaling without creating any material file size problems. 

In fact, the concept of individual text files is really quite arbitrary. A collection of text files is more of a liquid medium in itself—a uniform cloud of elements that can range from low to high entropy depending on the whims of their puppeteer. 

For bulk text editing and advanced filtering, I've found nothing better than [Sublime Text][st], especially for very large multi-file writing projects involving Markdown and LaTeX. 

[st]: https://www.sublimetext.com/


## Designing a better system for everything else

All information can't (and shouldn't) be stored in plain text. Virtually all of my non-plain-text information is some form of reference information—files that are less likely to be edited and have more read-only value. This is an enormous category containing PDFs, photos, web clippings, and more. PDFs are easily the largest group within the non-plain-text category, and I've found that the best way to retrieve PDFs is to thoughtfully and verbosely name them so they can be searched by file name. The longer the file name (complete with `yyyy-mm-dd` date), the more easily it can be found later with even basic searches using OS X Spotlight or the iOS Dropbox app. 

In fact, in my experience, long file names are vastly superior to tags or folders. I have folders with hundreds of PDFs that I can easily navigate with file filters using [Alfred file filters][aff] or [Path Finder][pf]. File names also don't rely on a meta data layer like tags. 

For deeper content searches, I use DEVONthink. Even before I made a firm commitment to leave Evernote, I had largely replaced Evernote as a PDF repository with DEVONthink. There are so many reasons to love DEVONthink, which in my opinion is truly the best all around content management system for the Mac beyond the OS X file system itself.

Like Evernote, you can put virtually any media type into DEVONthink. *Unlike* Evernote, you aren't limited to keeping everything inside a proprietary database, and you aren't forced to store all of your data on Evernote's servers. DEVONthink lets you index folders in the Mac file system outside of DEVONthink, and I use this *a lot* to do keyword content searches across multiple folders of PDFs—often mixtures of PDFs stored in research folders and PDFs I've created myself for my work. In an instant, I can see sorted results and the incidence of keywords and phrases—and I can open the PDFs in Preview and work with them with any tool on the Mac. 

In its simplest form, DEVONthink is a very powerful search tool—and more accurate at searching *inside* PDFs than Evernote in experiments I've conducted. But DEVONthink Pro Office (DTPO) offers so much more, including the most accurate OCR engine I've ever used. DTPO comes with built-in [ABBYY Fine Reader technology][abbyy] for OCR. Not only is it extremely accurate, I can queue up hundreds of files at once. In fact, one of the first things I did after letting DTPO import my Evernote notebooks (something else DTPO does flawlessly), was to have DTPO OCR all PDF scans and images containing text, which DTPO turns into searchable PDF.

With Evernote, I have to rely on their cloud-based OCR and the text indexing Evernote does within the app. If I export an image or PDF scan from Evernote, the OCR layer does not go with it. With DTPO, the OCR layer is saved into the file allowing me to use the searchable PDF anywhere else I want, not just DTPO.

DTPO is also very inbox-centric. Every DTPO database has an inbox, and DTPO even has a global inbox from which files can be moved anywhere. The inbox approach makes a lot of sense to me because it causes me to take at least one additional look at everything going in before filing it away.   

When the new [DEVONthink for iOS][dtg] comes out later this year, DEVONthink will really be the undisputed winner in the all-purpose information storage category. 

8/5/2016 Update: [DEVONthink To Go 2][d] is now in the App Store.

The more I use DTPO, the more I *really* use it. I can even integrate the plain text notes I described earlier into DEVONthink by simply indexing the folder where I store my plain text notes, and it even recognizes OS X file colors / tags. It is the ideal companion to the already powerful file system that ships with every Mac.


## Apple Notes is pretty good too

As of iOS 9, Apple Notes became much more robust. While I don't see myself ever using it to the [extent that David Sparks does][sparky], I have started using Notes for a special category of information that I need fast access to from my phone. Things like insurance cards, notes about my kids' medicine doses, and other personal information are really useful to have stored locally on my phone—only a quick iOS Spotlight search away. The notes I create in Apple Notes tend to be more like mini-documents. It's not a place I dump thoughts or disorganized text. It's a mostly read-only place for light rich-text reference notes with small attachments. 

As of iOS 10, Apple Notes has become even stronger with the ability to share notes. Even though Evernote allows *paying* customers to share notebooks with *non-paying* customers, the non-paying person still has to use and maintain Evernote for it to matter. In my experience, most of my friends and family members don't keep Evernote up to date and don't use it regularly. Apple Notes is on every Apple device by default, making it more reliable for note sharing. 


## In summary

My information systems will always be in a state of flux, but I feel like I've become much more aware of key patterns in how I save and use information. I also want to prioritize creativity in the design of my information systems and minimize "data hoarding" just because an app makes it easy. I want to be more of a filter on both incoming information and information I've already stored—emulating a paper filing system using digital tools. In doing this, I hope to discover even more patterns, connections, and [aesthetics][aes]. 

[d]: http://www.devontechnologies.com/products/devonthink/devonthink-to-go.html
  
[aes]: http://www.practicallyefficient.com/2016/07/13/the-role-of-aesthetics-in-information-systems.html

[1w]: http://bit.ly/1writerapp

[abbyy]: https://www.abbyy.com

[ryan]: http://ryanirelan.com/

[dtg]: http://blog.devontechnologies.com/2016/05/making-progress/

[aff]: http://www.practicallyefficient.com/2016/03/09/alfred-file-filters.html

[pf]: http://www.cocoatech.com/pathfinder/

[drafts]: https://itunes.apple.com/app/id905337691?mt=8&uo=4&at=11l4Cf&ct=website

[nvALT]: http://brettterpstra.com/projects/nvalt/

[sparky]: http://macsparky.com/blog/2016/2/7al32geo05j88gmyrkrku0e04yncvm

[alfred]: https://www.alfredapp.com

[^f1]: There are a lot of reasons I'm leaving Evernote. And for the record, it's not *just* about the price increase, although that certainly makes it easier to leave a system I was only fractionally in love with. I do *not* believe the higher price of Evernote alone should be reason to leave Evernote. In fact, I agree with [Brett Kelly](https://brettkelly.org/evernote-price-increase/) that the price increase is actually quite small for someone who uses and relies heavily on Evernote. 

