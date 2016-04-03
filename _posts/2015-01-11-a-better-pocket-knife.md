---
layout: post
title: A better pocket knife with Launch Center Pro and Pythonista
redirect_from: /home/2015/01/11/a-better-pocket-knife/index.html
---
<p>As nice as it is to write a for-my-eyes-only script to solve a specific problem on my Mac, it is satisfying in an entirely new way to write code on a mobile device. It just feels less like "programming" and more like making a better pocket knife.</p>

<p><strong>A mundane problem I wanted to solve:</strong></p>

<p>I love budgeting, but not as much as I love food. It's always been a struggle for me to manage what I'm spending eating out over the course of a month—especially since what my family and I spend at restaurants tends to vary a lot in size and frequency.</p>

<p>It's easy to set a food budget at the <em>beginning</em> of the month, and it's easy to see whether we came in under or over that budget at the <em>end</em> of the month, but it's a lot harder to ascertain whether or not I'm on track as the days of the month tick by.</p>

<p><strong>The pocket knife solution:</strong></p>

<p>I wrote a simple Python script in <a href="https://itunes.apple.com/us/app/pythonista/id528579881?mt=8">Pythonista</a> that takes a monthly dollar figure—my remaining food budget for the month—and averages it over the remaining days in the current month:</p>

<pre><code>
import datetime, calendar
import sys
import console

budget = float(sys.argv[1])

d = datetime.datetime.today().day
m = datetime.datetime.today().month
y = datetime.datetime.today().year
last = calendar.monthrange(y,m)[1]

remaining_per_day = budget / (last - d)
message = 'You have $' + str(round(remaining_per_day,2)) + ' remaining per day for the next ' + str(last - d) + ' days.'

console.clear()
print message
</code></pre>

<p>The Python script itself is fairly unremarkable, but what impressed the hell out of me is that I was able to write it entirely on my iPhone, then slap a "GUI" on it using <a href="https://itunes.apple.com/us/app/launch-center-pro/id532016360?mt=8">Launch Center Pro</a>. </p>

<p>I don't even have to open Pythonista to use it. I just tap a Launch Center Pro action, enter a dollar figure, and Launch Center Pro sends it to Pythonista, which runs the script and puts an answer in the console.</p>
  
      <img src="/img/img.gif" alt=""/>
  

<p>This little workflow takes advantage of Pythonista's ability to <a href="http://omz-software.com/pythonista/docs/ios/urlscheme.html">accept standard input via its URL scheme</a> and Launch Center Pro's ability to send a URL that consists partly of numeric keypad input.</p>
  
       [caption id="" align="alignnone" width="400.0"]<img src="/img/img.png" alt="In LCP's action settings, enter Pythonista's URL scheme in the URL field along with [prompt-num], which is LCP's variable for keypad input. The name of the Python script in this example is Budget.py."/> In LCP's action settings, enter Pythonista's URL scheme in the URL field along with [prompt-num], which is LCP's variable for keypad input. The name of the Python script in this example is Budget.py.[/caption] 
  

<p><strong>This was a mundane problem, but the solution feels remarkable.</strong></p>

<p>To me, Pythonista is a very important app because it feels like an obvious step toward a future where more software creation will happen on devices that we don't think of as "computers" in the conventional sense.</p>

<p>Maybe I'm overblowing all this, but I just think it's amazing that I can write a piece of code on a mobile device, then snap a few blocks together to essentially create a custom app. I can't help but think the future of programming won't feel like "programming"—much like using an iPhone doesn't feel like "computing."</p>

<h2 id="otherresources">Other resources</h2>

<ul>
<li><a href="http://nerdquery.com/search.php?query=Pythonista&amp;search=1&amp;category=24&amp;catid=24&amp;type=and&amp;results=50&amp;db=0&amp;prefix=0&amp;media_only=0">Anything Gabe Weatherhead has written about Pythonista</a></li>
<li><a href="https://duckduckgo.com/?sites=leancrew.com&amp;ka=h&amp;k7=w&amp;kj=%23434843&amp;ky=%23F3FEF3&amp;kx=%23384338&amp;kt=Helvetica&amp;q=Pythonista">Anything Dr. Drang has written about Pythonista</a>, especially <a href="http://www.leancrew.com/all-this/2013/10/simple-expense-report-with-drafts-and-pythonista/">his expense report workflow using Drafts and Pythonista</a></li>
<li><a href="https://brettkelly.org/ios-buffer-sharing-pythonista-launch-center-pro/">Brett Kelly on using Pythonista and Launch Center Pro for better web site sharing</a></li>
</ul>

<p><em>Some of the media elements in this post are best viewed in the <a href="http://www.practicallyefficient.com/home/2015/1/11/a-better-pocket-knife">original</a>.</em></p>
