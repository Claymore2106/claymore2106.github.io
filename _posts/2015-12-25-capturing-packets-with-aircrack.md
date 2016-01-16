---
layout: post
title: Capturing Packets with Aircrack-ng
---

## Setup

Before you can start using Aircrack, you need to set it up, and for that you
 need to choose which OS will be best for you. In the case of Windows, you'll
 need to assemble your own DLL's, which I wouldn't recommend if you don't know
 what you're doing. For Linux you need to learn how to use the OS, but Aircrack
 will most likely work out of the box. I recommend downloading [Virtualbox][VB]
 for your current OS, and [picking a Linux distro][distro] to install as the
 virtual machine. This way, you run a computer within a computer. Your current
 OS is your main, and your Linux machine is just a program.

 For this tutorial, I will be using **Linux Mint** without the VM.

You will also need a wifi card, integrated or external, and it needs to be
 compatible with Aircrack. Compatibility is determined by chipset, not
 manufacturer. The Aircrack website has a
 [page dedicated to helping you with this][drivers] and you should check it out.

 I will be using a **Panda Wireless PAU05** USB wifi dongle.

## Updates

First off, you should make sure your packages and distro are up to date. Ideally
 you should do this every time you're going to install something if some time
 has passed since you last updated. Its simple and only takes a minute. Update
 the apt repository by running `sudo apt-get update`

(Forgive the mice in the pictures, didn't realize Mint keeps it)
![Run apt-get update](/images/Capturing-Packets-Aircrack/1-apt-update.png)

Then, run `sudo apt-get upgrade`

![Run apt-get update](/images/Capturing-Packets-Aircrack/2-apt-upgrade.png)

Finally, run `sudo apt-get dist-upgrade`

![Run apt-get dist-upgrade](/images/Capturing-Packets-Aircrack/3-apt-dist-upgrade.png)

Now, your system should be up to date. These steps are necessary to make sure
 you have all necessary headers and files in case you need to compile from
 source code.

With that done, we can install the Aircrack suite and start capturing packets.

## Installation

Depending on your respsitories, you have Aircrack available for download. You
 can check by running 


<!--- References --->

[VB]: https://www.virtualbox.org/wiki/Downloads
[distro]: http://www.howtogeek.com/191207/10-of-the-most-popular-linux-distributions-compared/
[drivers]: [http://www.aircrack-ng.org/doku.php?id=compatibility_drivers]
