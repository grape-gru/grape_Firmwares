<h1 align="center">grapes- <code> "not-so extreme" girmware</code> for the slipper fero</h1>
<h3 align="center">doesn't blow smoke up your ass</h3>

<p align="center">
  <img src="https://user-images.githubusercontent.com/55334727/215170306-051eeb8f-8f72-437f-8c2d-0e4be009bdad.png">
</p>

[Intro](https://github.com/ClaraCrazy/Flipper-Xtreme#What-makes-it-special) | [Animations](https://github.com/ClaraCrazy/Flipper-Xtreme#Animations--Asset-Packs) | [Wiki](https://github.com/ClaraCrazy/Flipper-Xtreme/wiki) | [Changelog](https://github.com/ClaraCrazy/Flipper-Xtreme#list-of-changes) | [Known bugs](https://github.com/ClaraCrazy/Flipper-Xtreme/issues?q=is%3Aissue+is%3Aopen+label%3Arelease-pending) | [Install](https://github.com/ClaraCrazy/Flipper-Xtreme#Install) | [Build](https://github.com/ClaraCrazy/Flipper-Xtreme#build-it-yourself) | [Discord](https://discord.gg/flipper-xtreme) | [Donate](https://github.com/ClaraCrazy/Flipper-Xtreme#%EF%B8%8F-support)
-----

This firmware is a complete overhaul of the [Official Firmware](https://github.com/flipperdevices/flipperzero-firmware), and also features lots of awesome code-bits from [Unleashed](https://github.com/DarkFlippers/unleashed-firmware).

-----
<br>
<h2 align="center">why does this section try to sell you on something you already bought?</h2>

nothing. its just not annoying or attached to idiot children and their precious cult. 
<br><br>
- <h4>blowing smoke up your ass for no raisin!!!</h4>

- <h4>lies upon lies upon lies</h4>

- <h4>just make your own and stop reading this horrible bullshit written by some 13 yr old.</h4>
<br><br>
A full list of changes can be found [here](https://github.com/ClaraCrazy/Flipper-Xtreme/wiki/Customization)

-----
<br>
<h2 align="center">grape_ Settings:</h2>

stole some shit from people who actually wrote it. whatever, its fucking gpl, LFG!!!

<img src="https://user-images.githubusercontent.com/49810075/228392945-1e68b996-4e2c-46c6-8aae-d0aadd8ea001.gif" align="left" width="400px"/>

<ins><b>Interface:</b></ins>
Change meaningless shit from the desktop animations, to the main menu apps, lockscreen style, statusbar items and screen options like dark mode and lefty mode.

<ins><b>Protocols:</b></ins>
Toggle USB & Bluetooth mode for our Bad-Keyboard app, and manage Subghz settings.

<ins><b>Misc:</b></ins>
Change Flipper's name, xp level, manage settings for RGB backlight.

<br clear="left"/>

-----
<br>
<h2 align="center">Animations / Asset Packs:</h2>

stole some anims but there's a guide to make some more, if you give a shit!!!

<img src="https://user-images.githubusercontent.com/55334727/214010675-9eddb8f5-1dd6-4cf4-a0ee-e37af8b6c933.PNG" align="left" width="200px"/>
You can easily create your own pack, or find some user made ones in the discord channel. Check <a href="https://github.com/ClaraCrazy/Flipper-Xtreme/wiki/Asset-Packs">here</a> for a tutorial on creating your own. Essentially, we got our own <code>Anims</code> & <code>Icons</code> folders, inside each <code>Asset Pack</code>.

<br clear="left"/>

<br>

<img src="https://user-images.githubusercontent.com/55334727/214016338-95a619c7-88d2-4db5-bb7a-75282d9082b8.png" align="left" width="200px"/>
Once you have some packs, upload them to your Flipper in <code>SD/dolphin_custom</code> (if you did this right you should see <code>SD/dolphin_custom/PackName/Anims</code> and/or <code>SD/dolphin_custom/PackName/Icons</code>).


<br clear="left"/>

<br>

<img src="https://user-images.githubusercontent.com/55334727/214013624-25dad48e-72ea-4a90-9060-66e137e0d61a.png" align="left" width="200px"/>
After installing the packs to Flipper, hit the <code>Arrow UP</code> button on the main menu and go to <code>Xtreme Settings</code>. Here choose which pack you want and tweak the other settings how you prefer, then press back to reboot and enjoy your new assets for all apps (e.g. Subghz scanning asset) & animations!

<br clear="left"/>

-----
<br>
<h2 align="center">Bad Keyboard:</h2>

<img src="https://user-images.githubusercontent.com/49810075/223855940-b8ee6770-4520-4bcc-a4cc-089196cf904b.png" align="left" width="250px"/>

BadUSB is a wonderful app, but it lacks bluetooth capabilities. Now some might argue that its useless as you will always need authentication from both sides, but what if I told you that we found a solution to this problem?
<br><br>
Bad-KB allows you to toggle between USB and Bluetooth mode for your attacks. In Bluetooth mode it allows you to spoof the name & MAC of the device to whatever you want. Being a JBL speaker or a wireless razer keyboard is easily doable, allowing you to trick people so you can run your payloads without needing a cable at hand.

-----
<br>
<h2 align="center">Levels:</h2>

This Firmware has 30 levels, not just the basic 3 the official one has.

With this new system in place, it allows for some cool stuff like locking animations behind a certain level. This can be done fairly easy: The idle_animations are tied to the level system. Specifically, the `Min level` variable of your manifest file is used here. Each level you reach, unlocks a new animation. The higher your level, the more animations people can see.

<details>
<summary>Our example</summary>

In our example case, this is used with the NSFW animation pack you can select in the Xtreme app. Dont worry, this is not used by default because I know not everyone likes to see my / anime tits and thats fine. Anyways.. each level gives a brand new background animation, they also become more and more lewd over time.

| Level  | Animations |
| ------------- | ------------- |
| 1-10  | Try harder. Just sexy clothes |
| 11-20 | Some tits, maybe an ass |
| 21-30 | Fully NSFW, graphic scenes |

</details>

-----
<br>
<h2 align="center">List of changes:</h2>

Note: This repo is always updated with OFW & Unleashed. No need to mention all those here. We will only mention **our** changes that we can actually be credited for.

```txt
[Added]

- Xtreme App
- Asset Packs
- More UI options
- Bad-Keyboard App
- A new battery display-type
- Scrolling view for long file names in browser
- NSFW Animations tied to the level system. Read more above
- Folder handling for empty ones (Now indicate they are empty)

- Custom subghz presets
- Multiple NFC protocols
- Multiple Sub-Ghz protocols | Merged from Unleashed, thanks @xMasterX
- Subghz and IR signal replication via gpio | Credits to @ankris812

- New API Routes for Locale settings
```
```txt
[Updated]

- All Assets

- Tons of apps
- File browser
- Massive compiler re-do
- About 4k files to speed things up a lot
- Applications to now use the new Locale setting
```
```txt
[Fixed]

- Keyboard issues on first char
- Passport crash on high level
- SFW / Dummy_mode getting you XP
- Leveling system
- Mood system
```
```txt
[REMOVED]

- Unused Dummy Mode
- Broken apps (bad apple, chess, etc.)
- Tons of unused code from FAPs and system calls
```

----
<br>
<h2 align="center">Install:</h2>
<br>

There are 3 methods to install Xtreme, we recommend you use the **Web Updater**, but choose whichever one you prefer:

<br>

> <details><summary><code>Web Updater (Chrome)</code></summary><ul>
>   <li>Open the <a href="https://github.com/ClaraCrazy/Flipper-Xtreme/releases/latest">latest release page</a> and click on the <code>Web Updater</code> link</li>
>   <li>Make sure qFlipper is closed</li>
>   <li>Click <code>Connect</code> and select your Flipper from the list</li>
>   <li>Click <code>Install</code> and wait for the update to complete</li>
> </ul></details>

> <details><summary><code>qFlipper Package (.tgz)</code></summary><ul>
>   <li>Download the qFlipper package (.tgz) from the <a href="https://github.com/ClaraCrazy/Flipper-Xtreme/releases/latest">latest release page</a></li>
>   <li>Open <a href="https://flipperzero.one/update">qFlipper</a> and connect your Flipper</li>
>   <li>Click <code>Install from file</code></li>
>   <li>Select the .tgz you downloaded and wait for the update to complete</li>
> </ul></details>

> <details><summary><code>Zipped Archive (.zip)</code></summary><ul>
>   <li>Download the zipped archive (.zip) from the <a href="https://github.com/ClaraCrazy/Flipper-Xtreme/releases/latest">latest release page</a></li>
>   <li>Extract the archive. This is now your new Firmware folder</li>
>   <li>Open <a href="https://flipperzero.one/update">qFlipper</a>, head to <code>SD/Update</code> and simply move the firmware folder there</li>
>   <li>On the Flipper, hit the <code>Arrow Down</code> button, this will get you to the file menu. In there simply search for your updates folder</li>
>   <li>Inside that folder, select the Firmware you just moved onto it, and run the file thats simply called <code>Update</code></li>
> </ul></details>

<br>

**If you have issues or crashes with the install process, you can try to use `Settings > Storage > Factory Reset` then retry the install.**
**Doing that will NOT remove your saved files, it will only forget some settings and paired devices.**

----
<br>
<h2 align="center">Build it yourself:</h2>

```bash
To download the needed tools:
$ git clone --recursive https://github.com/ClaraCrazy/Flipper-Xtreme.git
$ cd Flipper-Xtreme/

To flash directly to the Flipper (Needs to be connected via USB, qFlipper closed)
$ ./fbt flash_usb

To just compile firmware
$ ./fbt updater_package

If building FAPS:
$ ./fbt fap_dist

If building image assets:
$ ./fbt resources icons dolphin_ext
```

----


