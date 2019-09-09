---
title: "Migrated Website to Hugo"
date: '2019-09-08T03:03:14-05:00'
Description: "Migrated my blog from Jekyll to Hugo."
tags: ["Software Development", "Technology"]
draft: true
author: "Steven Suwatanapongched"
headerimage: /images/headers/software_development.jpg
image: "/images/blog/hugo-logo.jpg"
images: ["/images/blog/hugo-logo.jpg"]
thumbnail: "/images/blog/tn_hugo-logo.jpg"
disable_feed: true
---

Over the past week I migrated my blog from using static site generator, [Jekyll](https://jekyllrb.com/) to use [Hugo](https://gohugo.io/). I also switched hosts from [Github Pages](https://pages.github.com/) to [Netlify](https://www.netlify.com/).

The main reasons for the changes are:

* Jekyll/Ruby is just too slow as a static site generator in development/production.
* Hugo/Go is fast.
* Wanted to try out Netlify.

When I wrote new posts with Jekyll, it was painfully slow to build the site after any small set of changes. With Hugo, it's really fast. I can pretty much hit command+S, to save all the time and have the page refresh right away.

![Hugo](/images/blog/hugo-logo.jpg)

Overall the project migration went pretty smoothly thanks to [some migration tools](https://gohugo.io/tools/migrations/). I specifically used [ConvertToHugo](https://github.com/coderzh/ConvertToHugo).

Some of the challenges I came across were:

* Updating some front matter for pages and posts.
* Find/replace certain strings to improve site as well as front matter.
* Migrating some Ruby syntax to Go (Hugo).
* Figuring out Hugo scopes.
* Learning how to create/use a theme.
* Getting atom feed to work.

I tried out Netlify for the first time and love it. Their tools and interface was very intuitive for building and deploying was pretty straightforward. I also love how easy it was to set up HTTPS ([Let's Encrypt](https://letsencrypt.org/)) wit them. And like Github Pages, it's all free since I currently have no need for the paid features.

