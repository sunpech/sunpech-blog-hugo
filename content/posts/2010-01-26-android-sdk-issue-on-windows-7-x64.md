---
author: "Steven Suwatanapongched"
blogger_id: tag:blogger.com,1999:blog-6841384.post-6014119442015021448
blogger_orig_url: https://www.sunpech.com/2010/01/android-sdk-issue-on-windows-7-x64.html
date: '2010-01-26T18:59:00.000-06:00'
headerimage: /images/headers/android.jpg
modified_time: '2014-08-07T20:14:24.526-05:00'
redirect_from: /2010/01/android-sdk-issue-on-windows-7-x64.html
tags:
  - Android
  - Guide
  - Software Development
  - Technology
old_thumbnail: https://3.bp.blogspot.com/_7U5MdumP-no/S1-JuvXb-TI/AAAAAAAAOEc/-7CpDZMLDBA/s800/Android_error_message_64bit.jpg
thumbnail: /images/blog/tn_default.jpg
title: Android SDK issue on Windows 7 x64
---


I recently installed the [Android SDK](https://developer.android.com/sdk/) and [Eclipse](https://www.eclipse.org/downloads/) (32-bit) onto my Windows 7 Ultimate 64-bit machine.  First thing I wanted to do was go through the [Android Hello World Tutorial](https://developer.android.com/guide/tutorials/hello-world.html).

Well, I ran into the following error message:



> 'java' is not recognized as an internal or external command, operable program, or batch file.  SWT folder '' does not exist.  Please set ANDROID_SWT to point to the folder containing swt.jar for your platform.


![Android Error Message 64-bit](/images/blog/Android_error_message_64bit.jpg)


I read somewhere that I should install the x64 Java version.  However, when I went to [Java download page](https://www.java.com/en/download/manual.jsp), it didn't even have the x64 version available to download.  Turns out that the problem was that I was using [Google Chrome](https://www.google.com/chrome) to browse there.  I had to use Internet Explorer (x64 bit version) to get the x64 Java link to even show up!

This worked for me, but you can check out the following link at StackOverflow: [https://stackoverflow.com/questions/1919340/android-sdk-setup-under-windows-7-pro-64-bit](https://stackoverflow.com/questions/1919340/android-sdk-setup-under-windows-7-pro-64-bit)