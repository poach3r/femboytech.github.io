---
layout: post
title:  "Cool Programs 1: Pywal"
date:   2023-03-04 00:00:00 -0500
author: poacher
---

# Introduction

[Pywal](https://github.com/dylanaraps/pywal) is a piece of software which allows for the ultimate ricing experience, allowing you to easily theme a majority of the programs you use based on your wallpaper with a few CLI commands.

# Installation

### Universally

`pip3 install pywal`

### Arch

`pacman -S python-pywal`

### Void

`xbps-install pywal`

# Usage

`wal -i "/path/to/img.jpg"` will set the desired image for theming.

## Applying Themes to Terminal

Add the following lines to your ~/.bashrc/

`(cat ~/.cache/wal/sequences &)`

`source ~/.cache/wal/colors-tty.sh`

## Reapply Theme on Reboot

Add the following to your .xinitrc OR your window managers config file (ie ~/.config/i3/config)

`wal -R`
