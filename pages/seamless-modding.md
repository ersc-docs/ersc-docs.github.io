---
layout: page
title: Seamless Modding
permalink: /seamless-modding/
nav_order: 2
---
<details markdown="block">
<summary>Table of Contents</summary>

> * [**Installation Guide**](#installation-guide)
> * [**Uninstall Guide**](#uninstall-guide)
</details>

## INSTALLATION GUIDE:  
This guide will go over using Seamless Coop in conjunction with other mods.
For optimal experience, all players should use the same mods together - with the exception for visual mods, which can remain personal.

  
> <b><u>IMPORTANT NOTE</u></b>: This will prevent you from launching vanilla Elden Ring, as EAC will fail to verify the modded files - unlike the standalone install.  

Seamless Coop will also not be able to start from the standalone launcher.
  
> <b><u>NOTE</u></b>: This guide was written with file extensions **ENABLED**. If some file names do not match what you're seeing, please turn this setting on in File Explorer:  
<a href="https://i.imgur.com/sBU3kWt.png"><img src="https://i.imgur.com/sBU3kWt.png" width="600"></a>
  
1\. Download the following:
   1. [Elden Mod Loader](https://www.nexusmods.com/eldenring/mods/117)
   2. [Seamless Coop, version 1.7.2](https://www.nexusmods.com/eldenring/mods/510)  
   3. [Mod Engine 2](https://github.com/soulsmods/ModEngine2/releases)
   4. Latest versions of the mods of your choosing.

> <u><b>IMPORTANT NOTE</b></u>: Mods have to be compatible with the version of Elden Ring you're using. Typically only the latest version of Elden Ring is supported, and if the mod has been abandoned you will not be able to use it.  
> <u><b>IMPORTANT NOTE</b></u>: All players must use the same mods in order to connect to each other.
  
2\. In Steam, right click `Elden Ring`. Then click `Manage`, and `Browse local files`.
  
3\. Enter the `Game` folder.
  
4\. Extract `Elden Mod Loader` (file 1.i) into your `Game` folder:  
<a href="https://i.imgur.com/ZTnDDdj.png"><img src="https://i.imgur.com/ZTnDDdj.png" width="600"></a>
  
5\. Extract `Seamless Coop` (file 1.ii) into your `Game` folder:  
<a href="https://i.imgur.com/z7p8cRT.png"><img src="https://i.imgur.com/z7p8cRT.png" width="600"></a>
  
6\. Enter the `SeamlessCoop` folder, and select `ersc.dll`, `ersc_settings.ini` and the `locale` folder:  
# <a href="https://i.imgur.com/wLRTgWN.png"><img src="https://i.imgur.com/wLRTgWN.png" width="600"></a>
  ![image](https://github.com/ersc-docs/ersc-docs.github.io/assets/174225858/531629d7-504f-497f-9792-a4645e0638f4)

7\. Copy and paste them into the `mods` folder:  
# <a href="https://i.imgur.com/EFmxOBC.png"><img src="https://i.imgur.com/EFmxOBC.png" width="600"></a>
  ![image](https://github.com/ersc-docs/ersc-docs.github.io/assets/174225858/bff6984a-de72-460e-a4a5-225c6f770511)

8\. Edit the settings to your personal liking - by editing the values after `=`. the only setting that has to be the same for everyone in the play group is the password. Do not delete any lines or write stuff in non-designated places.
    An example of a properly configured ini:

```ini
[GAMEPLAY]

; Invaders are other players that will join your world uninvited and try to kill you and your party
allow_invaders = 1

; Debuffs (Rot Essence) will be acquired when you die, and will only be cured when you sit at a bonfire
death_debuffs = 1

; Spirit summons can aid you in multiplayer
allow_summons = 0

; 0 = Normal | 1 = None | 2 = Display player ping | 3 = Display player soul level | 4 = Display death count
overhead_player_display = 4


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
cooppassword = reforgedfloppa

[SAVE]

;Your save file extension (in the vanilla game this is .sl2). Use any alphanumeric characters (limit = 120)
save_file_extension = err

[LANGUAGE]

;Leave this blank unless you want to load a custom locale file. The mod will default to your game language.
mod_language_override = japanese
```
> <b><u>IMPORTANT NOTE</u></b>: There might be changes to the ini in the future, in the form of new features or field name changes. When updating Seamless Coop, it is recommended to overwrite it with the new ini and configure your settings again.

  
9\. Go back to the `Game` folder.

10\. Open `mod_loader_config.ini`

11\. Change `exmaple.dll = 1` to `ersc.dll = 0`

12\. Save the file.
   
13\. Create a folder named `ModEngine2`:  
<a href="https://i.imgur.com/4f9l8it.png"><img src="https://i.imgur.com/4f9l8it.png" width="600"></a>
  
14\. Extract `Mod Engine 2` (file 1.iii) into the `ModEngine2` folder:  
<a href="https://i.imgur.com/od0fvlU.png"><img src="https://i.imgur.com/od0fvlU.png" width="600"></a>
  
(Optional) Create a shortcut to `launchmod_eldenring.bat` on your desktop - this can be done by right clicking the file and pressing `Create shortcut` (under `More options` in Windows 11). Drag and drop the resulting shortcut to your desktop.

  
15\. Run `launchmod_eldenring.bat` once and get to the main menu. This will create a save file compatible with your current Elden Ring version.

   
To install each of your mods (files 1d), follow the steps as follows:

<details markdown="block">
  <summary>My mod contains many files and folders</summary>

> 1. Enter your `ModEngine2` folder.  
> 2. Enter the `mod` folder.  
> 3. Extract your mod to this folder, as shown:  
> <a href="https://i.imgur.com/uLvLBsJ.png"><img src="https://i.imgur.com/uLvLBsJ.png" width="600"></a>
> 
> <b><u>IMPORTANT NOTE</u></b>: When using multiple mods, they may overwrite each other when modifying the same files. Therefore, the install order is significant when combining mods.  
> 
> <b><u>NOTE</u></b>: If your mod contains modified assets (such as textures and models), they will be typically only be loaded for yourself. To show those assets on other players, copy the file and append _l to the end of it. For example:
> ```
> Local player file:   hd_m_1500.partsbnd.dcx
> Remote players file: hd_m_1500_l.partsbnd.dcx
> ```
</details>
<details markdown="block">
  <summary>My mod contains a DLL file!</summary>

> 1. Enter your `mods` folder.  
> 2. Extract your mod to this folder, as shown:  
> <a href="https://i.imgur.com/bT6X7Fd.png"><img src="https://i.imgur.com/bT6X7Fd.png" width="600"></a>
> 
> **__NOTE__**: If the mod's filename is `dinput8.dll`, it is recommended you rename it to `<modname>.dll`.
</details>
<details markdown="block">
  <summary>My mod contains a launcher!</summary>

> Mod launchers usually wrap around either ModEngine 2 or a dll injector.
> 
> Since you will not be using the original launcher, pay no attention to it - and instead look at the other files that come with your mod - and choose one of the previous methods.
> 
> <u>Example 1</u>: Elden Ring Ascended comes pre-packed with ModEngine 2. It's best to take the contents of the `mod` folder of it, and install it as shown in "⁠My mod contains many files and folders"  
> <u>Example 2</u>: Elden Ring FPS comes with a dll injector launcher. For it, you will have to take the contents of `Elden_Ring_FPS` and install it as shown in "My mod contains a DLL file!⁠"
</details>
<details markdown="block">
  <summary>My mod only contains a regulation.bin!</summary>

> A `regulation.bin` file can be installed in the same method as other Mod Engine 2 mods, see "⁠My mod contains many files and folders"
</details>

After the installation of all of your mods, run `launchmod_eldenring.bat` - or the desktop shortcut to it, to run modded Elden Ring.  
<b><u>NOTE</u></b>: It may need to be run as administrator.

OR

To combine all of the above with a randomizer:
<details markdown="block">
  <summary>My mod is a randomizer!</summary>

> 1. Go to your `Game` folder.
> 2. Extract the `randomizer` folder to it:  
> <a href="https://i.imgur.com/CVmA6Vo.png"><img src="https://i.imgur.com/CVmA6Vo.png" width="600"></a>
> 3. Enter the `randomizer` folder and run `EldenRingRandomizer.exe`:  
> <a href="https://i.imgur.com/dEmyw9i.png"><img src="https://i.imgur.com/dEmyw9i.png" width="600"></a>
> 4. Apply your randomizer settings:  
> <a href="https://i.imgur.com/I9loKWD.png"><img src="https://i.imgur.com/I9loKWD.png" width="600"></a>
> 5. Supply your Mod Engine's mod folder path:  
> <a href="https://i.imgur.com/eBfU1Bc.png"><img src="https://i.imgur.com/eBfU1Bc.png" width="600"></a>
> 6. Click `Randomize items and enemies`.
> 7. Click `Options`, and then click `Save options file`:  
> <a href="https://i.imgur.com/beH6nmA.png"><img src="https://i.imgur.com/beH6nmA.png" width="600"></a>
> 8. Send the file to your playmates. They will need to load it through `Load options file`, and follow steps 5 and 6.
> 9. Click `Launch Elden Ring` from within the randomizer UI to launch the game.
</details>

## UNINSTALL GUIDE:
Before uninstalling - it is possible to disable Mod Loader. This will allow running of *Vanilla Elden Ring* or *Seamless Coop Standalone* with less effort, and no permanent change to your setup.
To do so, simply go to your `Game` folder, and rename `dinput8.dll` as `_dinput8.dll`. To revert this change and launch your mods, simply rename it back.

To uninstall, delete the following files and directories from your `Game` folder:
```
ModEngine2
mods
SeamlessCoop
dinput8.dll
mod_loader_config.ini
```
If you have installed a randomizer, delete the `randomizer` folder as well. A clean `Game` folder is as shown:  
<a href="https://i.imgur.com/pKkYDa6.png"><img src="https://i.imgur.com/pKkYDa6.png" width="600"></a>
