---
layout: page
title: Seamless Modding (using only ModEngine2)
permalink: /seamless-modding-me2/
nav_order: 5
---
# Seamless Modding (using only ModEngine2)

A guide on how to setup ModEngine 2 with Seamless Coop

> **Required**
>
> You MUST launch Seamless Coop with either the launcher or ModEngine2. DLL injectors like Elden Mod Loader and Lazy Loader
> won't work.
> 


## Files you need
Seamless Coop and ModEngine2.

Make sure that you have:
- [ModEngine2](https://github.com/soulsmods/ModEngine2/releases/latest)
- [Seamless Coop](https://www.nexusmods.com/eldenring/mods/510)

## Setup

1. Where to put the files.  

    After downloading both `Seamless Coop` and `ModEngine2`, extract both archives. Open up the `Seamless Co-op v1.x.x-*` folder, 
    and inside should be a folder `SeamlessCoop`. Open that folder and copy all of the files and folders in this folder.

    Next go to where you installed `ModEngine2`. Open up that folder, and open up the `mods` folder that is already in there.
    Paste the copies of the files from `SeamlessCoop` into this folder. Then go back one folder to whatever folder you put 
    `ModEngine2` in.

2. Setup ModEngine2.  

    In the main `ModEngine2` folder, you should see a `config_eldenring.toml`. Open this file, and past this right below your
    `[modengine]` section.

    ```toml
    external_dlls = [ "mod/ersc.dll" ]
    ```

    Your config toml should now start like this:

    ```toml
    # Global mod engine configuration
    [modengine]
    # If set to true the debug console will appear while the game is running
    debug = false
    
    # List of files that will be loaded into the game as DLL mods.
    # Absolute paths to mods are supported but must use '\\' to separate path items. For example, if your mod is at E:\coolstuff\coolmod.dll, you must enter
    # the path in the config as "E:\\coolstuff\\coolmod.dll".
    # If there's no drive specifier (C:, D:, etc), the path is relative to where the launcher is located. For example, having the path as "mod.dll" will tell
    # Mod Engine 2 to look for the directory mod inside the Mod Engine 2 directory with the launcher.
    #
    # Multiple mods must be separated with commas. For example if you have 3 mods, you will have something like the following:
    # external_dlls = [ "coolmod.dll", "D:\\nicemods\\nicemod.dll", "sosofolder\sosomod.dll" ]
    external_dlls = [ "mod/ersc.dll" ]
    ```

3. Additional mods.  

    You can put file mods into the mod folder, as well, now. You can also put more DLL mods by seperating the paths to them 
    with a comma. Ex:

    ```toml
    external_dlls = [ "mod/ersc.dll", "mod/PostureBarMod.dll" ]
    ```

    You can also put the dll mods in whatever folder you want, as long as the path in the toml file is also updated to reflect
    that. You can also put an absolute that to the file. Ex: `G:\Steam\steamapps\common\ELDEN RING\Game\mods\ersc.dll`. Also
    make sure to put the rest of the Seamless Coop files with the `ersc.dll` file. That goes for all mods loaded this way. Make
    sure the files they came with are in the same directory as them.

4. Launching the game  

    Finally, you can launch the game by launching the `launchmod_eldenring.bat` file. This will find the game through steam, 
    and load up your mods!

    Happy Hunting!
