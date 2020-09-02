---
author: "Steven Suwatanapongched"
blogger_id: tag:blogger.com,1999:blog-6841384.post-7628154985244238079
blogger_orig_url: https://www.sunpech.com/2008/12/setting-up-wrt54g-as-wireless-bridge.html
date: '2008-12-24T23:39:00.000-06:00'
headerimage: /images/headers/technology.jpg
modified_time: '2014-08-08T17:01:27.441-05:00'
redirect_from: /2008/12/setting-up-wrt54g-as-wireless-bridge.html
tags:
  - Guide
  - Technology
old_thumbnail: https://4.bp.blogspot.com/_7U5MdumP-no/SVMeq-RLbEI/AAAAAAAAIZk/b33sMkW_w9o/s800/linksys_wrt54g.jpg
thumbnail: /images/blog/tn_linksys_wr54g.jpg
title: Setting up WRT54G as a wireless bridge with DD-WRT
---


My parents have a [Thai TV](https://www.thaitv.tv/) ethernet box of some kind so they can tune in to their Thai stations, shows, and even radio on their HDTV.  However, I had to run a 50 foot CAT5 cable from the upstairs to the first floor great room, which is quite messy.  So for Christmas this year, I bought them a [Linksys-Cisco WRT54GL Wireless-G Broadband Router](https://www.amazon.com/gp/product/B000BTL0OA?ie=UTF8&amp;tag=sunpech-20&amp;linkCode=as2&amp;camp=1789&amp;creative=9325&amp;creativeASIN=B000BTL0OA).

![Linksys WRT54G](/images/blog/linksys_wrt54g.jpg)

The setup I wanted was to have the Thai TV box, which uses an ethernet port for all data, connect to the wireless router, and have the wireless router connect to the wireless router upstairs.  This setup required a wireless bridge, which the router did not come configured with.  So after some googling, I found the proper links to set it all up with:

![WiFi Bridge](/images/blog/WIFIBRDG.jpg)

First thing to do, is to figure out what to do with your particular router: [Linksys WRT54G/GL/GS/GX](https://www.dd-wrt.com/wiki/index.php/Linksys_WRT54G/GL/GS/GX).  For me, I had to [Flash the WRT54Gv8](https://www.dd-wrt.com/wiki/index.php/How_To_Flash_the_WRT54Gv8).

Unfortunately for me, I messed up the installation, and "bricked" my router.  But after more googling, I found out how to "unbrick" it: [UnBrick your Linksys router - WRT54GS v7](https://blog.rim3y.net/zero/?p=942).  Apparently my problem was that the tftp program was just incredibly slow in uploading the firmware, and I closed the DOS window too quickly due to what appeared to be inactivity.

The last thing I had to do was set up the [wireless bridge](https://www.dd-wrt.com/wiki/index.php/Wireless_Bridge), which was the easy part.  So there you have it, how to set up a wireless bridge using DD-WRT.