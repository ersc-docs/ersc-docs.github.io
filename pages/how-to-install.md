---
layout: page
title: How to install
permalink: /how-to-install/
nav_order: 1
---
<details markdown="block">
<summary>Table of Contents</summary>

> * [**How to Install**](#how-to-Install)
>   *   [Video Guide](#video-guide-of-seamless-coop-151-by-layka)
>   *   [Text instructions](#video-guide-of-seamless-coop-151-by-layka)
>   *   [Linux/Steam Deck](#linuxsteam-deck-launch-script)
> * [**How to Update**](#new-item-guide)
> * [**New Item Guide**](#new-item-guide)
>   * [For basic use](#for-basic-use)
</details>

# How to Install

## Video guide of Seamless Coop 1.5.1, by Layka:  
<iframe width="560" height="315" src="https://www.youtube.com/embed/PMHcGmmhXN4" frameborder="0"></iframe>

## Text instructions

0. Purchase the game on Steam. Each player must have access to a unique copy.  
    
    **IMPORTANT**: There will be no compatibility or support for pirated copies of the game. Any discussion involving it will result in an immediate ban.
  
1. Get the latest version of the mod from:
    [Nexusmods](https://www.nexusmods.com/eldenring/mods/510?tab=files)  
    Use `MANUAL DOWNLOAD`. There is no need to install Nexus Mods' Mod Manager.  
    
    **IMPORTANT**: All players must use the same version. If you are starting to play with a new group, it's highly recommended you all update to the latest version.
  
2. In Steam, right click `Elden Ring`. Then click `Manage`, and `Browse local files`.
  
3. Enter the `Game` folder.
  
4. Extract the archive from Step 1 into this folder. A successful installation will look like this:
<a href="/assets/img/sucessful_installation.png"><img src="/assets/img/sucessful_installation.png" width="720"></a>
  
5. Open the `SeamlessCoop` folder.
  
6. Open `seamlesscoopsettings.ini` using any text editor - Notepad (Windows) or nano (Linux) is sufficient.
  
7. Edit the settings to your personal liking - by editing the values after ` = `. the only setting that has to be the same for everyone in the play group is the password. Do not delete any lines or write stuff in non-deisgnated places.  
    An example of a properly configured ini:

```ini
[PASSWORD]

; Set your co-op password. This cannot be blank
; You must set a secure and unique password, then share it with those who you'd like to play with
; Simple passwords are not recommended, secure ones could be for example a random series of numbers and letters
; You must have a space after the '=' (e.g. cooppassword = example)
cooppassword = seamless

[SETTINGS]

; Replaces the 'Host of Fingers' text above players
; 0 = Off (no text)
; 1 = Generic ('Host of Fingers' displayed)
; 2 = Ping view (player ping will be displayed instead (in ms))
playerhud = 0

; Whether to dock the HUD which appears above players
; 0 = Automatic
; 1 = Permanently docked
dockplayerhud = 1

; The file extension at the end of your seamless co-op saves you don't need to add a "."
; (e.g. savefileext = mywarriorplayerthrough) will produce a save file named "ER0000.mywarriorplayerthrough"
; A few rules:
; - Only alphanumeric characters
; - Don't use the game's default (sl2)
savefileext = co2
```
**IMPORTANT**: There might be changes to the ini in the future, in the form of new features or field name changes. When updating, it is recommended to run over it and with the new ini and set your settings again.
  
**If you are on Windows**, this is the end of the installation for you - return to the `Game` folder, and open `launch_elden_ring_seamlesscoop.exe`. If there is no EAC splash screen on launch, the mod was installed correctly!

**NOTE**: If you are getting `Inappropriate Activity Detected` after mod launch, that means that it failed to load. Some antiviruses can false flag and prevent the mod from hooking into the game - disable or uninstall them to resolve this.

(Optional) Create a shortcut to `launch_elden_ring_seamlesscoop.exe` on your desktop - this can be done by right clicking the launcher and pressing Create shortcut (under More options in Windows 11). Drag and drop the resulting shortcut to your desktop.
  
## Linux/Steam Deck:
There are multiple ways to make the mod work on Linux and Steam Deck. Here's a few ways we know work.
### Solution 1 - Non-steam app
1. Add `launch_elden_ring_seamlesscoop.exe` as non-steam app in Steam  
  On Desktop (desktop mode for Steam Deck) this can be done from the "Add a game" button in the lower left corner of the Steam client, then find and select the the executable in the game folder.
2. Open up the properties menu of the new `launch_elden_ring_seamlesscoop.exe` entry in Steam. Feel free to rename it to whatever you like
3. On the "Compatibility" page, you'll want to set your preferred Proton version. If you don't know what to pick, Proton 8.0 or 7.0 should work fine.

You should be able to launch the mod via this new entry now.  
If important, it will have its own separate location for saves.

### Solution 2 - Install script
> [rentry.org/er-coop-deck](https://rentry.org/er-coop-deck)  
> Credit to david2775 on Discord
  
Open Elden Ring's launch options, and paste the following:
```ini
DXVK_FRAME_RATE=58 PROTON_SET_GAME_DRIVE=1 VKD3D_FEATURE_LEVEL=12_0 DXVK_STATE_CACHE=1 DXVK_ASYNC=1 /bin/bash ./launch_elden_ring_seamlesscoop.sh %command%
```

A selection box will now appear whenever trying to launch Elden Ring, allowing you to choose whether to play Seamless Coop (default) or Vanilla.

Video guide for Linux:  
<video controls src="/assets/vid/er-seamless-deck.mp4" width=720 title="Linux video guide"></video>

# How to Update

To update the mod, simply repeat steps 1-7 of the installation instructions.  

Keep in mind, every Elden Ring update (by FromSoftware) is expected to break all the mods, including Seamless Coop, until they're updated. Since the game is still actively supported, updating the mod is a regular practice.  

<a href="/assets/img/how_to_update_seamless.gif"><img src="/assets/img/how_to_update_seamless.gif" width="600"></a>
   
# New Item Guide

**IMPORTANT**: Seamless Coop adds new items to the game. They're added automatically to any character that doesn't have them upon load. **They all have item descriptions detailing their use**.

## For basic use
* One player must use the `Tiny Great Pot` to start a session.
* All other players must use the `Effigy of Malenia` to join that session.
* To end a session for yourself, a player must use the `Separation Mist`. Only once you aren't in a session you'll be able to properly quit the game.
