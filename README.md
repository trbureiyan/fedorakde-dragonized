# FedoraKDE-Dr460nized Custom

<p align="center">
<a><img src="https://i.imgur.com/GW2L0Oc.png" style="height: 25%; width:25%;"/></center></a></p>

My customization of my Fedora Linux 38 KDE Plasma. Small tutorial about the themes I use, programs, and more.

In this repository you'll find:

- fish & starship prompt
- Kvantum themes
- Plasma color (Sweet)
- Plasma Desktop theme (Sweet-Dark)
- Wallpapers
- Latte Dock profiles
- Plasma Widgets
- Plasma Global Theme
- Cursor skin / style
- Plasma Effects


## Screenshots

<p align="center">
<a><img src="https://i.imgur.com/kTh9IPc.png" style="height: 75%; width:75%;"/></center></a></p>
<p align="center">
<a><img src="https://i.imgur.com/zXiucom.png" style="height: 75%; width:75%;"/></center></a></p>
<p align="center">
<a><img src="https://i.imgur.com/5Owzmsy.jpg" style="height: 75%; width:75%;"/></center></a></p>
<p align="center">
<a><img src="https://i.imgur.com/lYEXonT.jpg" style="height: 75%; width:75%;"/></center></a></p>


## Details of my PC

- **OS:** [Fedora 38 KDE Plasma](https://fedoraproject.org/spins/kde/)
- **WM:** [kwin](https://userbase.kde.org/KWin)
- **Terminal:** [fish](https://fishshell.com)
- **Terminal Font:** [Hack Nerd Font 13](https://www.nerdfonts.com)
- **Editor:** [nano](https://www.nano-editor.org)
- **Theme:** [Plasma, Sweet-Dark (GTK2/3)](https://github.com/EliverLara/Sweet)
- **Theme Icons:** [BeautyLine](https://store.kde.org/p/1425426/)


## Setup / Installation

### Index: 

- [Download some resources](https://github.com/trbureiyan/fedorakde-dragonized/tree/e531906706c08d57b860d29954215e622c3b25bc/Resources) Credits to [@Sandip Sky](https://www.youtube.com/@sandipsky8756), Thanks for the resources.
  - There are files for fish config, starship prompt and latte dock profile.
- Nerd Hacker Font

#### Tools that we need

- 7z
- wget
- 


#### We can start with something easy, installing the font that i use

##### Opcional Fonts

One of my favorite sources, you can implement them in your Linux customization however you want.

There are:

- losevka
- Icomoon
- Material


###### 1. Installing opcional fonts:

**Iosevka**

---

> First let's enter the fonts folder:
``` sh
cd /usr/share/fonts
```

> In root we'll to download a ZIP file
``` sh
wget http://fontlot.com/downfi1e/5baeb08d06494fc84dbe36210f6fOad5.105610
```

> With 7z we can see the resources of the ZIP
``` sh
7z l 5baeb08d06494fc84dbe36210f6fOad5.105610
```

>Let's move the ZIP and rename them like
``` sh
mv 5baeb08d06494fc84dbe36210f6fOad5.105610 compressed.zip
```

> And unzip it for the fonts folder

``` sh
unzip compressed.zip
```

> We can now remove the ZIP file

``` sh
rm compressed.zip
```

> With `find` we can locate the font files that we'll use

``` sh
find . | grep • "\.ttf$" while read line; do cp $line .; done
```
 
> Now we'll to remove the next directory

``` sh
rm —r iosevka—2.2.1/
rm —r iosevka—slab-2.2.1/
```

> Finally with `ls` we can confirm that the fonts are in the folder

**Icomoon** 

---

First Let's download [the ZIP](https://icomoon.io/#icons-icomoon)

> Now we move the zip to actual directory

``` sh
mv /home/"Type your user"/Downloads/"Name of icomoon font".zip .
```

> Unzip the file

``` sh
unzip "Name of icomoon font".zip
```


> We move everything that ends in .ttf to the directory

``` sh
mv icomoon/* . t tf
rm —r f icomoon
```


##### FiraSans & Hack Nerd Font

---

FiraSans fonts is at [/Resources](https://github.com/trbureiyan/fedorakde-dragonized/tree/0dafff438736cedeccac612491e9bd603df623eb/Resources/FiraSans_fonts)

> Try to click them and install the fonts, but if an error appears, let's try the next steps:

In your File manager, go to `/usr/share/fonts` and paste .ttf files on there.

**For Hack Nerd Font:**

Let's download the [fonts](https://www.nerdfonts.com/font-downloads):

> Move the ZIP files to the actual directory (/usr/share/fonts)

``` sh
mv /home/"Type your user"/Downloads/"Name of the Hack nerd font".zip .
```

> And unzip the font files

``` sh
unzip "Name of the Hack nerd font".zip
```

#### Installing theme



## Recommendations

---
