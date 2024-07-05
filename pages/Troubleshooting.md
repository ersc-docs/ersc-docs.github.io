---
layout: page
title: Troubleshooting
permalink: /troubleshooting/
nav_order: 5
---
# Troubleshooting

## Messages,issues and solutions when using the Seamless Coop items

<details markdown="block">
<summary> Failed, no session found </summary>

>To connect, one player must use the Tiny Great Pot. After that, all other players must use the Effigy of Malenia.
>
>Proceed with the following debugging steps:
>1. Purchase the game on Steam. Piracy is not supported and won't ever be. The mod will not work unless everyone has a unique copy.
>
>2. Make sure everyone playing has the same Elden Ring version. Version can be seen at the title screen, bottom right.
>
>3. Make sure everyone is running the same Seamless Coop version.
>
>4. If anyone uses other mods, you need to double check that the correct launcher is being used. It's possible one person did not launch the correct version of the game to play with others.
><b><u>NOTE:Make</u></b> sure everyone is using the same regulation.bin file mods.
>
><b><u>IMPORTANT NOTE:</u></b> Both of these versions are listed in the start menu. You can share pics to verify you match.
>
>5. Make sure everyone has set the same password in the seamlesscoopsettings.ini. You must save the file and restart the game entirely for the new password to be registered.
>
>6. Everyone must be connected to Steam's Friends network.
>
>7. Verify game files in steam. It should verify rougly 450-600 files else try again.
>
> <b><u>NOTE:</u></b> During Steam maintenance, connectivity will go offline. This usually doesn't last more than a few minutes.
>
>8. Do not block any players  on Steam in your group.
>
>9. If all the above checks out, test out your connection in vanilla Elden Ring. If that works, Seamless Coop has been blocked by your firewall or antivirus.
>
><b>EXTRA: If you trust other people in the session and don't mind them knowing your IP address</b>, you can improve the connection quality by sharing your IP directly.
><b>In Steam, Steam => Settings => In-Game => Steam Networking and set it to "Always".</b>
</details>

<details markdown="block">
<summary> Failed, Steam timed out </summary>

>This is nothing to do with the mod - there is just no connection to Steam. Remember that the steam servers go down for maintenance <b><u>every Tuesday</u></b>. The mod can't fix poor internet connections that may cause this error.
>Steam Server Check: https://steamstat.us/
</details>

<details markdown="block">
<summary> Failed: Search request timed out </summary>

>Steam must be open and connected online.
</details>

<details markdown="block">
<summary> Cooperator was (Unable to join session) </summary>

>You are able to find the session but something is blocking/hindering you from joining the session. 
>
>1. Make sure no one has blocked anyone in the session on Steam.
>
>2. Make sure neither Steam or Elden Ring is blocked by your firewall/s or antivirus.
>
>3. Try without/with VPN enabled
>
>4. Try restarting your router.
>
>5. If you have installed Riot's Vanguard installed try turning it off. If you have any other games anti cheat that is known to be intrusive torn them off as well.
</details>

<details markdown="block">
<summary> You must own Shadow of the Erdtree to join this session. </summary>

>This means you must own the DLC and have it installed to join this session, because the host is in the DLC area.
>
>If you are trying to join someone not in the DLC area your password is most likely in use by other people.
>Change your password into something better and try again.
</details>

## General connection issues

<details markdown="block">
<summary> General Connection issues </summary>

>1. Try restarting your routers and PCs
>2. Try using ethernet instead of WiFi
>3. Try turning your VPN off/on
>4. As a last resort try another network entirely and make sure your internet provider is not having any disturbances.
>
><b><u>NOTE:</u></b> In Steam go to Steam -> Settings -> In-Game -> Steam Networking -> Chose Friends only (If you are steam friends) or Always. <b><u>This will share your IP address with people you connect with.</u></b>
</details>

<details markdown="block">
<summary> Desynced/Invisible enemies </summary>

>Rest at a grace.
>
>Do the Steps above in "<b>General Connection Issues</b>".
</details>

## Errors and Crashes

<details markdown="block">
<summary> <b>"Inappropriate Activity Detected"</b> after game launch </summary>

><u>If it happens during Seamless Coop launch</u>.
> It means that the mod failed to hook into the game after being loaded. This is due to antiviruses false flagging and preventing it from working. Please disable or uninstall them.
>
><u>If it happens during vanilla launch</u>.
> It means that you have disabled EAC by using other mods/bypasses, such as Mod Engine 2 and Mod Loader. The most common hook is Mod Loader, which is done through dinput8.dll - renaming or moving it to another folder will let you run vanilla Elden Ring.
>
><u>If this happens when launchg the game through Mod Engine 2.1's launchmod_eldenring.bat</u>.
>It means you have not followed the instructions in [Seamless Modding](https://ersc-docs.github.io/seamless-modding/) to use seamless coop with other mods.
>
><u>If it happens when launching the game throgh the <b>Randomizer</b>.</u>
>It means your version of Seamless Coop is no longer up to date, make sure you have the latest version of Seamless Coop installed in your <b>mods</b> folder. You can find the latest version of Seamless Coop here: [Seamless Coop](https://www.nexusmods.com/eldenring/mods/510/?tab=files).
>
><b>NOTE:</b> Seamless Coop, by itself, can run in parallel to vanilla playthroughs without any file renaming.
>The moment a dll hook without a launcher is add, switching between vanilla and modded playthroughs becomes more complicated. Consult ⁠[Seamless Modding](https://ersc-docs.github.io/seamless-modding/) for more info.
</details>

<details markdown="block">
<summary> Failed to launch Elden Ring.exe error 740 </summary>

>Run <b>ersc_launcher.exe</b> as admin
</details>

<details markdown="block">
<summary> Failed to find "SeamlessCoop//ersc.dll" </summary>

>Use the latest launcher bundled with the game.
>
>White list the game folder in your antivirus. If you are using anything other than Windows Defender as an antivirus try disabling it. 
>
>Make sure ersc.dll  is present within the SeamlesCoop folder. Right click it and click on Properties. Press Unblock, if that option is visible.
>
>Make sure you've correctly installed the mod by following ⁠⁠⁠[How to install](https://ersc-docs.github.io/how-to-install/).
</details>

<details markdown="block">
<summary> I am getting crashes </summary>
>Most likely, not a Seamless Coop bug.
>Due to how Elden Ring applies its updates, it will often result in corrupted files.
>Please verify files through Steam first.
>
>The current version of raytracing in Elden Ring isn't very stable.
>Please turn it off in the ingame settings before submitting a report.
>
>Some software hooks into Elden Ring, which interferes with Seamless Coop's hooks and can cause a white screen hang, or crashes.
>
>As a rule of thumb, these are usually overlays and tuners.
>These are including, but not limited to:
>AMD Ryzen Master
>AMD Adrenaline
>Rivia Tuner
>MSI Afterburner
>Medal
>Overwolf
>Process Lasso
>System Explorer
>And might also include Discord and GeForce overlays.
>Run <b>ersc_launcher.exe</b> as admin
</details>

<details markdown="block">
<summary> This version of seamless co-op(1.7.x) is depreciated and requires an update.  </summary>

>It means this version is no longer supported and a new version is avaliable.
>
>You can download the latest version of Seamless Coop from it's nexus mods page here. [Seamless Coop](https://www.nexusmods.com/eldenring/mods/510/?tab=files)
>and follow the instalation steps in [How to install](https://ersc-docs.github.io/how-to-install/) to update to the new version.
</details>

<details markdown="block">
<summary> Game closes on launch with no messages.  </summary>

>Start by making sure steam is open in online mode.
>
>Try verifying game files in steam. Should verify rougly 450-600 files.
>
>Redownload the mod again to make sure nothing went wrong with the download. You can down load it from the [Nexus page](https://www.nexusmods.com/eldenring/mods/510/?tab=files).
>Install it like suggested in [How to install](https://ersc-docs.github.io/how-to-install/)  
</details>


