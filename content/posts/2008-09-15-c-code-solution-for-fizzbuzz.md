---
author: "Steven Suwatanapongched"
blogger_id: tag:blogger.com,1999:blog-6841384.post-1087262992477565695
blogger_orig_url: https://www.sunpech.com/2008/09/c-code-solution-for-fizzbuzz.html
date: '2008-09-15T22:20:00.000-05:00'
headerimage: /images/headers/software_development.jpg
modified_time: '2012-01-01T23:03:53.750-06:00'
redirect_from: /2008/09/c-code-solution-for-fizzbuzz.html
tags:
  - Software Development
title: A C# Code Solution for FizzBuzz
thumbnail: /images/blog/tn_default.jpg
url: /2008/09/c-code-solution-for-fizzbuzz
---


I read a [slashdot article](https://it.slashdot.org/article.pl?sid=08/09/15/0210235) earlier today which lead me to a Coding Horror article: [Why Can't Programmers.. Program?](https://www.codinghorror.com/blog/archives/000781.html).  This lead me to the FizBuzz problem, which prompted me to write my own quickie solution in C# (as a console application).

### Problem:

*Write a program that prints the numbers from 1 to 100. But for multiples of three print "Fizz" instead of the number and for the multiples of five print "Buzz". For numbers which are multiples of both three and five print "FizzBuzz".*

#### My Quick Solution:

```
for (int i = 1; i &lt;= 100; i++)
{
  if ((i % 3 == 0) &amp;&amp; (i % 5 == 0))
  {
      Console.WriteLine(&quot;FizzBuzz&quot;);
  }
  else if (i % 3 == 0)
  {
      Console.WriteLine(&quot;Fizz&quot;);
  }
  else if (i % 5 == 0)
  {
      Console.WriteLine(&quot;Buzz&quot;);
  }
  else
  {
      Console.WriteLine(i.ToString());
  }

}

Console.ReadLine();
```

I know my version is probably not optimal, nor is it the shortest way to write it.  I just wanted to write it for fun, code for fun.  I honestly can't remember the last time I coded something purely for fun.  Now I'm wondering how I can optimize this in C# and even how to write it in other languages.

Where I formatted my C# code into HTML for Blogspot: [https://formatmysourcecode.blogspot.com](https://formatmysourcecode.blogspot.com)