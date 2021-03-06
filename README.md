<p align="center">
<a name="top" href="https://github.com/addy-dclxvi/almighty-dotfiles/"><img src="https://raw.githubusercontent.com/addy-dclxvi/almighty-dotfiles/master/header.png"></a>
</p>

## Introduction
A collection of configs to be placed in the users home directory usually prefixed with a period, hence the name dotfiles.
This repo is actually intended for my personal backup, but everyone are welcome to use these resources. <br />
Designed for **Arch Linux**, but can also works for another distro.

## Preview
**A Change of Seasons** <br />
![alt text](https://raw.githubusercontent.com/addy-dclxvi/almighty-dotfiles/master/preview.jpg) <br />
**Openbox Theme** : Clair (included in this repo)

## Containing
- **Openbox** <br /> Some useful keybinds like snap window with useless gaps (super + arrows). MPC control using *play/pause, next, previous,* and *stop* keys. *Super + number* to switch workspace like in i3wm.
*Super + shift + number* to send window to another workspace (also like in i3wm), and more keybinds. Please read the *rc.xml* first before using it, just in case I forgot to remove my **self-destruct** keybind before I pushed it to this repo. <br /> <br />
And a well commented *autostart* file is included. Also including two bonus Openbox Theme only for You, Triste & Clair. Want more themes? please check my [Openbox Theme Collections](https://github.com/addy-dclxvi/Openbox-Theme-Collections).

- **obmenu-generator** <br /> My Openbox menu in the screenshot above is generated using obmenu-generator pipemenu. To use my scheme simply copy my scheme & config, then install *obmenu-generator* from AUR and type ```obmenu-generator -p``` and reconfigure Openbox.

- **i3-gaps** <br /> Pretty stock simple config with useless gaps. My config is using Polybar as statusbar.

- **Polybar** <br /> Just a very basic config from Jaagr's Polybar example.
  
- **zshrc** <br /> Containing some useful alias, and simple [Oh-My-Zsh](https://aur.archlinux.org/packages/oh-my-zsh-git) config. Including my minimalist oh-my-zsh themes (in ~/.oh-my-zsh folder).
To use it, simply install oh-my-zsh package, copy my .zshrc & .oh-my-zsh folder to your home. Then switch shell using ```chsh``` command.
  
- **Compton** <br /> Eye candy shadow. Also some useful "exclude" to avoid broken compositing.

- **Conky** <br /> Just a single conkyrc. For my another Conky collections please check my other [repos](https://github.com/addy-dclxvi?tab=repositories).

- **Tint2** <br /> Just a single tint2rc. For my another Tint2 collections please check my [Tint2 Themes Collections](https://github.com/addy-dclxvi/Tint2-Theme-Collections).

- **termite** <br /> My custom color schemes for termite. To use white color schemes just launch ```termite-light``` command from *dmenu* (if you are using use my *~/.bin* & *.profile*). And Use *M+ 1mn* fonts.

- **Xresources** <br /> My custom color schemes & config for Urxvt, including copy paste support by [Muennich](https://github.com/muennich/urxvt-perls). Hit Alt+C to copy, and Alt+V to paste (*xsel* package is needed). Use *M+ 1mn* fonts.<br />
Also contains my stupidly minimalist *rofi* theme.

- **ncmpcpp** <br /> A simple ncmpcpp config, with album art support. The album art script is taken from [Marco](https://marcocheung.wordpress.com/). Slightly modified to get rid the transparency bug. <br /> <br />
![alt text](https://raw.githubusercontent.com/addy-dclxvi/almighty-dotfiles/master/preview2.png) <br />
**Now Playing** : Dream Theater - Strange Deja Vu (Metropolis Part 2 : Scenes from a Memory, 1999) <br /> <br />
To use ncmpcpp with album art, simply launch ```my-music``` from dmenu (if you are using my *~/.bin* & *.profile*). Urxvt with pixbuf enabled is needed. You can get it from AUR, the package name is *rxvt-unicode-pixbuf*. And Use *M+ 1mn* fonts, because of what? It just looks nice. <br />
Also integrated with *dunst* notification. Just copy my dunst config, install dunst, and do nothing. Dunst will launch automatically if triggered by *notify-send* event.

- **gtk.css** <br /> Add useless space wasting paddings (who don't love terminal paddings? it looks nice) for vte-based terminal, including termite.

- **bin** <br /> The most useful script here is gitsetup & gitpush by [Erik Dubois](http://erikdubois.be/quick-easy-way-set-personal-github-repository), and some script for Tint2 executor.
The rest are only toys from [Crunchbang Forum](https://crunchbang.org/forums/viewtopic.php?id=13645). Don't forget to make them executable. Also copy *.profile* file to your home to make them executable without writing full path.

## Additional Information
Some of these configs are hardcoded, that mean You need to edit the configs before it would work. Like the path and default apps.
- My username at my machine is *addy@freako*, so some of these configs path are pointing to ```/home/addy``` 

- My wlan adapter is *wlp2s0*, and my ethernet adapter is *enp1s0*. If you find these in the configs, replace them with your own. Use ```iwconfig``` to find yours. 

- My fonts are M+ 1mn (for terminal) and Roboto & Noto Sans (for GTK, openbox, panel, and other things that don't need a fixed space font). For iconic fonts, depends on what You see inside the config file. 

- My Web Browser is Chromium.

- My terminal is termite, and Urxvt as spare.

- My program launcher is dmenu & rofi.

- My text editor is Geany.

- My wallpaper handler is Feh.

- My screenshooter is Scrot. You will see that my keybind for printscreen is executing scrot.

- My music player is ncmpcpp & Audacious (only for double click mp3 file, I mainly using ncmpcpp), my media player is VLC.

- My image viewers are Viewnior.

- My Window Managers are Openbox, i3-gaps.

- My panels are tint2 (with executor support) and polybar (with libmpdclient support). I gave up with lemonbar & dzen2 after slamming my head into wall twice!

## Package List
I can't remember one by one what packages need to be installed to make everything works.
But I have generated a [pkglist.txt](https://github.com/addy-dclxvi/almighty-dotfiles/blob/master/pkglist.txt) file. It contains a list of my installed packages, maybe it will help You to decide what packages need to be installed.
It is pretty barebones & not so bloated, only containing 772 packages. <br />
Or if You want to brutally replicate my setup, just install them all using ```yaourt -S pkglist.txt --needed```  <br />
It will install every packages that I have but You don't have. But I'm too afraid to test it by myself. Maybe You want to be a volunteer to test the command above, and post the results here. If your OS is broken, I will not use that command.

## Comments
I have spend so much time writing comments in my config files for a purpose, to be read.

## Apologies
I'm sorry for this damned *readme* file. I'm trying to provide the best. And about **self-destruct** keybind, I was kidding. There is no such thing here. I just want to see people read the config files before using it.
Only copy & paste configs without learn anything is not a Linux way. <br />
Regards, Addy.

## Motivational Quotes
"The Linux philosophy is *'Laugh in the face of danger'*. Oops! Wrong One. *'Do it yourself'*. Yes, that's it." -- Linus Torvalds

## My Links
[Google+](https://plus.google.com/+AdhiPambudi)
[Deviant Art](http://addy-dclxvi.deviantart.com/)
