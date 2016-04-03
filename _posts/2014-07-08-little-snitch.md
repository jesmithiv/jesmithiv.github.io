---
layout: post
title: Using Little Snitch to lower your LTE bill
redirect_from: /home/2014/07/08/little-snitch/index.html
---
<p>Your Mac is a tiny but vociferous habitat amid an even more boisterous biome. The internet is a <em>really</em> loud place.</p>

<p>If you could somehow translate network traffic to an audible frequency, I&#8217;m sure it would sound like a rainforest of monkeys, tropical birds, frogs, bugs, and God knows what other creatures screaming out incessantly in a programed ritual of information mating.</p>

<p>But how loud <em>should</em> your Mac be? Who should it be allowed to cavort with?</p>

<p>Enter <a href="http://www.obdev.at/products/littlesnitch/index.html">Little Snitch</a>—a Mac application that alerts you any time any application on your Mac attempts to connect to the internet. You&#8217;re able to allow or deny connections on a permanent or temporary basis. Little Snitch groups these &#8220;rules&#8221; into profiles that can be network-specific or global. Best of all, as you join new networks, Little Snitch lets you assign them to profiles.</p>

<p>I use three Little Snitch profiles to muzzle the monkeys:</p>

<ol>
<li><strong>Home</strong>: My home network, including Wi-Fi and ethernet connections</li>
<li><strong>Public Wi-Fi</strong>: Any open or public network I join</li>
<li><strong>LTE</strong>: Any network created by my iPhone or iPad&#8217;s hotspot feature</li>
</ol>

<h2 id="myhomeprofile">My Home Profile</h2>

<p>On my home network profile, anything goes. I don&#8217;t have any data caps or security concerns at home, so I generally cut things loose. If home were the only twig in the internet rainforest I sat on, I probably wouldn&#8217;t need Little Snitch at all—though I do like how the menubar icon shows me if something is doing a lot of uploading or downloading.</p>

<h2 id="mypublicwi-fiprofile">My Public Wi-Fi Profile</h2>

<p>If my home network is a tranquil pond of koi, public Wi-Fi is a muddy swamp full of piranha and pythons—with panthers patrolling the perimeter.</p>

<p>My Public Wi-Fi profile is much more restrictive. I&#8217;ve locked down just about everything <em>except</em> essential services, web browsing, and email. If I <em>must</em> connect to a public network, I want as little information flowing in and out of my Mac as possible.</p>

<h2 id="mylteprofile">My LTE Profile</h2>

<p>When connected to LTE, the concern isn&#8217;t privacy predation. It&#8217;s data usage. And boy, does Little Snitch really help here.</p>

<p>Before I started using Little Snitch a few months ago, I was routinely running right up against my Verizon Wireless data limit around the 23rd day of each month&#8217;s billing cycle. My options were 1) impose a moratorium on LTE usage the last week of the month, 2) go over my limit and incur an overage charge, or 3) increase my data limit.</p>

<p>I stubbornly never chose option (3), meaning that every month I either had to give up the benefits of LTE or give up more money to keep using LTE.</p>

<p>I knew that <a href="http://www.backblaze.com">Backblaze</a>, my preferred online backup service, was part of the problem. Backblaze currently offers no way of restricting backups by network.<a href="#fn:fb" id="fnref:fb" title="see footnote" class="footnote">1</a>  And my Mac currently offers no way to change the behavior of applications on a network-by-network basis. As far as my Mac is concerned, a Wi-Fi network fed by LTE data is the same as any other Wi-Fi network.</p>

<p>To reduce the bleeding, I had to remember to manually pause Backblaze when connecting by LTE, and I frequently did <em>not</em> think to do that until it was too late.<a href="#fn:f1" id="fnref:f1" title="see footnote" class="footnote">2</a> </p>

<p>Now, Little Snitch essentially does the pausing for me. It&#8217;s as simple as permanently blocking <code>bztransmit</code> the first time it tries to connect over LTE.</p>

  
      <img src="/img/img.png" alt=""/>
  

<p>As soon as I began using Little Snitch this way, my LTE data usage issues went away completely. In fact, I barely climb above 2.5 GB of LTE data usage in any given month. Before, I would end up anywhere from 4.0 to 4.5 GB, putting me at or over my 4 GB plan.</p>

<p>Little Snitch lets me use just enough LTE on my Mac to be productive—mostly low-bandwidth web browsing and email.</p>

<h2 id="mypayoff">My Cash Flow Profile</h2>

<p>The economics here are what one might call intuitive. Little Snitch costs $35 <em>once</em>, and it saves me $10-15 <em>every month</em>. If you regularly hop across different networks, which each pose unique security and data usage challenges, I highly recommend trying out Little Snitch.</p>

<div class="footnotes">
<hr />
<ol>

<li id="fn:fb"><p>To be clear, this is not a criticism of Blackblaze. I HIGHLY recommend using Backblaze for bulk online backup. We just live at a time when mobile data isn&#8217;t yet a fully capable peer (cost-wise) compared to non-mobile networks.<a href="#fnref:fb" title="return to article" class="reversefootnote">&#160;&#8617;</a></p></li>

<li id="fn:f1"><p>To a lesser extent, Dropbox can also be a data hog, so I usually block Dropbox by default and allow it on an exception basis. Most of my Dropbox work involves text files, so the bandwidth is pretty low. However, I&#8217;ve taken data hits in the past when someone else added a large amount of data to a shared folder and Dropbox synced the data while I was connected to LTE. With Little Snitch always watching, there&#8217;s no need to worry about these unforeseen data traffic bursts.<a href="#fnref:f1" title="return to article" class="reversefootnote">&#160;&#8617;</a></p></li>

</ol>
</div>
