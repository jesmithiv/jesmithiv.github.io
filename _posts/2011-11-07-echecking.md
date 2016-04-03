---
layout: post
title: A Bank of America rant, then online check deposit made easy with Hazel and
redirect_from: /home/2011/11/07/echecking/index.html
---
<p>Years ago, I opened a checking account with Bank of America thinking that their nearly ubiquitous ATM presence would make my life easier. I figured that lots of ATMs meant fast and easy access to my account.</p>
<p>In practice I’ve found that every aspect of the Bank of America ATM experience is about waiting.</p>
<p>It seems that none Bank of America's top brass have ever visited an actual brick and mortar branch. If they had, they would surely notice that virtually none of their outdoor customers drive through human teller lanes anymore.</p>
<p>It’s not unusual at all, particularly in the southeast, where I live, to find four empty teller lanes and five or more people in line at a single ATM.</p>
<p>Maybe I’m living in an alternate reality. Maybe Bank of America tellers have unionized against ATMs. Maybe, using Bernoulli's Principle, bank branch architects rely on the drive-through structure to keep the building from collapsing.</p>
<p>I don’t know. I’m just tired of waiting in line while I watch the wind blow through spaces that would have been occupied by cars in the 20th century—cars that are now in front of me, wanting the same single ATM I do.</p>
<p>Even when your turn finally arrives, using a Bank of America ATM is about waiting. There are noticeable Windows Vista-esque delays between screen transitions, especially when depositing checks.</p>
<p>All that to say, I’m not too keen on the Bank of America ATM experience.</p>
<p>So I’m moving my checking account to Ally Bank, an all-online outfit. Not only does Ally reimburse all foreign ATM fees, they just started offering online check deposit. So far we are getting along really well. Ally works the way I need a 21st century bank to work.</p>
<h2 id="depositingcheckswithhazelandautomator">Depositing checks with Hazel and Automator</h2>
<p>When I scan checks front and back, my <a href="http://www.amazon.com/gp/product/B004ISGG7Q/ref=as_li_ss_tl?ie=UTF8&amp;tag=practiceffici-20&amp;linkCode=as2&amp;camp=217145&amp;creative=399349&amp;creativeASIN=B004ISGG7Q">ScanSnap S1100</a> naturally creates a two-page PDF. Ally requires that checks be scanned to 300 dpi JPEG format, and the front and back must be uploaded as separate images.</p>
<p>I wanted to way to convert the PDF into two separate JPEGs quickly.</p>
<p>I created a <a href="http://www.noodlesoft.com/hazel.php">Hazel</a> rule that looks on my Desktop for PDFs that start with “Ally Check”. When Hazel spots one, it sends the PDF to an Automator workflow that converts the two-page PDF into two individual JPEG files. After that, Hazel moves the PDF to the trash.</p>
<p>Thanks to Hazel and Automator, I have a front and back JPEG of my check within split seconds of saving the PDF scan to my Desktop. Way faster than spending gasoline and time at a Bank of American ATM.</p>
<p>The Automator workflow:</p>
<p><img style="display: block; margin-left: auto; margin-right: auto;" title="pdf-to-jpeg-pe.png" src="/img/pdf-to-jpeg-pe.png" border="0" alt="Pdf to jpeg pe" width="566" height="499" /></p>
<p>The Hazel rule:</p>
<p><img style="display: block; margin-left: auto; margin-right: auto;" title="hazel-pdf-to-jpeg-pe.png" src="/img/hazel-pdf-to-jpeg-pe.png" border="0" alt="Hazel pdf to jpeg pe" width="532" height="276" /></p>
<p><em>Credit to <a href="https://discussions.apple.com/thread/1456558?start=0&amp;tstart=0">Simon Hobbs</a> for some tips that make the Automator workflow… work.</em></p>
