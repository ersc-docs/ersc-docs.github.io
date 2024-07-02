---
layout: page
title: Troubleshooting
permalink: /troubleshooting/
nav_order: 5
---
# Troubleshooting

## Messages and solutions when trying to use the Seamless Coop items

<details markdown="block">
<summary> Failed, nosession found </summary>

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
<summary> Failed,Steam timed out </summary>

>This is nothing to do with the mod - there is just no connection to Steam. Remember that the steam servers go down for maintenance <b><u>every Tuesday</u></b>. The mod can't fix poor internet connections that may cause this error.
>Steam Server Check: https://steamstat.us/
</details>

<details markdown="block">
<summary> Failed: Search request timed out </summary>

>Steam must be open and connected online.
</details>

## Errors that can occur upon launching Seamless Coop

<details markdown="block">
<summary> <b>"Inappropriate Activity Detected"</b> after game launch </summary>

><u>If it happens during Seamless Coop launch</u> it means that the mod failed to hook into the game after being loaded. This is due to antiviruses false flagging and preventing it from working. Please disable or uninstall them.
>
><u>If it happens during vanilla launch</u> it means that you have disabled EAC by using other mods/bypasses, such as Mod Engine 2 and Mod Loader. The most common hook is Mod Loader, which is done through dinput8.dll - renaming or moving it to another folder will let you run vanilla Elden Ring.
>
><u>If this happens when launchg the game through Mod Engine 2.1's launchmod_eldenring.bat</u> It means you have not followed the instructions in [Seamless Modding](https://ersc-docs.github.io/seamless-modding/) to use seamless coop with other mods.
>
>NOTE: Seamless Coop, by itself, can run in parallel to vanilla playthroughs without any file renaming.
>The moment a dll hook without a launcher is add, switching between vanilla and modded playthroughs becomes more complicated. Consult ⁠[Seamless Modding](https://ersc-docs.github.io/seamless-modding/) for more info.
</details>
