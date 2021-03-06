---
author: "Steven Suwatanapongched"
blogger_id: tag:blogger.com,1999:blog-6841384.post-8659935873398615085
blogger_orig_url: https://www.sunpech.com/2009/01/basic-combinatorial-mathematics.html
date: '2009-01-02T11:58:00.000-06:00'
headerimage: /images/headers/technology.jpg
modified_time: '2012-01-03T03:40:21.168-06:00'
redirect_from: /2009/01/basic-combinatorial-mathematics.html
tags:
  - Technology
thumbnail: /images/blog/tn_default.jpg
title: Basic Combinatorial Mathematics
---


I absolutely love reading [CodingHorror.com](https://www.codinghorror.com).  It's easily one of my favorite blogs to read about problem solving from the viewpoint of a programming/developer.  Recently, Jeff Atwood posted a problem:

> *Let's say, hypothetically speaking, you met someone who told you they had two children, and one of them is a girl. What are the odds that person has a boy and a girl?*

I was surprised by the number of readers who responded who got it wrong, very wrong.  Quite a few who commented answered one-half, 50%.  Reasoning ranged from it's always half, or because the ordering doesn't matter-- and that there are only 3 sets to choose from.  The latter of which I want to discuss.

Note: B = Boy, G = Girl

Some argued that the combinations to work off of is: BB, GG, BG (3 sets)
The full combination is: BB, GG, BG, GB (4 sets, where BG and GB are treated as separate sets)

The 3 set argument is that the BG, GB should be considered as one set, since order does not matter.  But I beg to differ.  Although order (older/younger) was not implied in the problem, it must be considered.  

Here's why:
Having only 3 sets is basically saying that it's equally likely that a couple with two children will have either a Boy-Boy, Girl-Girl, or Boy-Girl set.  This is not true.  It is a 50/50 chance they will have children of the same gender (Boy-Boy or Girl-Girl versus a Boy/Girl combo).  So a full 4 set combo must be used to deduce the answer to the problem.

The answer then, since we know that at least one is a girl, the BB set needs to get tossed out, leaving GG, BG, GB.  So then 2 out of the 3 sets can have boys, so there is a 2/3 chance that the couple's second child is a boy.

### Links:

* [The Problem of the Unfinished Game](https://blog.codinghorror.com/the-problem-of-the-unfinished-game/)
* [Finishing the Game](https://blog.codinghorror.com/finishing-the-game/)