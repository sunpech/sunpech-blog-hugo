---
author: "Steven Suwatanapongched"
blogger_id: tag:blogger.com,1999:blog-6841384.post-3702960488134665177
blogger_orig_url: https://www.sunpech.com/2008/09/math-behind-tinyurl.html
date: '2008-09-30T00:33:00.000-05:00'
headerimage: /images/headers/technology.jpg
modified_time: '2012-01-03T03:40:21.142-06:00'
redirect_from: /2008/09/math-behind-tinyurl.html
tags:
  - Technology
thumbnail: /images/blog/tn_default.jpg
title: The Math behind TinyURL
---


[TinyURL](https://www.tinyurl.com) is a website that condenses a submitted URL, usually a long one, into a short readable URL on tinyurl's website. In turn, this shorter URL then redirects to the original url.  This is quite handy.

As of this writing, the text below their logo reads:

> Making long URLs usable! More than 90 million of them. Over 1.5 billion hits/month.

From what I've seen, they only use letters and numbers.  So that gives us 26 possible letters, which are not case-sensitive (in other words, "A" is the same as "a").  There are 10 numbers then, zero through nine (0-9).  So through TinyURL's website, that gives us 36 possible links that are of 1 character length.  To get number links of length 2, we would multiply the total possible of the first character by the total possible of the second character, luckily they're the same, so 36 x 36 = 1296.  For each additional, we again multiply by 36.  If n is the number of characters, then the formula can be represented by 36^n, also read 36 raised to the power of n.  Mathematically it's represented as 36^n.

So one of the things I'm wondering is, how long before the tiny url isn't so tiny anymore?  

As of this writing, they have reached the 90 million (90,000,000) range.  So let's see how big this gets:

*1 character = 36^1 = 36 possible*\
*2 characters = 36^2 = 1296*\
*3 characters = 36^3 = 46,656*\
*4 characters = 36^4 = 1,679,616 (over 1 million)*\
*5 characters = 36^5 = 60,466,176*\
*6 characters = 36^6 = 2,176,782,336 (over 2 billion)*\
*7 characters = 36^7 = 78,364,164,096*\
*8 characters = 36^8 = 2,821,109,907,456 (over 2 trillion, approaching 3 trillion)*

So they just passed using 5 characters and are at 6 characters.  Getting to 7 or 8 characters may take a while still.  According to this Google Search, in 2006 Google has indexed over 25 billion web-pages.  So we're not even at the trillion mark just yet!

Plus, this isn't meant for everyone to use to index their page.  But for giggles, let's see what adding a few more characters will yield us.

*9 characters = 36^9 = 101,559,956,668,416*\
*10 characters = 36^10 = 3,656,158,440,062,976 (over 3 quadrillion!)*\
*11 characters = 36^11 = 131,621,703,842,267,136*\
*12 characters = 36^12 = 4,738,381,338,321,616,896 (over 4 quintillion!)*

So each new character that is added adds a significant amount to the upper limit on number of URLs.  They won't need to add too many characters at our current pace!  Wow, isn't math fun?!