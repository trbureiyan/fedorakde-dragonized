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
- Latte dock
	- Latte dock settings
	- Widgets
- Wallpapers
- Recommendations

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
---

To install our theme, first open system settings, go to Appearance > Global Theme > Get New Global Themes.

![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/2063e60e-9831-4437-bc2d-b595c954a5ed)

Search for Sweet KDE by Eliverlara and install it.

![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/0e23c463-ddd4-4845-b305-0dd738a7571b)


Once you have the global theme installed, go to Application style > Configure GNOME/GTK Application Style... > Get New GNOME/GTK Application Styles.

![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/5f918ca5-4b10-45e0-85c7-07f3c4f9ec43)


Search for Sweet by Eliverlara (it may appear as "Sweet - New flavor").

![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/405928fe-7e07-41a5-a391-5f1b37ba83b7)


Now, select Sweet-dark GTK Theme.

![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/05ed2a3d-cb0d-4001-9edf-66d8508a3eff)


Well. Now confirm that you have installed sweet plasma style and Sweet colors.

For our window customization, go to Window Decoration and apply the next setting:

![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/b3e80d57-0e2e-4738-9907-2efe39341e99)


In Fonts, you can add the fonts that we installed previously like Fira Sans or Hack Nerd.

![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/0a60ec61-f3bc-4b3f-b462-f8ac286d4de8)


In Icons, we'll use BeautyLine, so go to Download New Icons, search for BeautyLine by sajjad606, and install it.

![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/8a3981de-56ef-4ce0-861a-59dbebc26198)
![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/b49973f3-de59-44f5-9735-1a1d46be2157)


To use the chroma RGB cursor, go to Cursors > Get New Cursors, search for chroma cursor by vidmo1337, and install it.

![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/8baf2b18-7b76-4298-a6bb-5489fc1ab3f9)
![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/c1212caa-c147-4487-998e-92513d6b6a0d)


You can use the splash screen that you like the most by seeking to Get New Splash Screens, or if you prefer, deactivate the splash screen. In my case, I use the Arch splash.

![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/26312221-7baa-4e61-8706-7a710558c353)


#### Workspace Behavior
---

##### Desktop Effects

![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/c7ec6301-da09-4291-be63-d269b6fde311)


We'll install Wobbly windows and Magic lamp. Search for Wobbly windows and turn it on, following the settings for the effect.

![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/27c8d784-e56b-43a0-8388-9860aabdaba8)
![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/b7f8bf47-7ebc-4465-8647-fd02a8609eab)

Also, enable Magic Lamp:

![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/e1f75ffd-041e-4aaf-8e33-0ed162cdf416)

If you don't find Magic Lamp in your Desktop Effects, you can search for it in Get New Desktop Effects.

##### Screen Edges

As we will use Latte Dock and the top bar, to avoid inconvenience, let's disable the screen edges:

![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/9b990877-bd94-4b75-a2cc-68ab3d6acc4c)


#### Startup and Shutdown

You can still use the Breeze login screen, but I like the Nordic login screen by Eliver Lara.

![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/a5b9de6e-6dfd-43a1-85a5-2d7e48702669)


### Kvantum Theme

We'll install a theme with blur and transparency for Dolphin and Konsole.

First, we need the Kvantum engine. So let's go to Discover Store, search for Kvantum, and install the one called "Kvantum theme engine".

![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/4cac0d16-21c9-4552-963b-42b44a649132)


> If you encounter errors during installation, restart your computer and try again.

Now, go to [download](https://store.kde.org/p/1294013/) Sweet KDE theme for kvantum in the [next link](https://store.kde.org/p/1294013/).

Choose "Sweet-transparent-toolbar.tar.xz".

![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/fdae0e7f-ff9f-493a-a885-dfb651878a06)


Extract the zip archive

![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/a3ea469c-2533-4ed4-a01d-b0345113173a)


Now, open Kvantum Manager to proceed with the installation of the theme

> If the program doesn't open on the first try, try opening it again.

![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/60449de8-1852-49eb-b6e3-35c869d11c59)

Select the theme that we downloaded previously and install it

![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/fedaafe5-19d0-45e1-a635-496d01321b13)


Go to the next tab, ("Change / Delete Theme") and select "Sweet-transparent-toolbar"

![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/812069b6-0706-45a2-b268-f878fecc3d89)

Well, now return to System Settings > Appearance > Application Style, select and apply kvantum-dark.

### Latte Dock

---

Search for "KDE Plasma Desktop - Latte" on the Discover Store and install it.

// photo.jpg

Before customizing our Latte Dock and adding a top bar, let's install some widgets that we need:

First, go to your desktop, right-click, and select "Add Widgets."

// Photo.jpg

In the Widgets window, go to "Get New Widgets."

// Photo.jpg

Search for the Window Buttons Applet by himdek.

// photo.jpg

And the Window Title Applet by Psifidotos.

// photo.jpg

To fully apply the window title and avoid issues, go to your System Settings > Workspace > Window Management > KWin Scripts > Get New Scripts.

Then, install "Hide Titles" by bahamondev.

// photo.jpg

#### Latte Dock Settings

---

Now, let's customize Latte Dock. To do this, open Latte Dock or right-click on any icon in the bottom bar and select "Configure Latte..."

// photo.jpg

> If the settings don't open on the first try, try opening it again.

In the settings, go to the Layouts Editor tab. You will have the Default profile. We'll install our Dr460nized profile. To do this, select "Import" > "Import From Local File..."

// photo.jpg

And import [the file](https://github.com/trbureiyan/fedorakde-dragonized/blob/main/Resources/Dr460nized.layout.latte).

// photo.jpg

Now, select the new profile and click on "Switch."

// Photo.jpg

And now we have the dock both up and down.

Now you can discard or remove the KDE dock:

Right-click on the taskbar > Enter Edit Mode > Remove Panel.

// photo.jpg 
// photo.jpg

Now, you can remove the white icons or launchers without an icon by right-clicking and selecting "Unpin Launcher."

#### Widgets

---

If you don't have the widgets in the top bar, like the window buttons we installed previously, you can add them by following these steps:

Go to Widgets by right-clicking on the bottom or top tab > "Add Widgets."

// photo.jpg

Search for Window Button and drag it to the top bar on the left side.

Now, let's configure the Window Buttons widget on the top bar.

Go to "Edit Panel."

// photo.jpg

Configure the Window Button.

// photo.jpg

And make sure that these settings are similar to my settings.

// photo.jpg

Now, let's install other widgets.

As before, search for "Better Application Dashboard" by himdek. Right-click on the bar > "Add Widgets" > "Get New Widgets."

// photo.jpg

And add the widget to the top bar.

// photo.jpg

You can also configure the widget, such as changing the icon.

// photo.jpg // photo.jpg

And add a shortcut to access it.

> If you can't find the widget in the previous step, try finding it on the Discover Store > Plasma Addons > Plasma Widgets.

// photo.jpg

Now that we're in Plasma Widgets, let's install our clock widget for the desktop. Search for "Clear Clock" by qewer.

// photo.jpg

Right-click on any empty space on your desktop and select "Add Widgets." Drag Clear Dock onto the desktop. If you want to configure it, just right-click on it.

> If you have issues, or it bothers you that sometimes there are problems with some applications because it may not fit well or interfere with the top panel, you can make it hide automatically.


## Wallpapers
---



## Recommendations
---

No quites la barra de notificaciones de la barra superior, porque puede que deshabilites el control de música y no puedas subir volumen con alguna tecla

---
