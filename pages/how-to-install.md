---
layout: page
title: How to install and update
permalink: /how-to-install-and-update/
nav_order: 1
redirect_from: /how-to-install/
---
<details markdown="block">
<summary>Table of Contents</summary>

> * [**How to Install**](#how-to-Install)
> * [**How to Update**](#new-item-guide)
> * [**New Item Guide**](#new-item-guide)
>   * [For basic use](#for-basic-use)
</details>

# How to Install

0. Purchase the game on Steam. Each player must have access to a unique copy.  
    
    **IMPORTANT**: There will be no compatibility or support for pirated copies of the game. Any discussion involving it will result in an immediate ban.
  
1. Get the latest version of the mod from:
    [Nexusmods](https://www.nexusmods.com/eldenring/mods/510?tab=files)  
    Use `MANUAL DOWNLOAD`. There is no need to install Nexus Mods' Mod Manager.  
    
    **IMPORTANT**: All players must use the same version. If you are starting to play with a new group, it's highly recommended you all update to the latest version.
  
2. In Steam, right click `Elden Ring`. Then click `Manage`, and `Browse local files`.
  
3. Enter the `Game` folder.

4. If you have installed Seamless Coop in the past, delete both `launch_elden_ring_seamlesscoop.exe` and the `SeamlessCoop` folder:
<a href="/assets/img/legacy_installation.png"><img src="/assets/img/legacy_installation.png" width="720"></a>
  
6. Extract the archive from Step 1 into this folder. A successful installation will look like this:
<a href="/assets/img/successful_installation.png"><img src="/assets/img/successful_installation.png" width="720"></a>
  
7. Open the `SeamlessCoop` folder.
  
8. Open `ersc_settings.ini` using any text editor - Notepad (Windows) or nano (Linux) is sufficient.
  
9. Edit the settings to your personal liking - by editing the values after ` = `. the only setting that has to be the same for everyone in the play group is the password. Do not delete any lines or write stuff in non-designated places.  
    An example of a properly configured ini:

```ini
[GAMEPLAY]

; Invaders are other players that will join your world uninvited and try to kill you and your party
allow_invaders = 1

; Debuffs (Rot Essence) will be acquired when you die, and will only be cured when you sit at a bonfire
death_debuffs = 1

; Spirit summons can aid you in multiplayer
allow_summons = 1

; 0 = Normal | 1 = None | 2 = Display player ping | 3 = Display player soul level | 4 = Display death count
overhead_player_display = 3


[SCALING]

; Amount of health (%) per player for each enemy
enemy_health_scaling = 10

; Amount of damage (%) per player for each enemy
enemy_damage_scaling = 20

; Amount of posture absorption (%) per player for each enemy
enemy_posture_scaling = 30

; Amount of health (%) per player for bosses
boss_health_scaling = 40

; Amount of damage (%) per player for bosses
boss_damage_scaling = 50

; Amount of posture absorption (%) per player for bosses
boss_posture_scaling = 60

[PASSWORD]

; Session password
cooppassword = bingusISreal

[SAVE]

;Your save file extension (in the vanilla game this is .sl2). Use any alphanumeric characters (limit = 120)
save_file_extension = co2

[LANGUAGE]

;Leave this blank unless you want to load a custom locale file. The mod will default to your game language.
mod_language_override = hungarian
```
**IMPORTANT**: There might be changes to the ini in the future, in the form of new features or field name changes. When updating, it is recommended to run over it and with the new ini and set your settings again.
  
**If you are on Windows**, this is the end of the installation for you - return to the `Game` folder, and open `ersc_launcher.exe`. If there is no EAC splash screen on launch, the mod was installed correctly!

**NOTE**: If you are getting `Inappropriate Activity Detected` after mod launch, that means that it failed to load. Some antiviruses can false flag and prevent the mod from hooking into the game - disable or uninstall them to resolve this.

(Optional) Create a shortcut to `ersc_launcher.exe` on your desktop - this can be done by right clicking the launcher and pressing Create shortcut (under More options in Windows 11). Drag and drop the resulting shortcut to your desktop.

**If you are on Linux**, add `ersc_launcher.exe` to Steam as a Non-Steam game, and launch it from there:
1. On Desktop (desktop mode for Steam Deck) this can be done from the "Add a game" button in the lower left corner of the Steam client, then find and select the the executable in the game folder.
2. Open up the properties menu of the new `ersc_launcher.exe` entry in Steam. Feel free to rename it to whatever you like
3. On the "Compatibility" page, you'll want to set your preferred Proton version. If you don't know what to pick, Proton 8.0 or 7.0 should work fine.

# How to Update

To update the mod, simply repeat steps 1-9 of the installation instructions.  

Keep in mind, every Elden Ring update (by FromSoftware) is expected to break all the mods, including Seamless Coop, until they're updated. Since the game is still actively supported, updating the mod is a regular practice.  

<a href="/assets/img/how_to_update_seamless.gif"><img src="/assets/img/how_to_update_seamless.gif" width="600"></a>
   
# New Item Guide

**IMPORTANT**: Seamless Coop adds new items to the game. They're added automatically to any character that doesn't have them upon resting at a grace. **They all have item descriptions detailing their use**.

## For basic use
* One player must use the `Tiny Great Pot` to start a session.
* All other players must use the `Effigy of Malenia` to join that session.
* To end a session for yourself, a player must use the `Separation Mist`. Only once you aren't in a session you'll be able to properly quit the game.
