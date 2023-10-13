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
- Konsole Customization
	- Starship Prompt
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

Search for "KDE Plasma Desktop - Latte" in the Discover Store and install it.

![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/81660601-92fb-4af7-a924-0f9d26e61247)

Before customizing our Latte Dock and adding a top bar, let's install some widgets that we need:

First, go to your desktop, right-click, and select "Add Widgets"

![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/160203ac-2d9b-450a-9aa5-388688fa6dfe)

In the Widgets window, go to "Get New Widgets"

![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/376c9027-b771-4ee6-9c49-8a99b2412c10)

Search for the Window Buttons Applet by himdek.

![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/1aae4f19-854c-4cc5-b7d3-92388be3b09b)

And the Window Title Applet by Psifidotos.

![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/f4b42674-43ba-4d66-b749-d98d4a875758)

To fully apply the window title and avoid issues, go to your System Settings > Workspace > Window Management > KWin Scripts > Get New Scripts.

![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/fc33be5c-4fd5-472e-8ec9-bb23d9ad0cb8)

Then, install "Hide Titles" by bahamondev.

![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/4fb2585b-c46a-4252-9de3-865777a4b370)

#### Latte Dock Settings

---

Now, let's customize Latte Dock. To do this, open Latte Dock or right-click on any icon in the bottom bar and select "Configure Latte..."

![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/4fc06ad7-da49-4972-830f-5c36a6886c35)


> If the settings don't open on the first try, try opening them again.

In the settings, go to the Layouts Editor tab. You will have the Default profile. We'll install our Dr460nized profile. To do this, select "Import" > "Import From Local File..."

![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/1c2a8d57-7f02-4634-9186-85a4881c3b30)


And import [the file](https://github.com/trbureiyan/fedorakde-dragonized/blob/main/Resources/Dr460nized.layout.latte).

![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/8ae32876-39b7-4eeb-8b50-6cb8f0197d94)


Now, select the new profile and click on "Switch"

![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/89cd9ef0-4621-4f57-9fb2-cb2ba29e1330)


And now we have the dock both up and down.

Now you can discard or remove the KDE dock:

Right-click on the taskbar > Enter Edit Mode > Remove Panel.

![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/cd5cbfda-d56c-4cdc-8ffe-885f93178b90)
![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/dbe14c36-0374-4f62-a72b-f71100722809)


Now, you can remove the white icons or launchers without an icon by right-clicking and selecting "Unpin Launcher."

![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/7e5e6417-7368-4c90-b14b-76c5c374dea9)


#### Widgets

---

If you don't have the widgets in the top bar, like the window buttons we installed previously, you can add them by following these steps:

Go to Widgets by right-clicking on the bottom or top tab > "Add Widgets"

![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/915ed76b-f8c3-4197-b172-518cf19c557c)


Search for Window Button and drag it to the top bar on the left side.

![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/53f87021-cbd2-406e-a6a1-6df99e266167)


Now, let's configure the Window Buttons widget on the top bar.

Go to "Edit Panel"

![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/ca03505b-3470-4a17-b4c9-fb536300d255)


Configure the Window Button.

![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/2c211bf0-78e5-490c-a451-9fbffe1fc088)


And make sure that these settings are similar to my settings.

![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/7193b933-b3c7-4879-a7d8-5ed709e6c8e1)


Now, let's install other widgets.

As before, search for "Better Application Dashboard" by himdek. Right-click on the bar > "Add Widgets" > "Get New Widgets."

![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/8e9958fc-8c96-4b8b-9bc1-0aad9209a939)


And add the widget to the top bar.

![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/a00d342e-0116-45b6-8016-9b818589ce35)


You can also configure the widget, such as changing the icon.

![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/1d5a439e-5394-40f4-8201-8b7444e4ed10)
![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/f4498593-59cb-4d7a-941c-d37719c44b88)


And add a shortcut to access it.

![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/871d8491-b236-4a1f-9e56-86243be909dd)


> If you can't find the widget in the previous step, try finding it in the Discover Store > Plasma Addons > Plasma Widgets.

![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/e4ca6ef5-d20c-4492-9760-2d89418d5590)


Now that we're in Plasma Widgets, let's install our clock widget for the desktop. Search for "Clear Clock" by qewer.

![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/e485e791-4520-4b31-a3d5-21254ace3424)
![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/9dd69e1a-3e14-46d1-9f14-917a82bf804f)


Right-click on any empty space on your desktop and select "Add Widgets." Drag Clear Dock onto the desktop. If you want to configure it, just right-click on it.

![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/14fafedf-86c9-4921-83e4-acb3bdfb2617)

> If you have issues, or it bothers you that sometimes there are problems with some applications because it may not fit well or interfere with the top panel, you can make it hide automatically.

Right-click on any tab, and enter in Edit panel

![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/2e67d9b5-7a5e-49f7-9bee-3a0a606f4b38)

On latte configuration, search for Visibility and turn on Auto Hide.

![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/23f79a77-8b4d-45db-9cb5-67413249fd68)


### Konsole Customization

For our shell, we need to install fish first:

In Konsole / Shell run:


``` sh
sudo dnf install fish
```

Once fish is installed, let's enter Konsole Settings:

First, enter Profiles, create a New profile with the name that you prefer. In my case, I named the profile "Dragonized."

![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/a23cb652-ea0b-4b93-8ac0-92cdc36a1041)


Edit the profile, and ad `/bin/fish` in Command:

![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/86f199c3-c4f0-40fa-8a05-f7259192dd09)


Go to Appearance, select Edit, and set these settings:

![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/f8cd1c4d-ac14-4976-8d41-3a62524c1fb4)
![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/1c24a778-5b81-4d4f-9c69-576c2ea376e0)


In font, use Hack Nerd Font that we installed previously.

Now you can Apply and close the window, and finally set the new profile as Default.

#### Starship Prompt

Let's install the Starship Prompt.
First got to [starship.rs](https://starship.rs) and follow the installation instructions.

![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/80953f5e-4854-4f41-b813-954ae96a5aaf)


> You can check [the documentation](https://starship.rs/guide/) for more customization.

To follow the customization, copy the fish folder and starship archive.

![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/54579b37-55bc-482a-8157-4d1224db437c)


Go to your home directory and press ctrl + h to see the hidden folders.

![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/04c92d0d-77ed-484e-ad63-cc7a720f0f55)

Enter on .config

![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/bf4b7156-84d6-403f-b0bc-3d0378f1130e)


And paste the files that you copied previously into the folder.

![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/f5236539-078b-4249-8db7-113f89502d5b)


Close Konsole and open it again; now you will see the customized prompt.

![image](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/d44e8607-33c9-4a02-8324-577f3f2b4dad)


And that concludes the customization, but you can customize more and refer to the [starship.rs](https://starship.rs/) documentation.

Customize the fish shell by typing:
``` sh
fish_config
```
In Konsole. An HTML page will be displayed where you can configure your shell.

Thank you for reading and following this repository.

You can follow me on Instagram, Facebook, and Twitter as @trbureiyan.

See you!


## Wallpapers
---

![aestheticjapanese_wallpaper-transformed](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/61bd3895-8242-4810-91e1-c0fb7365708d)
![japanesesamurai_wallpaper-transformed](https://github.com/trbureiyan/fedorakde-dragonized/assets/111925453/f9ae4308-ee01-4eec-b819-80a13d2b1cb6)


## Recommendations
---

Don't remove the notification bar from the top bar because it may disable music control, and you will not be able to adjust the volume with any key.

---
