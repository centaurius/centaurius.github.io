---
layout:     post
title:      "HaveUReddit?  A chrome extension made at HackBU 2016"
subtitle:   "Discover what's trending on reddit with our wordcloud and data analytics chrome extension."
date:       2016-02-13 20:17:35
author:     "Hamilton A. White"
header-img: "img/banner.png"
---

<h1 class="section-heading">HaveUReddit: Developed in 24 hrs at HackBU 2016</h1>

<h3 class="section-heading">So, what is it and what does it do?</h3>
<p>So glad you asked!  HaveUReddit is an implementation of python running in a chrome extension which interfaces to reddit and displays the most trending phrases on your current subreddit.  Once installed in chrome, just hit the blue and purple reddit hexagon on the bookmarks bar, to see what's trending!</p>

<p>We'll get into the technical stuff later, but you can try it out right now by going to the <a href="https://github.com/centaurius">Centaurius</a> github project page and download the chrome extension from our 'releases' folder. </p>

<h3 class="section-heading">Done?  Cool, let's move on to the coding!</h3>

<p>HaveUReddit is a project that is composed of many different elements.  In short, upon clicking the application, the extension loads up an instance of python in the background, polls the current subreddit for data on the words used, and removes extraneous/common phrases.  Finally, the remaining words are plotted in a 'word cloud' format...all in python.</p>

<p>To create this extension, our team used: </p>

<ul style="list-style-type:disc">
  <li>Reddit Praw: The Python Reddit API Wrapper</li>
  <li>Matplot Library</li>
  <li>HTML, CSS, JS, Jekyll, Markdown, and Pixlr</li>
  <li>Chrome Developer Framework and Extensions Manager</li>
</ul>



<h5 class="highlight_text">...All in 24 hours!</h5>

<h3 class="highlight_text">Why is this project unique?</h3>

* It pulls data on the comments from a user-defined subreddit.
* It parses through all the text, eliminates the most common phrases or words, and then plots the results as a word cloud based on frequency.
* Unlike other word cloud generators, our algorithm is open source, written in python, complied in Pyjs, and runs within the browser!
* The algorithm can be used on any text file
	 * We've tested this algorithm on Project Gutenberg books, and it had a low time complexity
	 * We made the algorithm from scratch.
 

<h3 class="highlight_text">What have we learned?</h3>
<p>Using python to create algorithms can be fun and a worthwhile endeavor, but cross-compiling to javascript to run the python code in the browser is difficult</p>

<h3 class="highlight_text">Next Steps</h3>
* Optimize code better
* Create a .CRX file of our chrome extension
* Test, retest, and test again
