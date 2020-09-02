---
author: "Steven Suwatanapongched"
blogger_id: tag:blogger.com,1999:blog-6841384.post-7235748124438055884
blogger_orig_url: https://www.sunpech.com/2012/06/putting-cyanogenmod-on-kindle-fire.html
date: '2012-06-28T11:00:00.000-05:00'
headerimage: /images/headers/android.jpg
modified_time: '2014-08-07T19:36:22.312-05:00'
redirect_from: /2012/06/putting-cyanogenmod-on-kindle-fire.html
tags:
  - Android
  - Technology
old_thumbnail: https://1.bp.blogspot.com/-yU7gPhRWdPg/T-wtYgHP_BI/AAAAAAABOks/dvPzH189ZBg/s800/Nexus7_tablets.jpg
thumbnail: /images/blog/tn_kindle-fire-cyanogenmod.jpg
title: Putting CyanogenMod on the Kindle Fire
---

After seeing the [Nexus 7 tablet](https://www.engadget.com/2012/06/27/nexus-7-tablet-hands-on/) make its debut at [Google I/O](https://developers.google.com/events/io/) yesterday, it made me realize how my Kindle Fire (KF) is kind of lame. I [reviewed the Kindle Fire](/2011/11/kindle-fire-review) back in November 2011.

![Nexus 7 tablets](/images/blog/Nexus7_tablets.jpg)

To be fair though, my needs have changed. When I initially purchased the KF, I didn't want an iPad2 or a 10" tablet. I just wanted a simple reading device that could browse the web a bit and play some games. And that's exactly what the KF was, and *still* is.

My needs have changed in that I want more. I want Gmail. I want YouTube. I want more apps.

The problem is that over the past eight months, I haven't seen any big improvements happen from Amazon. The [Amazon App Store](https://www.amazon.com/appstore) has fewer of the apps I like available compared to [Google Play](https://play.google.com/store). On top of that, the Google Apps such as Gmail and YouTube aren't available. To me, the biggest reason to use Android is Google's products and services: Gmail, Google Maps, YouTube, etc. These are all solid apps that should be on any Android device.

Besides the lack of Google Apps, there's no native Facebook app! The one in the Amazon App store simple redirects to a browser of the mobile site! This is incredibly misleading.

On top of all of this, there are other nuances with the KF: The UI sucks. The carousel and bookshelf is just stupid. I'm sure there are folks that like how this UI is rather simple. It's just not for me. I ended up installing Go Launcher EX alongside it. *(See [instructions](https://www.pcworld.com/article/252821/get_more_out_of_your_kindle_fire_tablet_five_tips.html) on how to install it.)* The volume UI also is not readily available-- requires an extra click to get there. The rotating wallpapers cannot be customized either.

Recalling all these frustrations, I got pretty close to [pre-ordering the Nexus 7](https://play.google.com/store/devices/details?id=nexus_7_8gb&amp;feature=single-wide-banner), which is priced exactly at $199, very competitively against the Kindle Fire.

But I didn't. Instead, I decided to just hack my Kindle Fire and see how close to a vanilla Android I could get.

Below are instructions I followed to get a custom ROM (Simple CyanogenMod 9) onto my Kindle Fire by rooting it. *Disclaimer: I am not responsible for anything that goes wrong with your device if you attempt anything I have written and linked to below.*

The instructions are pretty clear and I highly recommend reading and following them.

* Get Kindle Fire Utility (I used v0.9.6). See instructions [here](https://forum.xda-developers.com/showthread.php?t=1399889).
* Unzip the Kindle Fire Utility and install the drivers.
* Root the device.
* Install TWRP Recovery. For instructions, see: [How to Root and Install Custom Recovery on Kindle Fire using Kindle Fire Utility](https://www.androidauthority.com/how-to-root-and-install-custom-recovery-on-kindle-fire-using-the-kindle-fire-utility-53451/).
* Install [Simple CyanogenMod 9 ROM (6-10-2012)](https://forum.xda-developers.com/showthread.php?t=1689000). For instructions, see: [Amazon Kindle Fire: Flashing the Simple CM9 custom ROM](https://www.androidauthority.com/kindle-fire-install-simple-cyanogenmod-9-cm9-custom-rom-94468/).

*Note, for the developers out there that have the Android SDK installed, the KF Utility has adb packaged in it already.*

So, I was able to put Simple CM9 on my Kindle Fire using the instructions in the links listed above. Here's a picture my KF running Google Play that's downloading Google Chrome browser.

![Kindle Fire Install](/images/blog/KindleFire_install.jpg)

Here is a screenshot of my homescreen after some customizations.

![Kindle Fire Screenshot 1](/images/blog/KindleFIre_screenshot.jpg)

Another screenshot of the Settings and tablet information.

![Kindle Fire screenshot 2](/images/blog/KindleFire_screenshot_02.jpg)

Overall, it was a pretty simple process. Just follow the instructions. I was able to re-download my Kindle books again using Kindle app in the Google Play store. My Kindle Fire is just awesome now. Maybe I'm speaking too soon, as it hasn't even been a full twenty-four hours of running it just yet. I do notice that it sucks up the battery a lot more, but that should be obvious as I'm running a heavier UI and more apps.

These are exciting times aren't they? Microsoft has entered the tablet space (once again) with their [Surface](https://www.microsoft.com/surface/en/us/default.aspx). Or at least the announcement of it. There's a [rumor](https://www.theverge.com/2012/6/26/3119096/amazon-kindle-fire-successor-july-31-release-rumor) of a new Kindle Fire from Amazon next month. A lot of competition, which in the end the consumers win.

#### Update (January 8, 2013)

Just wanted to add that there is a way to root the Kindle Fire from a Mac. Just use [BreakDroid](https://northmendo.com/breakdroid/downloads/) The Kindle Fire Utility doesn't work on my Windows 8 Pro virtual machine like it did on Windows 7 Ultimate.

Also, I switched to use [Jandycane](https://forum.xda-developers.com/showthread.php?t=1766829) instead of CM. Still basically the same steps as above, but it gives me Jelly Bean on the tablet. I don't expect any more updates for custom ROMs on KF simply because Google Nexus tablets are superior in every way.

#### Update (August 7, 2013)

A few weeks ago I switched back to using [Cyanogenmod on the Kindle Fire](https://wiki.cyanogenmod.org/w/Otter_Info) (1st Generation). Overall it's been pretty good, but my KF is now my secondary tablet device since I got a [Nexus 7](https://www.google.com/nexus/7/) (2nd Gen).

![Cyanogenmod KF](/images/blog/cyanogenmod_KF.png)