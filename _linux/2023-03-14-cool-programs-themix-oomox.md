---
layout: post
title:  "Cool Programs 3: Themix/Oomox"
date:   2023-03-14 00:00:00 -0500
author: poacher
---

# Introduction

[Themix/Oomox](https://github.com/themix-project/themix-gui) is a theming application which allows you to easily create new GTK2/3, Cinnamon, Openbox, and Spotify themes.

# Installation

### Universally

```
git clone https://github.com/themix-project/oomox.git --recursive
cd oomox
make -f po.mk install
./gui.sh
```

### Arch

```
pacman -S themix-full-git
```

# Usage

```
themix-gui
``` 

will launch the GUI. Inside the GUI you can modify various presets and then export them by clicking the `Export Theme` button in the top right. You can also create Icons and then export them by clicking on the `Export Icons` button in the top right, next to the `Export Theme` button.

![themix](/assets/themix.png)