---
author: "Steven Suwatanapongched"
blogger_id: tag:blogger.com,1999:blog-6841384.post-6665102534805821074
blogger_orig_url: https://www.sunpech.com/2010/08/installing-thai-fonts-onto-android.html
date: '2010-08-30T09:00:00.110-05:00'
headerimage: /images/headers/android.jpg
modified_time: '2014-08-07T20:13:45.291-05:00'
redirect_from: /2010/08/installing-thai-fonts-onto-android.html
tags:
  - Technology
  - Android
  - Guide
old_thumbnail: https://1.bp.blogspot.com/_7U5MdumP-no/THt8iBDVVQI/AAAAAAAAWWA/ppE6gy3cFIw/s800/Screen+shot+2010-08-30+at+4.40.01+AM.png
thumbnail: /images/blog/tn_install-thai-fonts-android.jpg
title: Installing Thai fonts onto an Android device
---


I've received numerous requests asking for help on how to install Thai fonts onto an Android device after my initial post on [Rooting my Nexus One and installing Thai fonts](/2010/01/rooting-my-nexus-one-and-installing-thai-fonts).  Since I do update my Android phone with the [CyanogenMod ROM](https://www.cyanogenmod.com/) quite often (which wipes the Thai fonts on each install), I thought I'd share a simple shell script to help get Thai fonts onto Android.

This post **does not cover how to root an Android device**.  I will leave that to you to figure out.  But if you happen to have a Nexus One like me, check out the following link: [Video: How to unlock and root a Nexus One](https://androidandme.com/2010/01/hacks/video-how-to-unlock-and-root-a-nexus-one/).

Also, you will need to have the [Android SDK](https://developer.android.com/sdk/index.html) on your system (hopefully Mac or Linux-- which is what the script is written for, although for Windows it won't be hard to figure out what commands need to be run-- hint: use .\adb.exe instead of ./adb  in DOS or whatever command prompt and skip the shell script).

There are the *two prerequisites* to installing Thai fonts: **a rooted device** and **the Android SDK** on your system.  Oh, and I guess how to run some basic knowledge of the command line in a shell (Terminal).

#### Instructions

1. Attach your Android device to your computer via USB and mount it.</li>
2. Download: [InstallThaiFontsOntoAndroid.zip](https://www.mediafire.com/?464j2791iccuan9).
3. Unzip it and you will see a folder.

    ![Screnshot 1](/images/blog/Screen-shot-2010-08-30-at-4.40.01-AM.png)

    The contents of the folder should be placed in the <i>tools folder</i> of the Android SDK where adb is.

    ![Screenshot 2](/images/blog/Screen-shot-2010-08-30-at-4.19.06-AM.png)

    ![Screenshot 3](/images/blog/Screen-shot-2010-08-30-at-4.22.30-AM.png)

4. Open up a Terminal (Applications-&gt;Utilities-&gt;Terminal.app) and go into the directory where your android SDK and go into the folder: <i>tools</i>.

    ![Screenshot 4](/images/blog/Screen-shot-2010-08-30-at-4.30.23-AM.png)

5.  You can test to make sure that your device is connected by the following command in the terminal:

    ```
    ./adb devices
    ```

6. And to mount it:

    ```
    ./adb remount
    ```
7. Make sure that the script, install_thai_fonts.sh, is executeable by running:

    ```
    chmod +x install_thai_fonts.sh
    ```
8.  
    * **[Recommended]** Now you are ready to run the shell script to install the six fonts onto the device.

      ```
      ./install_thai_fonts.sh
      ```
    *Or, if you don't wish to run the shell script...*
    
    * **[Alternate]** Run the following line by line (you can copy &amp; paste them line by line into Terminal):

      ```
      ./adb push ./fonts/DroidSans.ttf /system/fonts/DroidSans.

      ./adb push ./fonts/DroidSans-Bold.ttf /system/fonts/DroidSans-Bold.ttf

      ./adb push ./fonts/DroidSerif-Bold.ttf /system/fonts/DroidSerif-Bold.ttf

      ./adb push ./fonts/DroidSerif-BoldItalic.ttf /system/fonts/DroidSerif-BoldItalic.ttf

      ./adb push ./fonts/DroidSerif-Italic.ttf /system/fonts/DroidSerif-Italic.ttf

      ./adb push ./fonts/DroidSerif-Regular.ttf /system/fonts/DroidSerif-Regular.ttf
      ```
     
    If there were no error messages, then you should now have the Thai fonts on the Android device.

9. **Reboot** and you will see Thai on webpages, SMS, and files names that are in Thai.


![Thai Fonts on Nexus One](/images/blog/IMG_2253.jpg)