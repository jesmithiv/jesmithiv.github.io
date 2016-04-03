---
layout: post
title: Evaluating LaTeX code with Alfred and Wolfram Alpha
redirect_from: /home/2014/07/10/latex-alfred-wolfram/index.html
---
<p>The LaTeX documents I create have a lot of numerical illustrations. If you write hundreds (maybe thousands) of numerical expressions in LaTeX over the course of a year, you <em>will</em> fat-finger a few digits along the way, and I <em>really</em> hate typos.</p>

<p>For example, my PDF output might have an expression like this:</p>
  
      <img src="/img/math-pe.png" alt=""/>
  

<p><em>Quick</em>. In your head. . . does that really equal 1.9602? Yeah, I don't want to do that either.</p>

<p>My old fashioned editing approach would be to hand check each one with a calculator like <a href="http://www.acqualia.com/soulver/">Soulver</a>, typing in the expression after it's typeset to PDF and verifying the result. This is because the LaTeX code itself isn't in a format that can be pasted into a typical calculator:</p>

<pre><code>\frac{0.9989 + \frac{0.9975}{1.04}}{0.9989} = 1.9602
</code></pre>

<h2 id="abetterway">A better way</h2>

<p>I only recently found out that <a href="http://www.wolframalpha.com">Wolfram Alpha</a> can evaluate most LaTeX expressions in their raw form. Just paste a LaTeX expression into Wolfram Alpha's text input field, and see what it does.</p>

<p>For an even faster approach—avoiding the need to even leave your favorite LaTeX editor—use the stock "Ask Wolfram" workflow in <a href="http://www.alfredapp.com">Alfred</a>:</p>
  
      <img src="/img/img.png" alt=""/>
  

<ol>
<li>Invoke Alfred</li>
<li>Start typing <code>wolf...</code> to bring up the Wolfram workflow</li>
<li>Paste LaTeX code and <code>return</code></li>
</ol><p>The workflow takes you straight to the Wolfram site, which <a href="http://www.wolframalpha.com/input/?i=%5Cfrac%7B0.9989%20%2B%20%5Cfrac%7B0.9975%7D%7B1.04%7D%7D%7B0.9989%7D">evaluates the expression</a> in a second or two.</p>
  
      <img src="/img/img.png" alt=""/>
  

<p>That's probably enough digits, Wolfram. But anyway, yeah, there's the 1.9602 I was hoping to see.</p>

<p>This is by far the fastest and most accurate way I've found to audit LaTeX numerical expressions on the fly. In fact, I've started using Wolfram Alpha to evaluate expressions in the first place. This lets me type LaTeX expressions as I "think" them and know that I can evaluate them in-line as I go.</p>

<p>Alfred, after all, is always just a <code>Cmd-Space</code> away.</p>

<p><strong>Update:</strong> For ideas on automating this process further with Python, see Dr. Drang's <a href="http://www.leancrew.com/all-this/2014/07/evaluating-latex-with-eddie-and-alpha/">follow-up post</a>.</p>

<p><strong>Update 2:</strong> <a href="http://www.practicallyefficient.com/home/alfred-alpha-awesome">Here's an even faster way</a> to evaulate LaTeX with Alfred and Wolfram.</p>
