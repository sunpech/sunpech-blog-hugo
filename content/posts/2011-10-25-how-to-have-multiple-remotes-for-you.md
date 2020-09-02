---
author: "Steven Suwatanapongched"
blogger_id: tag:blogger.com,1999:blog-6841384.post-913905597106831886
blogger_orig_url: https://www.sunpech.com/2011/10/how-to-have-multiple-remotes-for-you.html
date: '2011-10-25T12:40:00.000-05:00'
headerimage: /images/headers/software_development.jpg
modified_time: '2014-08-08T16:51:54.686-05:00'
redirect_from: /2011/10/how-to-have-multiple-remotes-for-you.html
tags:
  - Guide
  - Software Development
thumbnail: /images/blog/tn_git-multiple-remotes.jpg
title: How to have multiple remotes for you Git project
---


When I found out that [BitBucket added support for Git](https://blog.bitbucket.org/2011/10/03/bitbucket-now-rocks-git/), I got pretty excited.

Just this past year I started to use [Git](https://git-scm.com/) as my [DVCS](https://en.wikipedia.org/wiki/Distributed_revision_control) for all my projects. More importantly, my older projects didn't have any version control whatsoever. They were projects spread across multiple computers that only merged into a single external USB hard drive when I started to retire some computers because they were just too old (six plus years!).

Anyway, when this external drive began to make noises (clicking sounds), I decided I wanted to have my old projects stored in the cloud in case the the hard drive should ever fail.

[Github](https://www.github.com/) was my goto host as it was immensely popular. At first I was on the free plan (unlimited public repos), but I decided my ugly legacy code shouldn't be public, and went with their [micro plan](https://github.com/plans) ($7 per month for 5 private repos). These projects are retired and there is no plan for future development. I just want them hosted with my other active personal projects.

I signed up for [BitBucket](https://www.bitbucket.org/) not too long ago just because I wanted to play with [Mercurial](https://mercurial.selenic.com/). That didn't last very long. But with the new additional support for Git, and with the free unlimited private and personal projects, I knew I wanted to add this as a remote to also host all my projects.

But how was I to add another remote since I was already using Github? I wanted to add BitBucket as a remote along with Github. With a simple search on [StackOverflow](https://www.stackoverflow.com/], I came across [pull/push from multiple remote locations](https://stackoverflow.com/questions/849308/pull-push-from-multiple-remote-locations/3195446#3195446) (answer).

Here is an example **.git/config** setting, with the bolded text the example text to add a remote:

```
[core]
        repositoryformatversion = 0
        filemode = true
        bare = false
        logallrefupdates = true
        ignorecase = true
[branch "master"]
        remote = origin
        merge = refs/heads/master
[remote "origin"]
        <b>url = git@github.com:sunpech/project_foo.git
        url = git@bitbucket.org:sunpech/project_foo.git</b>
        fetch = +refs/heads/*:refs/remotes/origin/*
[remote "heroku"]
        url = git@heroku.com:project_foo.git
        fetch = +refs/heads/*:refs/remotes/heroku/*
```

Now when I push changes, it pushes it to both Github and BitBucket. Simple, and it works. Hope this helps.

Of course you'll still need to set up the project on each respective host, in which case I'll point you to this [Github setup tutorial](https://help.github.com/mac-set-up-git/) (also see [Using SSH to Access your Bitbucket Repository](https://confluence.atlassian.com/display/BITBUCKET/Using+SSH+to+Access+your+Bitbucket+Repository)).

I have this setup because I may choose to abandon my Github pay account, and just host my public repos there, and all my private repos on BitBucket-- saving me $7/month. Plus, I think it's great for Github to have competition.