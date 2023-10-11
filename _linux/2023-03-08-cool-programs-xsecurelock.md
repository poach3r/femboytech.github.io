---
layout: post
title:  "Cool Programs 2: XSecureLock"
date:   2023-03-07 00:00:00 -0500
author: poacher
---

# Introduction

[XSecureLock](https://github.com/google/xsecurelock) is a screen locking utility for X11 created by Google, yes, Google. It allows for large amounts of customization and top notch security.

# Installation:

### Universally:

```
git clone https://github.com/google/xsecurelock.git
cd xsecurelock
sh autogen.sh
./configure --with-pam-service-name=SERVICE-NAME
make
sudo make install
```

### Arch:

```
pacman -S xsecurelock
```

### Void:

```
xbps-install xsecurelock
```

# Usage:

```
xsecurelock
``` 

will initialize the default lock screen.

```
env XSECURELOCK_SAVER=saver_xscreensaver xsecurelock
``` 

will initialize the lockscreen with xscreensaver.

# Automatic Locking:

Automatic locking (or at least the method I will cover) requires <a href="https://man.archlinux.org/man/xss-lock.1">xss-lock<a>

## Installation:

### Arch:

```
pacman -S xss-lock
```

### Void:

```
xbps-install xss-lock
```

## Usage:

Adding

```
xset s 300 5
```

and

```
xss-lock -n /usr/lib/xsecurelock/dimmer -l -- xsecurelock
```

to the config file of your window manager or your .xinitrc will start allow XSecureLock to start after 300s of inactivity or whenever your system is told to suspend (ie closing a laptop lid).
