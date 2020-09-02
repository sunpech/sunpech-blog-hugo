---
author: "Steven Suwatanapongched"
blogger_id: tag:blogger.com,1999:blog-6841384.post-1451340704159923701
blogger_orig_url: https://www.sunpech.com/2012/11/fixing-android-error-message-error.html
date: '2012-11-15T11:00:00.000-06:00'
headerimage: /images/headers/android.jpg
modified_time: '2014-08-09T19:52:59.212-05:00'
redirect_from: /2012/11/fixing-android-error-message-error.html
tags:
  - Android
  - Guide
  - Technology
old_thumbnail: https://4.bp.blogspot.com/-DbUPW35q1z8/UKQaM0IRF2I/AAAAAAABVvg/ZrAWFQtepXc/s800/A7j94bVCYAI6WZd.png-large.jpg
thumbnail: /images/blog/tn_fix-android-error-message.jpg
title: Fixing an Android Error Message - Error retrieving information from server
---

I have a [Galaxy Nexus](https://en.wikipedia.org/wiki/Galaxy_Nexus) that recently got an over the air (OTA) update to Android 4.2 (Jelly Bean). Coming from 4.1.2 I was thrilled to see the new changes, particularly with their new [panorama feature](https://bgr.com/2012/11/02/android-4-2-ported-galaxy-nexus-photo-sphere/). But after the update I had issues with updating apps on the [Google Play Store](https://play.google.com/store).

### The Problem

I got the following error message:

```
Update for "Foursquare" could not be downloaded due to an error. (Error retrieving information from server. [RPC:AEC:0])
```

![Android Error Message](/images/blog/A7j94bVCYAI6WZd.png-large.jpg)

This would apply to any app, but for my case both Foursquare and Google Music.

I tried a lot of different things from clearing the cache of each of these apps as well as the Google Play app, to even uninstalling the Foursquare app and re-downloading it. None of which worked.

### Solution

In the end, I found [this link](https://blogs.bytecode.com.au/glen/2012/08/02/nexus-play-weirdness-error-retrieving-information-from-server-rpc-aec0.html) which pointed me in the right direction.

The workaround is to simply to go to **Settings-&gt;Accounts&amp;Sync-&gt;Google** and removing my Google account. Afterwards, just add it back again. Then the error message disappeared and I could update/install apps once again.