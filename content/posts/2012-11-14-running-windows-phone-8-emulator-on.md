---
author: "Steven Suwatanapongched"
blogger_id: tag:blogger.com,1999:blog-6841384.post-7557647617734760650
blogger_orig_url: https://www.sunpech.com/2012/11/running-windows-phone-8-emulator-on.html
date: '2012-11-14T11:00:00.000-06:00'
headerimage: /images/headers/software_development.jpg
modified_time: '2014-08-08T16:44:52.111-05:00'
redirect_from: /2012/11/running-windows-phone-8-emulator-on.html
tags:
  - Guide
  - Software Development
old_thumbnail: https://1.bp.blogspot.com/-zmyacljuX2g/UKN_RJcTrtI/AAAAAAABVvU/68s9SzlJNw0/s800/VMF5_WinPhone8.jpg
thumbnail: /images/blog/tn_windows-8-emulator-vmware.jpg
title: Setting up Windows Phone 8 Emulator on a Virtual Machine
---

Not long ago I blogged about [Installing Windows 8 Pro on Parallels Desktop 8](/2012/11/installing-windows-8-pro-on-parallels-desktop-8/). That of course worked for me, but when it came time to having Visual Studio 2012 (VS2012) and running an emulator for Windows Phone 8, it simply doesn't work. I searched the Internet as to why, and came up with the following links:

* [StackOverflow: Unable to create the virtual machine](https://stackoverflow.com/questions/13148828/unable-to-create-the-virtual-machine)
* [MSDN: Having problems running the Windows Phone 8 Emulator?](https://social.msdn.microsoft.com/Forums/en-US/wpdevelop/thread/860f4203-e3f7-410e-8bf5-2999224df312)
* [Running the Windows Phone 8 emulator in a virtual machine](https://blog.catenalogic.com/post/2012/10/31/Running-the-Windows-Phone-8-emulator-in-a-virtual-machine.aspx) (I followed this guide)


As a lot of people [pointed out](https://forum.parallels.com/showthread.php?p=646448#post646448), it's not really possible in [Parallels Desktop 8](https://www.parallels.com/products/desktop/) (PD8), but is possible through [VMware Fusion 5](https://www.vmware.com/products/fusion/overview.html) (VMF5) with a small workaround.

![Setting Up Windows Phone Emulator 1](/images/blog/VMF5_WinPhone8.jpg)

I recommend following [this guide](https://blog.catenalogic.com/post/2012/10/31/Running-the-Windows-Phone-8-emulator-in-a-virtual-machine.aspx), but will supplement some more information as it pertains to VMF5, as it's not exactly the same as [VMware Workstation 9](https://www.vmware.com/products/workstation/overview.html).

First off, I recommend installing from scratch. I tried to import my existing virtual machine created through PD8, and failed many, many, many times. I ended up with a blue screen screen and countless reboots that try to fix something that didn't get fixed. Save yourself time and just do a clean install of Windows 8 on VMF5.

Even if you have or haven't installed VS2012 with [Windows Phone 8 SDK](https://dev.windowsphone.com/en-us/downloadsdk), you should uninstall Hyper-V.

You can get to this in Windows 8 through Control Panel and search for "windows features". Then click on "Turn Windows features on or off".

![Setting Up Windows Phone Emulator 2](/images/blog/WindowsFeaturesOnOff.jpg)

Make sure these boxes are unchecked, as in off. *You'll check these back on later.*

![Setting Up Windows Phone Emulator 3](/images/blog/WindowsFeatureHyperV.jpg)

Next in the virtual machine's settings, in Processors &amp; Memory, uncheck "Enable hypervisor applications in this virtual machine". *You'll check this back on later.*

![Setting Up Windows Phone Emulator 4](/images/blog/VMF5_Settings_ProcMemory.jpg)

![Setting Up Windows Phone Emulator 1](/images/blog/Enable_HypervisorApps.jpeg" />

Next you have the Virtual Machine Library window open, and then right click + hold alt (option) key to get the option to "Open Config File in Editor".

![Setting Up Windows Phone Emulator 5](/images/blog/VirtualMachineLibrary_screenshot.jpg)

Here add the following settings, as they shouldn't exist.

```
hypervisor.cpuid.v0 = "FALSE"
mce.enable = "TRUE"
```

![Setting Up Windows Phone Emulator 6](/images/blog/EditVMXFile.jpg)

Finally, check back on everything you unchecked from before. A restart is probably needed for the Windows Hyper-V install again.

Now you'll be able to run a Windows Phone Emulator within VMware Fusion 5, on a Mac!

![Setting Up Windows Phone Emulator 7](/images/blog/WindowsPhoneEmulator.jpg)

Happy coding!

*Note: I haven't purchased my copy of VMware Fusion 5 yet. I'll likely buy it before the 30-day trial is up.*