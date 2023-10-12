# FedoraKDE-Dr460nized Custom

<p align="center">
<a><img src="https://i.imgur.com/GW2L0Oc.png" style="height: 25%; width:25%;"/></center></a></p>

My customization of my Fedora Linux 38 KDE Plasma. A small tutorial about the themes I use, programs, and more.

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

## Index: 

- [Download some resources](https://github.com/trbureiyan/fedorakde-dragonized/tree/e531906706c08d57b860d29954215e622c3b25bc/Resources) Credits to [@Sandip Sky](https://www.youtube.com/@sandipsky8756), Thanks for the resources.
  > There are files for Fish config, Starship prompt and Latte Dock profile.
- Tools that can we need
- Fonts
	- Optional fonts
	- Nerd Hacker Font
- Installing theme
	- Workspace Behavior
	- Startup and Shutdown
- Kvantum theme (Blur & transparency)

### Tools that we need

- 7z
- wget


#### We can start with something easy: installing fonts that I use.

##### Optional Fonts:

One of my favorite sources that you can implement them in your Linux customization however you want. These include:

- losevka
- Icomoon
- Material


###### 1. Installing opcional fonts:

**Iosevka**

---

> First, let's enter the fonts folder.
``` sh
cd /usr/share/fonts
```

> In root we'll to download a ZIP file.
``` sh
wget http://fontlot.com/downfi1e/5baeb08d06494fc84dbe36210f6fOad5.105610
```

> With 7z we can see the resources of the ZIP
``` sh
7z l 5baeb08d06494fc84dbe36210f6fOad5.105610
```

>Let's move the ZIP and rename them like:
``` sh
mv 5baeb08d06494fc84dbe36210f6fOad5.105610 compressed.zip
```

> And unzip it for the fonts folder.

``` sh
unzip compressed.zip
```

> We can now remove the ZIP file.

``` sh
rm compressed.zip
```

> With `find`, we can locate the font files that we'll use:

``` sh
find . | grep • "\.ttf$" while read line; do cp $line .; done
```
 
> Now we'll to remove the next directory:

``` sh
rm —r iosevka—2.2.1/
rm —r iosevka—slab-2.2.1/
```

> Finally, with `ls` we can confirm that the fonts are in the folder

**Icomoon** 

---
First, Let's download [the ZIP](https://icomoon.io/#icons-icomoon)

> Now, we move the zip to the actual directory:

``` sh
mv /home/"Type your user"/Downloads/"Name of icomoon font".zip .
```

> Unzip the file:

``` sh
unzip "Name of icomoon font".zip
```


> We move everything that ends in .ttf to the directory:

``` sh
mv icomoon/* . t tf
rm —r f icomoon
```


##### FiraSans & Hack Nerd Font

---

FiraSans fonts are at [/Resources](https://github.com/trbureiyan/fedorakde-dragonized/tree/0dafff438736cedeccac612491e9bd603df623eb/Resources/FiraSans_fonts)

> Try to click them and install the fonts, but if an error appears, let's try the next steps:

In your File manager, go to `/usr/share/fonts` and paste .ttf files on there.

**For Hack Nerd Font:**

Let's download the [fonts](https://www.nerdfonts.com/font-downloads):

> Move the ZIP files to the actual directory (/usr/share/fonts).

``` sh
mv /home/"Type your user"/Downloads/"Name of the Hack nerd font".zip .
```

> And unzip the font files:

``` sh
unzip "Name of the Hack nerd font".zip
```

### Installing theme

To install our theme, first open system settings, go to Appearance > Global Theme > Get New Global Themes.

// photo.jpg

Search for Sweet KDE by Eliverlara and install it.

// Photo.jpg

Once you have the global theme installed, go to Application style > Configure GNOME/GTK Application Style... > Get New GNOME/GTK Application Styles.

// Photo.jpg

Search for Sweet by Eliverlara (it may appear as "Sweet - New flavor").

// Photo.jpg

Now, select Sweet-dark GTK Theme.

Well. Now confirm that you have installed sweet plasma style and Sweet colors.

For our window customization, go to Window Decoration and apply the next setting:

// Photo.jpg

In Fonts, you can add the fonts that we installed previously like Fira Sans or Hack Nerd.

// Photo.jpg

In Icons, we'll use BeautyLine, so go to Download New Icons, search for BeautyLine by sajjad606, and install it.

// Photo.jpg

To use the chroma RGB cursor, go to Cursors > Get New Cursors, search for chroma cursor by vidmo1337, and install it.

// photo.jpg

You can use the splash screen that you like the most by seeking to Get New Splash Screens, or if you prefer, deactivate the splash screen. In my case, I use the Arch splash.

// photo.jpg

#### Workspace Behavior

##### Desktop Effects

We'll install Wobbly windows and Magic lamp. Search for Wobbly windows and turn it on, following the settings for the effect.

// photo.jpg
//photo.jpg

Also, enable Magic Lamp:

// photo.jpg

If you don't find Magic Lamp in your Desktop Effects, you can search for it in Get New Desktop Effects.

##### Screen Edges

As we will use Latte Dock and the top bar, to avoid inconvenience, let's disable the screen edges:

// photo.jpg

#### Startup and Shutdown

You can still use the Breeze login screen, but I like the Nordic login screen by Eliver Lara.

// photo.jpg

### Kvantum Theme

We'll install a theme with blur and transparency for Dolphin and Konsole.

First, we need the Kvantum engine. So let's go to Discover Store, search for Kvantum, and install the one called "Kvantum theme engine".

> If you encounter errors during installation, restart your computer and try again.

Now, go to [download](https://store.kde.org/p/1294013/) Sweet KDE theme for kvantum in the [next link](https://store.kde.org/p/1294013/).

Choose "Sweet-transparent-toolbar.tar.xz".

//photo.jpg 

Extract the zip archive

// photo.jpg

Now, open Kvantum Manager to proceed with the installation of the theme

> If the program doesn't open on the first try, try opening it again.

// photo.jpg

Select the theme that we downloaded previously and install it

// photo.jpg 

Go to the next tab, ("Change / Delete Theme") and select "Sweet-transparent-toolbar"

// photo.jpg

Well, now return to System Settings > Appearance > Application Style, select and apply kvantum-dark.

### Latte Dock




## Recommendations

---
