---
layout: post
title: Wolfram Alpha + LaTeX revisited
redirect_from: /home/2015/08/21/wolfram-alpha-latex-revisited/index.html
---
<p>I <a href="http://www.practicallyefficient.com/home/2014/7/10/latex-alfred-wolfram">mentioned before</a> how useful it can be to evaluate numerical LaTeX expressions with Wolfram Alpha using Alfred. I still do that a lot, but now that I have a Wolfram Alpha pro subscription, I'm spending more time on the WA website itself to take advantage of features like calculation history.</p>

<p>Another benefit of being on the website is being able to visually see how WA interprets the code I enter. This is a fantastic way to verify that I entered the code that I thought I entered—especially for longer expressions that go beyond the visible boundary of the input field.</p>

<p>A recent example: I wanted to evaluate:</p>

<pre><code>\frac{1677 - 1251.76}{1 + \frac{(1-0.004)}{1.04} + \frac{(1-0.004)(1-0.005)}{1.04^{2}} + \frac{(1-0.004)(1-0.005)(1-0.006)}{1.04^{3}}  }</code></pre>

<p>The first time I copied this expression into WA, I accidentally missed the very last bracket, probably because there was some extra space in front of it.</p>
  
      <img src="/img/img.png" alt=""/>
  

<p>I was able to quickly see that something was wrong since I intended the <code>1677 - 1251.76</code> term to be in the numerator. </p>

<p>So I tried again, making sure to capture all of the code, and got what I was looking for, including the numerical value of the expression, 113.41.</p>
  
      <img src="/img/img.png" alt=""/>
  

<p>Being able to evaluate these expressions on the fly is a godsend and greatly reduces the chances for typos in the final document. As an added bonus, since WA generates a unique URL for each query, I can copy it into my <code>.tex</code> file as a comment for later reference. For example, <a href="http://www.wolframalpha.com/input/?i=%5Cfrac%7B1677+-+1251.76%7D%7B1+%2B+%5Cfrac%7B%281-0.004%29%7D%7B1.04%7D+%2B+%5Cfrac%7B%281-0.004%29%281-0.005%29%7D%7B1.04%5E%7B2%7D%7D+%2B+%5Cfrac%7B%281-0.004%29%281-0.005%29%281-0.006%29%7D%7B1.04%5E%7B3%7D%7D++%7D">here's the calculation above</a>.</p>
