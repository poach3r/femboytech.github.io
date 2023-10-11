---
layout: post
title: "The Art of Ricing"
date: 2023-03-17 00:00:00 -0500
author: poacher
---

# Introduction:

This will be a rather comprehensive guide for creating a rice from scratch, I will be ricing my desktop alongside you in this guide, my choices for programs will be mentioned when relevant.

# 1. Choose a General Theme

This doesn't need to be anything specific, just think of a general concept or feeling that you want to base this around. Do you want it to feel warm? Do you want it to feel cosy? Do you want it to be minimal? Do you want lots of pink? etc...

There are a few color palette sites you can look at, I prefer https://colorhunt.co/

For my rice I would like to do a very colorful, very satured rice.

# 2. Choose a Wallpaper

The wallpaper is an extremely important aspect of the rice as it will likely define both the colorscheme and the feeling of the rice. For finding wallpapers I like to browse /wg/ because I'm a freak, however I recommend you browse something like Wallhaven or even just social media such as Twitter.

I chose a piece of art called "What Space Really Looks Like" by Nina Geometrieva

https://www.behance.net/gallery/12984019/What-Space-Really-Looks-Like

![wallpaper](https://i.postimg.cc/bvrCpcQd/wallpaper.jpg)

# 3. Choosing a Window Manager

This is arguably the most important part of the rice as it will determine how you do everything and what programs you use.

I have decided to use Hyprland, however, I also <a href="https://github.com/poach3r/yellow-dots">recently riced berrywm.<a>

## Xorg Window Managerss

**i3**: A barebones and easy to use window manager.

**bspwm**:  A slightly harder but more feature rich window manager.

**herbsluftwm**: An odd one, its a bit of a hackers window manager however it's extremely lightweight and customizable.

**XMonad**: An extremely efficient window manager, however it's hard to configure due to being written in Haskell.

**berrywm**: A very underrated floating window manager which is extremely lightweight and easy to configure.

## Wayland Window Managers

Note: I know they're compositors not window managers, I'm calling them window managers to make things less confusing.

**Hyprland**: A beautiful and extremely customizable window manager with incredible animatioms,.

**Sway**: i3 but for Wayland.

**riverwm**: An efficient window manager written in Zig.

# 4. Try out the Window Manager

After installing the window manager you think you want to use, go into the config and edit a few things such as keybindings and the terminal emulator used. The majority of window managers will generate a config file at ~/.config/(WINDOW MANAGER NAME)/ on first boot, so simply boot into them, logout/restart, modify the config, then try it out.

I modified the Hyprland config at ``~/.config/hypr/hyprland.conf`` and changed a few keybindings and then changed the default terminal emulator from Kitty to Foot (more on this later).

# 5. Choosing Programs

When ricing you will likely need to pick and choose what programs you want to use to serve certain functions, this section will cover these.

## 5a. Bars

The bar is another extremely important part of your rice as it will be on screen almost all the time, it displays extremely important information such as the time, your workspaces, battery life, and various other settings.

I used waybar for this rice however I have used polybar and yabar in the past.

**waybar**: A fantastsic and easily customizable bar for Wayland.

**polybar**: A very powerful though hard to configure bar for Xorg.

**Eww**: A cross compatible bar written in Rust which allows for far more complex actions than any other bar.

**yabar**: An underrated lightweight and easy to configure bar for Xorg.

**lemonbar**: An extremely lightweight bar which is truly for hackers, it can only be used by piping standard input into it.

## 5b. Notification Daemons

Your notification daemon provides notifications, pretty self explanatory.

I chose mako for this however I have used dunst in the past.

**mako**: A lightweight notification daemon for Wayland

**dunst**: A cross compatible notification daemon.

**xfce4-notifyd**: A standalone notification daemon recommended for use with XFCE desktops.

**fnott**: A keyboard driven notification daemon for Wayland.

## 5c. App Launchers

App launchers are also self explanatory, they allow you to easily launch programs with the press of a button (or 2!).

I have used Rofi in every single one of my rices, I recommend everyone use it.

**Rofi**: A cross compatible and extremely customizable program which allows you to do far more than just app launchers.

**dmenu**: A lightweight Xorg program mainly for launching apps, however, it can be made to do other things.

**Wofi**: A rewrite of Rofi built for Wayland.

**ULauncher**: A program launcher that can be easily configured through the use of community plugins and themes.

**DLauncher**: ULauncher but in Rust.

**Fuzzel**: A powerful but lightweight replacement for both Rofi and dmenu made for Wayland.

## 5d. Terminal Emulators

While most terminal emulators are the same there are some minor differences that make some better than others.

On Wayland I will always use foot, however I like to use Kitty on Xorg.

**Kitty**: Kitty is an easy to configure GPU-Accelerated terminal emulator.

**foot**: An extremely lightweight terminal emulator for Wayland.

**st**: An extremely lightweight but hard to configure terminal emulator.

**Alacritty**: Very similar to Kitty however it is harder to use but less bloated,

## 5e. File Managers

File manager choice is very limited, the majority of the ones on this list will be from big desktop environments however they can be used standalone.

I always use Thunar.

**Nautilus**: The GNOME file manager.

**Dolphin**: The KDE file manager.

**Thunar**: The XFCE file manager.

**Nemo**: The Cinnamon file manager.

**Ranger**: A TUI file manager.

## 5f. Shells

There are only 3 major shells on Linux, these shells are what allow you to use the terminal.

I have always used Fish, however zsh is better if you want a more customized experience.

**bash**: The default shell, basic, boring, just alright.

**Fish**: An easy to use but feature rich and customizable shell.

**zsh**: A "do it yourself" type shell, the majority of features are disabled out of the box and you have to enable and config them yourself.

# 6. Colors

For colors you have 2 options, either automatically generate colors and themes for programs from your wallpaper using Pywal or manually pick them and manually create themes for apps, I much prefer using Pywal.

# 7. Configuring the Window Manager

As stated earlier, almost all window manager config files are located at ~/.config/(WINDOW MANAGER NAME), I highly recommend keeping the documentation out at all times while configuring.

## IMPORTANT:

Depending on your window manager, the majority of the effects mentioned may require a compositor such as picom/compton.

## 7a. Gaps

I prefer to keep my gaps somewhere between 5-10px, this keeps things separated while not taking up too much space.

I have chosen to use gaps of 5px

## 7b. Borders

Borders are a good alternative to gaps, they also keep things separated but use less space.

I have chosen to not use borders however you can use them on top of gaps just fine.

## 7c. Rounding

Rounding does not always look good, it can very easily mess up a setup if used too aggressively.

I have chosen to use rounding of 8px

## 7d. Opacity

Opacity can look great however it can also get in the way, don't go overboard with it.

I have chosen to use 0.8 opacity on active windows and 0.7 opacity on inactive windows.

## 7e. Blur

Blurring the background almost always looks great, it also helps improve clarity.

I have chosen to use blur.

## 7f. Drop Shadow

Most window managers do not support drop shadow, even when using something such as picom, however if yours does and you area already using transparent windows then I highly recomend using it.

I will be using drop shadows.

# 8. Bar Configuration

I cannot cover bar configuration in depth due to the massive differences between bars, however I will try my best to cover the basics.

## 8a. Workspaces

I prefer to keep my workspaces either on the left of the bar or in the middle, this allows for them to not interfere with the other aspects of the bar.

## 8b. Clock

I keep my clock at the rightmost edge of the bar and use the 12 hour format.

## 8c. System Info

I prefer displaying only my CPU usage, RAM usage, and battery level, I keep these to the right of the bar next to the clock.

## 8d. Program Names

Some bars will allow you to display the name of the program currently being used, I like putting this on the left or middle of the bar depending on where my workspaces are.

# 9. App Launcher Configuration

Honestly just download someone elses script from GitHub and then modify the colors.

# 10. Notification Daemon Configuration

Notification daemons are generally easy to configure and usually use a similar format.

I have given mine no border and 8px rounded edges.

# The End Product

Hopefully by the end of this your rice should look fantastic, and while not everything will be riced this is a great place to start off.

This was the end product of my rice for this guide.

https://github.com/poach3r/hypr-dots

![rice](https://i.postimg.cc/xCb6Nvp2/rice.png)

![rofi](https://i.postimg.cc/9fkxf8pb/rice-rofi.png)