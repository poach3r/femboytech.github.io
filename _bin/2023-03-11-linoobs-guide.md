---
layout: page
title: "Linoobs Guide"
date: 2023-03-17 00:00:00 -0500
author: poacher
---

A WIP guide to Linux for extremely new users.

# Disclaimer:

I am only human, I cannot cover everything, if there is anything you would like added to this article my <a href="/contact">Discord DMs are open<a> 

# 1. Distribution

I recommend Fedora or KDE Neon, you can't go wrong with either of them.

[Fedora](https://www.fedoraproject.org/)
[KDE Neon](https://neon.kde.org/)

# 2. Desktop Environments

Desktop Environments and distribution are frequently conflated by new users. Your Desktop Environment is what is displayed, think your taskbar and desktop icons. Your distribution is the .iso you installed, it is a version of Linux that comes with certain programs preinstalled. Your Desktop Environment is **COMPLETELY SEPARATE** from your distribution, distributions may come with a Desktop Environment however you can install any Desktop Environment on any distribution.

# 3. The Terminal

Now the terminal may seem rather scary at first, however it really isn't, it's an extremely useful tool that you should familiarize yourself with.

## <a href="https://man7.org/linux/man-pages/man8/sudo.8.html">sudo<a>

Sudo is a command which allows you to run any command as **root**, this is the equivalent to running a program as **administrator** on Windows. Simply type it before whatever command you would like to run as **root** and then type in your password.

## apt

APT stands for Advanced Packaging Tool, it is the command line utility to install, remove, and update packages (programs) on Debian based distributions such as KDE Neon, Ubuntu, and Mint.

### Installing Packages

`sudo apt install package_name` 

allows you to install any package within the Debian repositories.

### Removing Packages

`sudo apt remove package_name` 

allows you to remove any package that was installed on your system via apt.

### Search for Packages

`apt search package_name`

allows you to serach for packages in the Debian repositories

### Upgrade Packages

`sudo apt full-upgrade` 

will upgrade your entire system, please use **EXTREME CAUTION** with this command as it can cause **PERMANENT DAMAGE** to your system.

## <a href="https://man7.org/linux/man-pages/man1/man.1.html">man<a>

Man is a utility which is usually installed by default on most distributions, it will display a verbose manual for whatever command you would like.

`man command_name`

## <a href="https://man7.org/linux/man-pages/man1/echo.1.html">echo<a>

Echo is a utility that displays whatever text you would like to the terminal.

`echo "Hello, World!"`

outputs

`Hello, World`

## <a href="https://man7.org/linux/man-pages/man1/touch.1.html">touch<a>

Touch is a utility which allows you to easily create files.

`touch ~/dir1/helloworld.txt`

creates the file helloworld.txt

## <a href="https://man7.org/linux/man-pages/man1/cat.1.html">cat<a>

Cat is a utility that will display the content of any text file on your system.

`cat ~/dir1/helloworld.txt`

outputs

`Hello, World!`
`How are you?`

## <a href="https://man7.org/linux/man-pages/man1/grep.1.html">grep<a>

Grep is a utility that will search any terminal output for a specific phrase. It is commonly used by "piping" another command into it.

`cat ~/dir1/helloworld.txt | grep "How"`
                         ^ This is a pipe!
outputs

`How are you?`

## <a href="https://man7.org/linux/man-pages/man1/ls.1.html">ls<a>

Ls is a utility which lists the contents of a directory.

`ls ~/dir1`

outputs

`file.txt helloworld.txt`

## <a href="https://man7.org/linux/man-pages/man1/mv.1.html">mv<a>

Mv is a utility which lets you move files.

`mv ~/dir1/file.txt ~/dir2/file.txt`

will move file.txt from ~/dir1 to ~/dir2

## <a href="https://man7.org/linux/man-pages/man1/cp.1.html">cp<a>

Cp is a poorly named utility which allows you to copy files.

`cp ~/dir2/file.txt ~/dir1/file.txt`

will create a copy of file.txt inside of dir1

# 4. The Myth of Bloat

"Bloat" is a term that is frequently thrown around in more "hardcore" parts of the Linux community, however it is a problem that is drastically overblown and is something you shouldn't be concerned about. Bloat is any program that is too large, uses too many resources (commonly RAM), and/or has too many packages. Programs which do these things aren't inherently bad, the number of packages which a program uses doesn't matter, a bit of extra storage space doesn't matter, some more idle RAM use doesn't matter. The only thing that does matter is whether the program functions well or not.

# 5. Anti-Viruses

One of the most common mistakes by new Linux users is believing they need an anti-virus, however this is simply false. Linux is far more secure than both Windows and MacOS for a variety of reasons.

## a. Small Userbase

If you're attempting to make some money or just cause chaos then you would want to target the biggest operating system, since Linux has only 1% market share it makes no sense to target Linux when targeting Windows wouldbe far more effective.

## b. Open Source

To someone not in the know, being open source may seem like a vulnerability rather than an added layer of protection, however this is just false. The open source nature of it means that people are constantly scouring the code for bugs and vulnerabilities to fix, this means that a hacker would have to be faster and smarter than the thousands of people contributing to Linux every day.

## c. Package Repositories

The majority of your software will either be installed through the official package repositories for your distribution, or GitHub. This prevents interference from 3rd parties who may try and give you malware (ie fake websites and download buttons). However, this does not make you immune to malware, malware can still be hidden in these things, and while extremely rare, it has happened before.

# 6. Drivers

Drivers are another thing that frequently confuse new users, for almost all hardware you own, you will not need to install drivers, either they're already built into the Kernel or they don't exist. For example, AMD has their GPU and CPU drivers built into the Kernel, you don't need to install anything else, they simply work out of the box.

## NVidia

<iframe width="640" height="360" src="https://www.youtube.com/embed/Q4SWxWIOVBM" frameborder="0" allow="accelerometer; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

NVidia drivers are a fickle thing, I can't make a guide (yet) but chances are your distribution tells you how to install them.

# 7. Fingerprint Readers

The majority of laptop fingerprint readers simply don't work, this is a harsh reality with Linux. Utilities like fprintd can add compatbility for some fingerprint readers, however not for a lot of them.

# 8. Program Emulation

Sometimes if you desperately need a Windows program you can emulate it through Wine or any Wine wrapper (ie Bottles or GNOME Boxes). Wine is an extremely flawed program and I would recommend avoiding it as much as possible, its prone to bugs, poor performance, and sometimes just not working. Instead, I highly recommend using alternatives to the programs that you would use on Windows.

# 9. Program Compatibility

Not all programs are compatible with Linux and this is fine! There are plenty of alternatives to these programs that are usually free and open source.

For easily finding alternatives I would recommend taking a look at <a href="https://alternativeto.net/">Alternative To.<a>

## Microsoft Office Suite

The Microsoft Office Suite is very easily replaced by Libre-Office, it is one of the most developed free and open source programs of all time and features everything in the Microsoft Office Suite.

<a href="https://www.libreoffice.org/">Libre-Office<a>

## Photoshop

Photoshop is not as easily replaced, alternatives like Gimp and Krita exist however they are not as feature rich. Gimp lacks things like Non Destructive Editing and Krita is mostly for drawing.

<a href="https://www.gimp.org/">Gimp<a>

<a href="https://krita.org/">Krita<a>

## Snip/ShareX

Snip and ShareX are both replaceable via either Flameshot or GNOME's screenshot tool, they function almost identically however they lack the ability to auto upload to a website like ShareX can.

<a href="https://flameshot.org/">Flameshot<a>

## Adobe Premiere 

Kdenlive is a fully featured editor which is on par with Adobe Premiere, it can be a bit slower in some areas and it does have some issues with certain hardware, however these problems are rather minor.

<a href="https://flameshot.org/">Kdenlive<a>

## Discord

While Discord *can* work perfectly fine on Linux it does not always work fine, this is why I recommend either Webcord or GTKCord4. Webcord is a fully featured Discord client which functions identically to the original, GTKCord4 is a beta program which rewrites the Discord client using the GTK toolkit.

<a href="https://github.com/SpacingBat3/WebCord">Webcord<a>

<a href="https://github.com/diamondburned/gtkcord4">GTKCord4<a>

## Outlook

There are many E-Mail clients for Linux however none of them are particularly great, however, Thunderbird has been undergoing many rewrites and will be massively improved in due time.

<a href="https://www.thunderbird.net/en-US/">Thunderbird<a>

## 7Zip/WinRAR

WinRAR isn't on Linux (duh) and while 7Zip is on Linux it's a pretty bad experience. Some file explorers will come with the ability to view RAR files by default and some don't, if yours doesn't then I recommend using Xarchiver and optionally a plugin which better integrates it with your file explorer.

<a href="https://xarchiver.sourceforge.net/">Xarchiver<a>

<a href="https://docs.xfce.org/xfce/thunar/archive">Thunar Xarchiver Plugin<a>

## Game Launchers

The only official game launcher that is compatible with Linux is Steam, Steam on Linux is an incredible experience due to things like Proton, however if you want to play games from other launchers on Linux there is an answer. Lutris is a program which lets you connect to your launchers account and then download your games and play them through Wine/Proton, while not a seamless experience it works extremely well.

<a href="https://lutris.net/">Lutris<a>

## Multimedia Viewers

VLC, just use VLC.

I'm kidding, while VLC is easily the best one there are other programs such as mpv and Celluloid (a front end for mpv).

<a href="https://www.videolan.org/vlc/">VLC<a>

<a href="https://mpv.io/">mpv<a>

<a href="https://celluloid-player.github.io/">Celluloid<a>

# 10. Essential Programs

These are programs that are very frequently used by you or required by other programs.

## <a href="https://git-scm.com/">git<a>

Git is a utility which allows you to easily download repositories from and commit to GitHub/GitLab. Also it was made by Linus Torvalds so you're obligated to use it.

## <a href="https://ffmpeg.org/">FFmpeg<a>

FFmpeg is a utility that allows you to easily modify videos through the commmand line, a commonly needed dependency.

## <a href="https://imagemagick.org/">ImageMagick<a>

FFmpeg but for images, also a commonly needed dependency.

## <a href="https://github.com/aristocratos/btop">BTOP<a>

BTOP is a massively improved version of HTOP, a TUI-based system monitoring utility.

## <a href="https://www.youtube.com/watch?v=773PhMgEOFw">QEMU/VirtManager<a>

VirtManager is a front end for QEMU, a utility that lets you easily create extremely efficient KVMs (Kernel Virtual Machines), I've linked a video by Mental Outlaw explaining how to use and install it.

## <a href="https://www.vim.org/">Vim<a>

Vim is a TUI program that allows you to easily and quickly edit text, however, it has a rather steep learning curve so be wary of that.

## <a href="https://cmake.org/">CMake<a>

CMake is a utility that allows for the compilation of various programs, it is frequently needed when you want to install a program not found in your repositories.

## <a href="https://gparted.org/">GParted<a>

GParted is program which allows you to easily partition disks.

## <a href="https://gparted.org/">Timeshift<a>

Timeshift is a program which allows you to easily backup and restore your Linux install, a necessity if you plan on doing some tinkering with your system.

## <a href="https://torproject.org/">Tor<a>

While Tor may have a poor reputation, it's an extremely useful program for securely and privately browsing the web.
