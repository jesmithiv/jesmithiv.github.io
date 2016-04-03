---
layout: post
title: Building a better writing workflow with Notational Velocity, MultiMarkdown,
redirect_from: /home/2010/06/01/notational-velocity-multimarkdown-and-simplenote/index.html
---
<p><em><strong>Update 2</strong>: If you're interested in developing Notational Velocity, <a href="http://www.practicallyefficient.com/2010/09/29/a-call-for-folks-interested-in-working-on-notational-velocity/">read this too</a>.</em>
<em><strong>Update 1</strong>: In my original post (below) I use MultiMarkdown and Markdown interchangeably when talking about Steve Frank's forked version of Notational Velocity. Currently, it only supports Markdown syntax, so it will not display MultiMarkdown-specific elements (e.g. HTML tables). See the comments for more discussion.
</em></p>
<p>***</p>
<p>In my last post on MultiMarkdown, I received a great comment from <a href="http://caudygeg.tumblr.com/">CraigM</a>, who recommended Notational Velocity over TextEdit for “simple” writing on the Mac.  Since I had been meaning to try Notational Velocity for a while, I decided there was no better time than now.</p>
<p>I took Craig’s suggestion and downloaded a <a href="http://github.com/panicsteve/nv/downloads">version</a> of Notational Velocity developed by <a href="http://github.com/panicsteve">Steve Frank</a> with a <span style="text-decoration: line-through;">Multi</span>Markdown preview pane attached.</p>
<p>I love it.</p>
<p><!--more-->It works exactly as advertised.  As you write in the main note pane, the <span style="text-decoration: line-through;">Multi</span>Markdown pane updates in real time.</p>
<p><img class="alignnone" src="/img/notation.png" alt="" width="478" height="287" /></p>
<p>Notational Velocity has an extremely simple interface. In fact, that’s probably its strongest “feature.”  It is truly designed to be a frictionless medium through which thoughts pass freely from wetware to software.</p>
<p>The search field in Notational Velocity is pure brilliance.  It doubles as a “create new note” field, for lack of a better term. You can simply start typing anything, and Notational Velocity will show notes that match your keywords. Or you can type the title of a new note, hit RETURN, and instantly begin writing. Your fingers never have to leave the keyboard.</p>
<p>Notational Velocity’s search field met another need I had on my Mac: the ability to instantly capture a thought with just a few keystrokes.  Even with TextEdit, I would have to open TextEdit, type something, then “save as.” I would have to make a decision about where I wanted to save the file. With Notational Velocity, all I have to do is invoke LaunchBar (CMD+SPACE), type NV, type a title, and press RETURN.  There are no decisions about where to save the file, and I know I can easily retrieve it later.</p>
<p>In the pre-digital world, Notational Velocity would be like having a pen and notepad handy and magically being able to file it instantly–and recall it at a moment’s notice later on. It’s actually quite interesting that despite all that computers allow us to do, they took away the ability to jot down a quick note, perhaps the most basic step toward conveying human creativity.</p>
<p>As a side “note,” I had been using <a href="http://www.evernote.com/">Evernote</a> for this purpose for a while, but I’m finding that I favor Notational Velocity for writing my own thoughts and Evernote for capturing other random bits of information, like web clippings.</p>
<h2 id="bringinghazelbackintothepicture">Bringing Hazel back into the picture</h2>
<p>In my last post on MultiMarkdown, I was really plugging Hazel and its ability to automate the creation of HTML documents from MultiMarkdown files. The Markdown preview pane in Steve’s version of Notational Velocity shows you a preview of the HTML. This is great for previewing, but I still needed way to actually copy the HTML code (so I could post it to the web).</p>
<p>Fortunately, Hazel is still able to take care of this for me.</p>
<p>I quickly realized that since Notational Velocity allows you to archive your notes as individual text files, I could take advantage of file name changes to trigger Hazel.  I’m sure I will massage my taxonomy a bit in the future, but right now I have a system that makes a lot of sense to me.</p>
<h2 id="hownotationalvelocityandhazelplaytogetherforme">How Notational Velocity and Hazel play together (for me)</h2>
<p>When I first start writing something bound for the web, like a blog post, I begin the name of the note with “draft.”  For example, “draft Notational Velocity MultiMarkdown.” This has the benefit of keeping my drafts grouped together if I sort my notes by title.</p>
<p>As I write a note, I like to keep the <span style="text-decoration: line-through;">Multi</span>Markdown pane pulled down so that I’m only seeing the text I type.  It’s like pulling the shades down for better concentration.</p>
<p>As I near completion, or if I want see how things are coming out, check link references, etc., I pull the <span style="text-decoration: line-through;">Multi</span>Markdown pane back up and read over things. It’s really great being able to preview the HTML.</p>
<p>When I’m happy with the result, I replace “draft” in the note name with “pub” for publish.  I created a new Hazel rule that’s triggered anytime Hazel sees a new file beginning with “pub” in my Notational Velocity notes folder on my Mac.</p>
<p>When Hazel sees the new pub file, it copies it to a folder I created called PublishHTML.  When Hazel sees new TXT files arrive in PublishHTML, it generates an HTML version using the <a href="http://www.practicallyefficient.com/2010/05/19/my-multimarkdown-writing-workflow-with-launchbar-and-hazel/">same kind of rule I described in my last post</a>.</p>
<p>Finally, another Hazel rule runs every so often to clean out the PublishHTML folder since it’s really being used temporarily.</p>
<p>Overall, I like this process much better for these reasons:</p>
<ul>
<li>Writing in Notational Velocity’s interface is really appealing</li>
<li>Hazel runs less often–only when I’m ready to create the final HTML document</li>
<li>My drafts are stored in Notational Velocity and can be easily located at any time using the fantastic search built into Notational Velocity</li>
<li>I can sync Notational Velocity with Simplenote. This allows me to edit my drafts on my iPad, iPod Touch, or really anywhere I have an internet connection. (Simplenote is a must-have if you do anything with Notational Velocity.)</li>
<li>I also keep my Notational Velocity notes folder in <a href="http://www.dropbox.com">Dropbox</a>, which gives me an easy way to restore files and also gives me another way to access files on the go. Note: You should only use Dropbox or Simplenote (not both) to keep your notes in sync across multiple Macs.</li>
</ul>
<h2 id="abitofextraapplauseforsimplenote">A bit of extra applause for Simplenote</h2>
<p>It’s worth emphasizing the convenience of <a href="http://simplenoteapp.com/">Simplenote</a>, a free service that syncs text-based notes created in the Simplenote iPad / iPhone app with servers. The syncing is seamless and fast. To my knowledge, it’s the first step toward Dropbox-like editing on the iPad. If I change anything in Simplenote, the changes are almost immediately available within Notational Velocity on my Mac. They also have a <a href="https://simple-note.appspot.com/login.html">web interface</a>, so you can access your notes anywhere you have an internet connection.</p>
<p>So thanks to CraigM for giving me another nudge toward Notational Velocity.  And a big thanks to Steve Frank for adding the Markdown preview pane.</p>
<p>By the way, Notational Velocity, Simplenote, and Dropbbox, are all completely free in their basic versions.  There’s no reason not to try them if you’re interested.  Please let me know how you like them or if you have any writing workflow tips of your own.</p>
<h2 id="onemorething">One more thing</h2>
<p>After I wrote this post, <a href="http://www.practicallyefficient.com/2010/05/19/my-multimarkdown-writing-workflow-with-launchbar-and-hazel/#comment-50">John Chandler</a> left a comment on my last post describing exactly the same process I outlined above. I’m glad someone else has stumbled across the same workflow, and it really affirms my decision to move into Notational Velocity as my primary MultiMarkdown text editor.</p>
<p>The comments on MultiMarkdown and Notational Velocity have been great. I look forward to hearing about other creative uses of these simple, but powerful tools.</p>
