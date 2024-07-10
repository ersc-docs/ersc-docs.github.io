---
layout: page
title: A Seamless Modding Rewrite
permalink: /ASMR/
nav_order: 6
---



# Using Seamless Coop with other mods.

## INSTALLATION GUIDE:  
This guide will go over using Seamless Coop in conjunction with other mods.<br /> 
If you want Seamless coop with no other mods follow [How to install](https://ersc-docs.github.io/how-to-install-and-update/) instead.<br />
For optimal experience, all players should use the same mods together - with the exception for visual mods, which can remain personal.

 <u><b>IMPORTANT NOTE</b></u>: Mods have to be compatible with the version of Elden Ring you're using. <br />
 Typically only the latest version of Elden Ring is supported, and if the mod has been abandoned you will not be able to use it.<br />  
 <u><b>IMPORTANT NOTE</b></u>: All players must use the same mods in order to connect to each other.

<details markdown="block">
  <summary>Windows</summary>


  <b><u>NOTE</u></b>: This guide was written with file extensions **ENABLED**.<br /> 
  If some file names do not match what you're seeing, please turn this setting on in File Explorer:<br />  
 <a href="https://i.imgur.com/sBU3kWt.png"><img src="https://i.imgur.com/sBU3kWt.png" width="600"></a>





 A guide on how to setup Seamless Coop with ModEngine 2 + other mods. 
 
 **Required**

 You MUST launch Seamless Coop with either the launcher or ModEngine2.<br /> 
 DLL injectors like Elden Mod Loader and Lazy Loader won't work.


## Files you need
Seamless Coop and ModEngine2.

Make sure that you have:
- [ModEngine2](https://github.com/soulsmods/ModEngine2/releases/latest)
- [Seamless Coop](https://www.nexusmods.com/eldenring/mods/510)

## Setup 


<details markdown="block">
  <summary>1. Where to put the files.</summary>

1.1 Extract `Mod Engine 2` using your prefered file archiver. Like [7zip](https://www.7-zip.org/download.html) as an example.<br />
<br />
    ![image](https://github.com/ersc-docs/ersc-docs.github.io/assets/174225858/ef067a95-3968-4e70-8c7e-5fb42b88802d)
 
1.2 Rename the folder `ModEngine-2.1.0.0-win64` into `ME2`<br />
<br />
    ![image](https://github.com/ersc-docs/ersc-docs.github.io/assets/174225858/5687de17-a960-4d45-b0e7-7251f8cc4107)

1.3 Place the `ME2` folder into your `Game` folder. <br />
<br />
    ![image](https://github.com/ersc-docs/ersc-docs.github.io/assets/174225858/268b828a-51e9-4d8d-bc03-6b5ff8b519ea)



<details markdown="block">
  <summary>Where is my Game folder</summary>

 *Browser local files in steam.*

1. Open Steam
  
2. Right click `Elden Ring`
 
3. Go down to `Manage`
 
4. Click on `Browser local files`
 
    ![image](https://github.com/ersc-docs/ersc-docs.github.io/assets/174225858/4ec7754c-956a-4699-b53f-e458deb91ad1)

This will open your `Elden Ring` folder and inside it is the `Game` Folder. 
 
You can pin the `Game` folder to `Quick acces` <br />
by right clicking the `Game` folder -> `Pin to Quick acces`. <br />
Which will make it available in the left side of the file explorer under Quick acces.
    ![image](https://github.com/ersc-docs/ersc-docs.github.io/assets/174225858/50750f3b-2030-4248-ad9a-a225a44ab415)

</details>

 1.4 Go back to where your `Seamless Co-op v1.x.x.zip` is located and extract it as well.
 
 1.5 Open the `Seamless Co-op v1.x.x` folder and inside you should see a `SeamlessCoop` folder and a `ersc_launcher.exe`
 
 1.6 Place the `SeamlessCoop` folder into the `ME2` folder that is in your `Game` folder.

  ![image](https://github.com/ersc-docs/ersc-docs.github.io/assets/174225858/e79276d1-956b-499d-8ea5-2296a8c663cf)

 1.7 You can now delete the files unrelated to `Elden Ring` from the `ME2` Folder. <br />
 They are `config_armoredcore6.toml`, `config_darksouls3.toml`, `launchmod_darksouls3.bat` and `launchmod_armoredcore6.bat`

 ![image](https://github.com/ersc-docs/ersc-docs.github.io/assets/174225858/ae2278af-4cce-4ee7-ad0c-8425a0a34774)

</details>

<details markdown="block">
<summary>2. Set a Password and configure the ersc_settings.ini</summary>

 2.1 Open your `SeamlessCoop` folder in your `ME2` folder. 
 
 2.2 Open the `ersc_settings.ini` file with text editor of choise.
 
 2.3 Change the settings to your/your groups liking and set a password.

```
[GAMEPLAY]

; Invaders are other players that will join your world uninvited and try to kill you and your party.  0=FALSE  1=TRUE
allow_invaders = 1

; Debuffs (Rot Essence) will be acquired when you die, and will only be cured when you sit at a bonfire.  0=FALSE  1=TRUE
death_debuffs = 1

; Spirit summons can aid you in multiplayer.  0=FALSE  1=TRUE
allow_summons = 1

; 0 = Normal | 1 = None | 2 = Display player ping | 3 = Display player soul level | 4 = Display player death count
overhead_player_display = 0


[SCALING]

; Amount of enemy health (%) per player for each enemy. (Default: 35 = 35% more enemy health per player)
enemy_health_scaling = 35

; Amount of enemy damage (%) per player for each enemy. (Default: 0 = 0% more enemy damage per player)
enemy_damage_scaling = 0

; Amount of enemy posture absorption (%) per player for each enemy. (Default: 15 = 15% more per player)
enemy_posture_scaling = 15

; Amount of boss health (%) per player for bosses. (Default: 100 = 100% more boss health per player)
boss_health_scaling = 100

; Amount of enemy damage (%) per player for bosses. (Default: 0 = 0% more enemy damage towards players, per player)
boss_damage_scaling = 0

; Amount of boss posture absorption (%) per player for bosses. (Default: 20 = 20% more boss posture per player)
boss_posture_scaling = 20

[PASSWORD]

; Session password
cooppassword = I Made A Password

[SAVE]

;Your save file extension (in the vanilla game this is .sl2). Use any alphanumeric characters (limit = 120)
save_file_extension = co2

[LANGUAGE]

;Leave this blank unless you want to load a custom locale file. The mod will default to your game language.
mod_language_override = 
```

 2.4 When you are done `Save` the changes.
 
 <b>Note:</b> Host's `ersc_settings.ini` determins the worlds `Scaling`, `Player Invasions`, `Rot` and `Spirit Summons`.
 
 <b>Note2:</b> You need to set the password in this location, When you are using `Mod Engine 2` to launch the game.
 
 <b>Optional</b> You can change the save file extension you use for a save depending on what mods you use.

```
[SAVE]

;Your save file extension (in the vanilla game this is .sl2). Use any alphanumeric characters (limit = 120)
save_file_extension = `co2`
```

 Change where it says `co2` into as an example `Moddedco2`,<br /> 
 then make a copy of your `ER0000.co2` file and rename the copy into `ER0000.Moddedco2`.<br /> 
 This will separate Seamless Coop only saves and saves using other mods.<br />
 So you dont accidently open them up and lose a lot of modded items on those characters.

</details>

<details markdown="block">
  <summary>3. Setting up Mod Engine 2</summary>

 3.1 Open your `ME2` folder. 
 
 3.2 Open the `config_eldenring.toml` with your prefered text editor.
 
 3.3 Copy and paste `external_dlls = [ "SeamlessCoop/ersc.dll" ]` into your `config_eldenring.toml` in the location shown below. 

    ```
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
    external_dlls = [ "SeamlessCoop/ersc.dll" ]

    # Mod loader configuration
    [extension.mod_loader]
    enabled = true

    # Not currently supported for Elden Ring
    loose_params = false

    # List of directories that contain modded files in order of prioritization. Inside each specified mod directory must have the game
    # assets in Fromsoft's asset structure. I.e. if you mod parts/something.partsbnd.dcx, the modded version must be at mod/parts/something.partsbnd.dcx.
    # Absolute paths to mods are supported but must use '\\' to separate path items. For example, if your mod is at E:\coolstuff\coolmod, you must enter
    # the path in the config as "E:\\coolstuff\\coolmod".
    # If there's no drive specifier (C:, D:, etc), the path is relative to where the launcher is located. For example, having the path as "mod" will tell
    # modengine 2 to look for the directory mod inside the mod engine 2 directory with the launcher.
    #
    # Multiple mods must be separated with commas. For example if you have 3 mods, you will have something like the following:
    # mods = [
    #    { enabled = true, name = "coolmod", path = "mod1" },
    #    { enabled = true, name = "nicemod", path = "mod2" },
    #    { enabled = true, name = "sosomod", path = "mod3" }
    # ]
    # Note that modengine 2 currently has no way to resolve conflicting files including regulation.bin, and thus the mod with the highest priority
    # will have the modded file be loaded in the case of conflict. Some support for merging of params and potentially other assets is considered for
    # a future release.
    mods = [
    { enabled = true, name = "default", path = "mod"}

    ]

    # When enabled, scylly hide will be injected into the game. This allows for antidebug measures in the game to be bypassed so that you can attach
    # debuggers such as Cheat Engine, x64dbg, windbg, etc to the game without as much trouble. If you're not reverse engineering the game, this option
    # is probably not for you.
    [extension.scylla_hide]
    enabled = false
    ```

3.4 Save the changes.

</details>


<details markdown="block">
<summary>4. Adding aditional mods.</summary>

<b><u> MAKE SURE TO READ THE DESCRIPTION AND/OR READ ME OF MODS YOU WANT TO USE </u></b> 

<details markdown="block">
<summary>What is the difference between what's refered to as file based mods and .dll mods?</summary>

`File based` mods are mods that would have to replace game file to function,<br />
 which we get around by using `Mod Engein 2` to launch the game.<br /> 
 This means that if you are using 2 mods that are file based<br />
 they may replace eachothers files which can and most likely will cause issues.
 
 
`.dll` mods are mods that need to be injected into the game to function and would not replace game files.

</details>

<details markdown="block">
  <summary>How do I know if it's a file based mod or a .dll mod?</summary>

 `File based` mods are usually overhauls like <br />
 Clever's moveset packs, Convergence and Elden Ring Reforged<br />
 or something like a armor replacer but can also be simple edits to the `regulation.bin`.<br /> 
   Big overhauls will sometimes come bundled with `.dll` mods and `Mod Engine 2`.
 
 `.dll` mods will generally speaking only have a .dll file, a config file aka a .ini file.<br />
 The .ini file may be in a folder sometimes. The can also come with it's own .exe file like Seamless Coop.
 
 You can `preview` what files a mod has on NexusMods before downloading<br />
 by going to the mods `file` page and click on `Preview file contents`. 

</details>

<details markdown="block">
  <summary>My mod is a file based mod.</summary>

<b>Will be using Clever's moveset modpack to demonstrate since it comes with no additional `.dll` mods or `Mod Engine 2`</b>
 
1. Open the zip file you have downloaded with prefered file archiver,<br /> 
   by selecting open archive or double clicking.

    ![image](https://github.com/ersc-docs/ersc-docs.github.io/assets/174225858/b9ffedb1-c36f-4c47-b934-2f62d007c7df)
 
2. Open your file exploerer and go to the `ME2` folder in your `Game` folder.
 
3. Open the `mod` folder. Which should at this point be empty.
 
4. Drag and drop the files from the mod into the `mod` folder.
 
    ![image](https://github.com/ersc-docs/ersc-docs.github.io/assets/174225858/61b427ec-560a-49de-8657-3357f20cebe9)
 
5. The mod is now installed.
 
<b><u>NOTE:</u></b> You can only have one `regulation.bin` mod at a time.<br /> 
Aka mods that come with a `regulation.bin` file.
 
<b><u>NOTE2:</u></b> Only you will see the texture and modle modifications you are using.<br /> 
  If you are using `parts` mods like armor and weapon mods<br />
  and you want it to be shown on the other players in your session when they wear this equipment.<br />
  Make sure that the `parts` files in your `parts` folder<br />
  come with a regular version and a `_l` version. (`l` is a lowercase `L`)

   ![image](https://github.com/ersc-docs/ersc-docs.github.io/assets/174225858/d436a59f-031e-46fa-b923-cb6067f729c9)
 
If they do not then make a copy and rename it.
 
Example:
`wp_a_0120.partsbnd.dcx`'s copy would be renamed into `wp_a_0120_l.partsbnd.dcx`

</details>

<details markdown="block">
<summary>My mod is a .dll mod.</summary>

You can use `Mod Engine 2` or `Elden Ring Mod Loader` for `.ddl` mods.

Some `.dll` mods needs to be last in `Mod Engine 2` for them to work. Some will only work with `Elden Ring Mod Loader`.

<b>If the `.dll` mod you are using is giving a Error saying "Could not find signature!"<br />
try loading it last in `Mod Engine 2` or try using `Elden Ring Mod Loader` and making a load order in .<br />
It could also mean that the mod is outdated</b>

<details markdown="block">
<summary>Using `Mod Engine 2`</summary>

1. Download what ever .dll mod you want to use. I.ll be using the Posture bar mod as an example.

2. Open the downloaded zip and navigate to where you see it's `.dll` file. 
 
    ![image](https://github.com/ersc-docs/ersc-docs.github.io/assets/174225858/1acd630c-6d23-4843-81e6-34630f528264)
 
3. Go to your `ME2` folder in your `Game` folder.

4. Make a new folder and name it into `dllMods`.<br /> 
  (You can name the folder to whatever you want,<br />
   if you do replace `ddMods` with what ever you named the folder into)

    ![image](https://github.com/ersc-docs/ersc-docs.github.io/assets/174225858/30b9991b-4d33-4797-a276-ac54d079468b)

6. Drag and drop the `.dll` mods content into the `dllMods` folder.

    ![image](https://github.com/ersc-docs/ersc-docs.github.io/assets/174225858/10820f1a-17bc-4b19-8b0a-5bbae3132854)

7. Go back into your `ME2` folder and open the `config_eldenring.toml`

8. Add the `.dll` mods `.dll` file into the config where you added Seamless Coop in a previous step.<br /> 
   Separate the `.dll` mods you are using with a `,`.

  ```
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
  external_dlls = ["SeamlessCoop/ersc.dll", "dllMods/PostureBarMod.dll"]
  
  # Mod loader configuration
  [extension.mod_loader]
  enabled = true
  
  # Not currently supported for Elden Ring
  loose_params = false
  
  # List of directories that contain modded files in order of prioritization. Inside each specified mod directory must have the game
  # assets in Fromsoft's asset structure. I.e. if you mod parts/something.partsbnd.dcx, the modded version must be at mod/parts/something.partsbnd.dcx.
  # Absolute paths to mods are supported but must use '\\' to separate path items. For example, if your mod is at E:\coolstuff\coolmod, you must enter
  # the path in the config as "E:\\coolstuff\\coolmod".
  # If there's no drive specifier (C:, D:, etc), the path is relative to where the launcher is located. For example, having the path as "mod" will tell
  # Mod Engine 2 to look for the directory mod inside the Mod Engine 2 directory with the launcher.
  #
  # Multiple mods must be separated with commas. For example if you have 3 mods, you will have something like the following:
  # mods = [
  #    { enabled = true, name = "coolmod", path = "mod1" },
  #    { enabled = true, name = "nicemod", path = "mod2" },
  #    { enabled = true, name = "sosomod", path = "mod3" }
  # ]
  # Note that modengine 2 currently has no way to resolve conflicting files including regulation.bin, and thus the mod with the highest priority
  # will have the modded file be loaded in the case of conflict. Some support for merging of params and potentially other assets is considered for
  # a future release.
  mods = [
      { enabled = true, name = "default", path = "mod" }
  ]
  
  # When enabled, scylla hide will be injected into the game. This allows for antidebug measures in the game to be bypassed so that you can attach
  # debuggers such as Cheat Engine, x64dbg, windbg, etc to the game without as much trouble. If you're not reverse engineering the game, this option
  # is probably not for you.
  [extension.scylla_hide]
  enabled = false
  ```

8. do the same for all `.dll` mods you want to use.

9. Save the changes when you are done.

</details>

<details markdown="block">
<summary>Using Mod Loader</summary>

Some `.dll` mods may require `Elden Ring Mod Loader` to load properly.

<b>THIS WILL MAKE YOU UNABLE TO LAUNCH VANILLA ELDEN RING IN OFFLINE MODE.\ 
UNLESS YOU RENAME `dinput8.dll` INTO `_dinput8.dll`.</b>

1. Download [Elden Ring Mod Loader](https://www.nexusmods.com/eldenring/mods/117)

2. Open the zip file you downloaded and drag and drop it's content into the `Game` folder. 

    ![image](https://github.com/ersc-docs/ersc-docs.github.io/assets/174225858/64a510d5-4695-4946-9dd9-74cb0a77dec5)

3. Download whatever `.dll` mod you want to use. I.ll be using the Posture bar mod as an example.

4. Open the zip and navigate to where you can see the `.dll` file.\  
   Then drag and drop it's content into the `mods` folder located in your `Game` folder.

    ![image](https://github.com/ersc-docs/ersc-docs.github.io/assets/174225858/fe2bf108-3377-4337-b4e1-a77a108b5cdd)

5. Go back into your `Game` folder

6. Open `Elden Ring Mod Loader`'s `mod_loader_config.ini` file.

7. Add the mods you have installed to your load order. Lowest number has highest load priority.<br />
   Increase the load delay if some `.dll` mods fail to load properly.


    ```
    [modloader]
    load_delay = 5000
    show_terminal = 0

    [loadorder]
    PostureBarMod.dll.dll = 1
    ```

8. Save the changes when you are done.

</details>

</details>

<details markdown="block">
<summary>I want to use a randomizer</summary>

1. Download [Elden Ring Item Randomizer]()

2. Open the zip file you downloaded with your prefered file archiver.

3. Drag and drop the `randomizer` folder into your `ME2` folder located in your `Game` folder.

    ![image](https://github.com/ersc-docs/ersc-docs.github.io/assets/174225858/6744e648-8425-4d3d-ba37-c5e0b81cf256)

4. Open the `randomizer` folder and run the `EldenRingRandomizer.exe`.

    ![image](https://github.com/ersc-docs/ersc-docs.github.io/assets/174225858/1077db6e-6c5f-4bea-80fd-fb15e4aa9853)

5. In the Randomizer window click on `Select game exe`

    ![image](https://github.com/ersc-docs/ersc-docs.github.io/assets/174225858/79ee827b-822c-4b02-997a-bdbdc5fb3763)

6. Navigate to your `Game` folder, select the `eldenring.exe` and press `Open`.

    ![image](https://github.com/ersc-docs/ersc-docs.github.io/assets/174225858/d2dac3bb-f90d-411b-b087-a7e3af1e65f4)

7. Change the settings to your likeing in the `Item Randomizer`, `Enemy Randomizer` and `Misc Options` tabs. 

8. If you want to use the Randomizer with other `file based` mods you can click on `Merge other mod`.

    <b>NOTE:</b> Trying to use Randomizers merge option with mods that make map edits can cause the randmizer to fail to randomize and spit out an error.

9. In the pop up select the option that suites your needs but easiest is to just click `Select mod directory to merge`.

    ![image](https://github.com/ersc-docs/ersc-docs.github.io/assets/174225858/405aee65-af84-4bad-8aa4-6b795b0497b6)
   
11. Navigate to the `ME2` folder and click on the `mod` folder and then click on `Select Folder`.

    ![image](https://github.com/ersc-docs/ersc-docs.github.io/assets/174225858/7f5186e7-d4d5-40e5-8914-cb4a3b419916)

12. When you feel happy with your options click `Randomize items and enemies` and wait for the randomizer to finish.<br /> 
    If you uncheck a tab the `Randomize` button will reflect this.


13. Uppon a succesful Randomization the Randomizer will say Done in green at the bottom.

    ![image](https://github.com/ersc-docs/ersc-docs.github.io/assets/174225858/7a68777a-b287-4f38-8f7e-e7bca17210ec)


14. Close the Randomizer window and go back into your `ME2` folder and open the `config_eldenring.toml`.

15. At the botton find the line `{ enabled = true, name = "default", path = "mod" }`

16. Add a `,` to the end of this line like so `{ enabled = true, name = "default", path = "mod" },`

17. Copy the line and paste it in the line below and change where it says `"mod"` into `"randomizer"`

It should look like this.

    ```
    # Note that modengine 2 currently has no way to resolve conflicting files including regulation.bin, and thus the mod with the highest priority
    # will have the modded file be loaded in the case of conflict. Some support for merging of params and potentially other assets is considered for
    # a future release.
    mods = [
       { enabled = true, name = "default", path = "mod" },
       { enabled = true, name = "default", path = "randomizer" },
    ]

    # When enabled, scylla hide will be injected into the game. This allows for antidebug measures in the game to be bypassed so that you can attach
    # debuggers such as Cheat Engine, x64dbg, windbg, etc to the game without as much trouble. If you're not reverse engineering the game, this option
    # is probably not for you.
    [extension.scylla_hide]
    enabled = false
    ```

<b><u>Save the changes</u></b>


<b>NOTE:</b> If you do not want to use the randomizer anymore or just disable it for the moment.<br />
You can add a `#` to the beginig of the line and `Mod Engine 2` will skip launching it.    
    ![image](https://github.com/ersc-docs/ersc-docs.github.io/assets/174225858/f2920cb1-7f18-4b69-9d75-e5bd37b73770)




</details>

</details>

<details markdown="block">
<summary>5. Launching the game</summary>

5.1 Open your `ME2` folder located in your `Game` folder.

5.2 Launch the game with the `launchmod_eldenring.bat`
    ![image](https://github.com/ersc-docs/ersc-docs.github.io/assets/174225858/9bd45726-c29e-478a-9e8e-b77dc64e62dd)

</details>




</details>


