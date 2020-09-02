---
author: "Steven Suwatanapongched"
blogger_id: tag:blogger.com,1999:blog-6841384.post-6486066378930805561
blogger_orig_url: https://www.sunpech.com/2012/01/sopa-blackout-set-for-january-18-2012.html
date: '2012-01-17T18:54:00.000-06:00'
headerimage: /images/headers/technology.jpg
modified_time: '2012-01-17T20:15:26.398-06:00'
redirect_from: /2012/01/sopa-blackout-set-for-january-18-2012.html
tags:
  - Technology
thumbnail: /images/blog/tn_default.jpg
title: SOPA Blackout set for January 18 2012
---


Tomorrow, Wednesday January 18, 2012, I plan to block this website out in support of [SOPA Blackout
SOPA Blackout](https://sopablackout.org/). Technically it won't be completed blocked out, as the javascript is only a black message overlay on top of the website. Users will still be able to click through once the popup comes up.

Here is the javascript that will be used in the header:

```
<script type="text/javascript" src="//js.sopablackout.org/sopablackout.js"></script>
```

On one of my other sites, [spong.org](http://spong.org/), will be blocked out completely using:

```
<script> 
var today = new Date();
if((today.getDate() == 18) && (today.getMonth() == 0) && (today.getFullYear() == 2012)) 
  {  window.location = "https://protestsopa.org"; }
</script>
```

There is a github project for the above: [SOPA-PIPA-Protest-Page](https://github.com/SaraJo/SOPA-PIPA-Protest-Page).