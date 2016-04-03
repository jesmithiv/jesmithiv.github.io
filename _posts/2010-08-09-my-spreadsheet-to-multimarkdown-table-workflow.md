---
layout: post
title: My spreadsheet to MultiMarkdown table workflow
redirect_from: /home/2010/08/09/my-spreadsheet-to-multimarkdown-table-workflow/index.html
---
<p>If you’ve ever tried to make a table in a word processor or spreadsheet, then “save as HTML,” you know what a mess you get.
Thanks to <a href="http://fletcherpenney.net/">Fletcher Penney</a>, however, we have <a href="http://www.practicallyefficient.com/tag/multimarkdown/">MultiMarkdown</a>, which makes creating HTML tables easy.</p>
<p>I haven’t exiled the spreadsheet from my HTML table workflow, however.  I’ve just recast it in a new role and paired it with  MultiMarkdown.  I’ll show you how too, but first, just for a little perspective (if drama), let’s look at just what a mess you get when you use Excel or Word the conventional way.</p>
<p><!--more-->I wanted to make this simple, innocuous-looking (but information-rich) 6x3 table:</p>
<table>
<col align="left"></col>
<col align="right"></col>
<col align="right"></col>
<thead>
<tr>
<th>Animal</th>
<th>Legs</th>
<th>Lives</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">Dog</td>
<td align="right">4</td>
<td align="right">1</td>
</tr>
<tr>
<td align="left">Cat</td>
<td align="right">4</td>
<td align="right">9</td>
</tr>
<tr>
<td align="left">Monkey</td>
<td align="right">2</td>
<td align="right">1</td>
</tr>
<tr>
<td align="left">Kangaroo</td>
<td align="right">2</td>
<td align="right">1</td>
</tr>
<tr>
<td align="left">Total</td>
<td align="right">12</td>
<td align="right">12</td>
</tr>
</tbody>
</table>
<p>Trying Excel first,  I entered the words and numbers in plain text – no formatting at all – then I saved it as an HTML file.  Excel generated a file with 336 lines of code. Word vomited out a whopping 599 lines of HTML.</p>
<p>Bleck.</p>
<p>Even if you copied this bloat into your blog or website, it likely wouldn’t render as expected.  There’s just too much junk in it. It’s not usable.</p>
<h2 id="abetterway">A better way</h2>
<p>MultiMarkdown gives us a simple, intuitive way to make HTML tables without generating an amorphous blob of code.  Instead of remembering HTML table codes, you simply use the pipe symbol | to separate columns.</p>
<p>I talked about MultiMarkdown tables in an <a href="http://www.practicallyefficient.com/2010/03/24/improve-your-web-writing-by-getting-back-to-basics-with-multimarkdown/">earlier post</a>. You can also check out Fletcher Penney’s <a href="http://fletcherpenney.net/multimarkdown/users_guide/multimarkdown_syntax_guide/">MultiMarkdown syntax help page</a> for all the details.</p>
<p>Now given that I just denounced Excel as a practical creator of usable HTML table code, it may surprise you that I’m about to recommend using a spreadsheet. But as I noted above, spreadsheets are still useful for making HTML tables,  just not in the traditional way.</p>
<p>Here are a few reasons I like using spreadsheets to create web-destined tables:</p>
<ul>
<li>Spreadsheets are good at math.  If you’re building a table involving calculations (e.g. sums, counts, averages, etc.), it’s a whole lot easier to let a spreadsheet do the number crunching.</li>
<li>Spreadsheets can be updated quickly.</li>
<li>Spreadsheets are reusable and easily repurposed.</li>
<li>You can make large tables quickly in a spreadsheet using copy, paste, fill, etc.</li>
<li>Spreadsheet rows and columns provide clear boundaries making things easier on your eyes as you build the table.</li>
</ul>
<p>I’m going to illustrate how easy it is to make clean, friendly HTML table code using a Google spreadsheet, though what I’m about to talk about could be done in any spreadsheet program.</p>
<h2 id="thespreadsheettomultimarkdowntableworkflow">The spreadsheet to MultiMarkdown table workflow</h2>
<p><strong>Step 1: Make your spreadsheet table</strong></p>
<p>Keep the formatting light since this is going to end up in a text file anyway.  Just focus on getting your numbers down.  (Of course, you could do this with an existing, prettier table too; doesn’t matter.)</p>
<p><a href="/img/MultiMarkdown-table-1-pe.png"><img class="aligncenter size-full wp-image-905" title="MultiMarkdown-table-1-pe" src="/img/MultiMarkdown-table-1-pe.png" alt="" width="291" height="258" /></a></p>
<p><strong>Step 2: Add MultiMarkdown table header syntax</strong></p>
<p>A MultiMarkdown table must have dashes in the second row.  You can use colons (:) on either side of the dashes to tell MultiMarkdown how to align the columns.</p>
<p>In my example, I’m going to left-align the left-most column and right-align the other two. (Putting a colon on both sides would center things.)</p>
<p><a href="/img/MultiMarkdown-2-pe.png"><img class="aligncenter size-full wp-image-906" title="MultiMarkdown-2-pe" src="/img/MultiMarkdown-2-pe.png" alt="" width="280" height="247" /></a></p>
<p><strong>Step 3: Plumb your table</strong></p>
<p>The pipe symbol tells MultiMarkdown where your table column borders are.  Adding them in a spreadsheet is easy.  Just insert new columns between each of your original spreadsheet table columns with the | character in each cell. Remember, copy, paste, and fill are your friends. Use them to make this go quickly.</p>
<p><a href="/img/MultiMarkdown-3-pe.png"><img class="aligncenter size-full wp-image-909" title="MultiMarkdown-3-pe" src="/img/MultiMarkdown-3-pe.png" alt="" width="303" height="259" /></a></p>
<p><strong>Step 4: Concatenate</strong></p>
<p>Concatenate is a fancy-sounding name for chaining pieces of text together.  Every spreadsheet program I’ve ever used has a concatenate function.  I really like the one in Google Spreadsheets because it accepts a range of text.  You don’t have to enter individual cells.</p>
<p>In column G, I’ve added some concatenate functions (see Formula bar for example) to pull everything together.</p>
<p><a href="/img/MultiMarkdown-4-pe.png"><img class="aligncenter size-full wp-image-911" title="MultiMarkdown-4-pe" src="/img/MultiMarkdown-4-pe.png" alt="" width="438" height="349" /></a></p>
<p>Column G is what we're after.  All we have to do is copy it into our MultiMarkdown file, and we're done. No "save as."</p>
<pre><code>Animal|Legs|Lives
:-----|-----:|-----:
Dog|4|1
Cat|4|9
Monkey|2|1
Kangaroo|2|1
Total|12|12</code></pre>
<p>That doesn’t look very pretty in plain text, but when you convert your text file to HTML, it’ll look just fine – or however your CSS tells it to look on your site.</p>
<table>
<col align="left"></col>
<col align="right"></col>
<col align="right"></col>
<thead>
<tr>
<th>Animal</th>
<th>Legs</th>
<th>Lives</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">Dog</td>
<td align="right">4</td>
<td align="right">1</td>
</tr>
<tr>
<td align="left">Cat</td>
<td align="right">4</td>
<td align="right">9</td>
</tr>
<tr>
<td align="left">Monkey</td>
<td align="right">2</td>
<td align="right">1</td>
</tr>
<tr>
<td align="left">Kangaroo</td>
<td align="right">2</td>
<td align="right">1</td>
</tr>
<tr>
<td align="left">Total</td>
<td align="right">12</td>
<td align="right">12</td>
</tr>
</tbody>
</table>
<p id="yourturn">Oh, and by the way, this table only took up a mere 39 lines of HTML code using MultiMarkdown. That's less than 12% of Excel and less than 7% of Microsoft Word.</p>
<h2>Your turn</h2>
<p>Share your own HTML table workflows.</p>
