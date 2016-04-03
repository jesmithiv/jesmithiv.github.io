---
layout: post
title: More than 50 years of persecution
redirect_from: /home/2012/09/14/more-than-50-years-of-persecution/index.html
---
<p>"My problem is that I have been persecuted by an integer."</p>

<p>So begins one of the most famous papers in the history of psychology. George A. Miller's <a href="http://www.musanim.com/miller1956/">seminal 1956 paper</a> "The Magical Number Seven, Plus or Minus Two: Some Limits on our Capacity for Processing Information" is widely interpreted to suggest that the typical human can only hold seven objects—give or take two—in working memory at a time.</p>

<p>Practical implementations of the "magical number seven" can be found throughout modern society, the most common example being phone number formats (###-####).</p>

<p>Miller addressed several aspects of human memory in his paper, which, by the way, is very entertaining to read given that it was originally intended to be an oral presentation. </p>

<p>He was particularly interested in experiments that sought to quantify a human's maximum channel capacity using bits, which he defined as follows:</p>

<blockquote>
  <p>One bit of information is the amount of information that we need to make a decision between two equally likely alternatives. If we must decide whether a man is less than six feet tall or more than six feet tall and if we know that the chances are 50-50, then we need one bit of information. </p>
</blockquote>

<p>Sound familiar?</p>

<p>Yes, the use of bits predates our modern networks. But for me, Miller's paper seemed especially prescient, given that I've been thinking a lot about the practical limits of my own channel capacity when it comes to the way <em>I</em> interface with computer encryption systems.</p>

<p>In other words: my ability to recall secure passwords.</p>

<h2 id="chunking">Chunking</h2>

<p>As is often the case after I read something interesting, I look for more. In this case, I wasn't surprised to find tracks ahead of me in the sand. A few web searches later, I found the work of <a href="http://web.missouri.edu/~cowann/docs/articles/in%20press/Cowan%20et%20al,%20Tall%20tales%20in%20press.pdf">Nelson Cowan, et al.</a>, who argue that Miller wasn't as infatuated with the number seven as many think.</p>

<p>Rather, Miller was quite intrigued with the concept of "chunking," which is the act of putting multiple items together into distinguishable groups as a memory device.</p>

<p>Further whetting my appetite for password applications was this example provided by Cowan, et al.:</p>

<blockquote>
  <p>Another example that makes the concept clear is memorization of the letter string USAFBICIA. This looks like 9 chunks (single, unrelated letters) but they can be reduced to three acronyms: USA (United States of America), FBI (Federal Bureau of Investigation), and CIA (Central Intelligence Agency). For someone who knows these acronyms by heart and notices these patterns, there are only 3 chunks to be remembered.</p>
</blockquote>

<h2 id="chunkingandpasswords">Chunking and passwords</h2>

<p>Chunking Theory was actually applied directly to password strategies by <a href="http://jiito.org/articles/JIITOv1p097-113Carstens30.pdf">Deborah S. Carstens, et al.</a>, who were interested in finding secure passwords that employees of security-conscious organizations could remember.</p>

<p>Not surprisingly, they found that "a password comprised of meaningful chunks is easier to recall than a password with random data, even if the password contains additional characters."</p>

<p>Carstens, et al. came up with several password templates that employees could fill in, so to speak, with information meaningful to them. The longest password resulted from a four-chunk formula where study participants had to select "two meaningful dates that weren’t easily accessible to the public using a symbol of choice to be used as day/month/year separators" and then "two sets of initials that contained at least one uppercase and one lowercase letter." That's 2 + 2 = 4 chunks.</p>

<blockquote>
  <p>An example of a Four-Chunk Password Level Experiment password is “08#11#71Lg12#11#81kd.” The first chunk is “08#11#71” which stands for “August 11, 1971.” The second chunk is “Lg” which stands for “Laura Green.” The third chunk is “12#11#81” which stands for “December 11, 1981.” Lastly, the fourth chunk is “kd” which stands for “Kyle Doyle.”</p>
</blockquote>

<p>Just like a computer can parse a string using delimiters, I think the human mind can parse (and consequently recall) longer passwords when those passwords are broken up by a delimiter like the hash symbol in the example above.</p>

<p>The added advantage, in the context of passwords, of using a symbol as a delimiter is that the password appears even more random to people (and machines) with no contextual knowledge of the underlying process used to form the chunks.</p>

<h2 id="butwhataboutpasswordmanagementsystems">But what about password management systems?</h2>

<p>I am very much of the mind that a good password management system is critical in modern life. Once I bought <a href="https://agilebits.com/onepassword">1Password</a>, I gladly gave up trying to remember passwords for the hundreds of credential-requiring sites I visit. Letting a program create and remember long, random passwords for me so that I don't have to just makes sense.</p>

<p>But a password manager can't eliminate the need to remember all passwords. At a minimum, you still need to know the master password to the password manager itself. And arguably, this master password should be the most difficult to hack of all—given that it's the key to all the other keys.</p>

<p>Ignoring all of the other practical benefits of a solid password management application like 1Password, I feel, in a sense, in the same place I started, which is trying to solve the classic password optimization problem:</p>

<p><em>Maximize the security of my password(s) subject to the limits of my natural channel capacity.</em></p>

<p>And evolution has given me just a few precious bits to work with.</p>

<h2 id="itsadauntingproblem">It's a daunting problem</h2>

<p>There is no easy answer to this. I would argue that there isn't a "solution" at all. At least not in the sense that I can ever create a password that is completely invincible to any and all forms of password cracking techniques.</p>

<p>The game of password security is only getting more sophisticated. So much so that I bet few people understand just what we—as limited channel capacity and slow-to-evolve beings—are up against.</p>

<p>I like how AgileBits, the maker of 1Password, <a href="http://blog.agilebits.com/2011/06/21/toward-better-master-passwords/">characterizes the game</a>: </p>

<blockquote>
  <p>The strength of a password creation system is not how many letters, digits, and symbols you end up with, but how many ways you could get a different result using the same system.</p>
</blockquote>

<p>In other words, a crazy-long 64-character password isn't very secure if it can be "solved for" in a variety of ways. The more paths to a solution, the more likely the solution will be found.</p>

<h2 id="backtochunking">Back to chunking</h2>

<p>Clearly we humans don't have the channel capacity to recall a random string of 64-characters, and so the only way we would ever be able to carry around such a string in our minds is by chunking. But if we use well-known chunks, the absolute length of the password becomes less relevant. </p>

<p>In the same AgileBits post I quoted above, the author, Jeff, lists several really good tips for building strong master passwords. For example, using a phrase that doesn't make numerical sense: "I have 35 bats: Larry, Moe &amp; Curly." But:</p>

<blockquote>
  <p>For those of us of a certain age and steeped in American culture, once we begin a list of names with “Larry…” following it with “Moe and Curly” is very predictable. So even though the Moe &amp; Curly add 11 characters to the password, those 11 characters are so predictable that they add very little actual strength. Even though it is shorter, using I have 35 bats: Larry &amp; Amy is actually stronger than I have 35 bats: Larry, Moe &amp; Curly.</p>
</blockquote>

<p>In other words, "Larry, Moe &amp; Curly" isn't really 18 characters. It's just a single chunk—a really well-known one at that. Easily guessed chunks effectively collapse the length of a password for a hacking algorithm.</p>

<h2 id="whereiamtoday">Where I am today</h2>

<p>I can't avoid having to store a handful of passwords in my head. For those, I try to use my own personal and silly brand of Chunking Theory. Chunking is by far the most practical method I've found for creating long, yet memorable-to-me passwords. </p>

<p>Hopefully by using creative chunks and mixing delimiters, I can keep my passwords strong but only a few bits in size so they fit through my naturally narrow channel.</p>

<p>But something tells me that no matter what I do, I will continue to be persecuted. . . by a password.</p>
