---
layout: page
title: Frequently Asked Questions
permalink: /faq/
nav_order: 2
---
# FAQ

## General use
<details markdown="block">
<summary>Why am I not getting the Seamless Coop items?</summary>

> You need to rest at a grace to obtain the Seamless Coop items.  
> If you didn't get them - please try verifying your game files through Steam and trying again:  
> Right click Elden Ring in Steam => Properties => Installed Files => Verify integrity of game files
</details>

<details markdown="block">
<summary>How can I use my Elden Ring characters in Seamless Coop?</summary>

<details markdown="block">
<summary>I'm using Windows</summary>

<a id="how-can-i-use-my-elden-ring-characters-in-seamless-coop?-windows"></a>
1. Open File Explorer.  
2. Click the address line, and enter: `%appdata%/EldenRing/`  
3. Enter the folder that corresponds to your SteamID. It will have a lot of numbers.  
4. Copy `ER0000.sl2`, and paste it.  
5. Rename the pasted file `ER0000.co2`  
6. Your vanilla characters will now show in Seamless Coop!
</details>

<details markdown="block">
<summary>I'm using Linux</summary>

<a id="how-can-i-use-my-elden-ring-characters-in-seamless-coop?-linux"></a>
1. Start Seamless Coop and get to the main menu.  
2. Exit the game.  
3. Go to `~/.local/share/Steam/steamapps/compatdata/1245620/pfx/drive_c/`  
4. Copy `ER0000.sl2`  
5. Enter the following command: `cd ~/.local/share/Steam/steamapps/compatdata find | grep ER0000.co2`  
6. Go to the found directory.  
7. `rm ER0000.co2`  
8. Paste the file from step 4.  
9. `mv ER0000.sl2 ER0000.co2`  
10. Your vanilla characters will now show in Seamless Coop!
</details>

</details>

<details markdown="block">
<summary>Can I do White Mask Varre's Quest in Coop?</summary>

> As of Elden Ring 1.06, an NPC was added to be able to complete this requirement. <b>His invasion sign is in the Writheblood Ruins</b>.
</details>

<details markdown="block">
<summary>Can I get achievements when playing this mod?</summary>

> Yes, you can.  
> List of items that *could* potentially not allow achievements to trigger:
>  - Potential that sometimes Steam will go down during a play session momentarily and prevent achievement unlocks. Missing achievements could be gained with `Steam Achievement Manager` which is a tool used to debug situations like this.
>  - A mismatch in events not triggering the achievement to unlock. This could happen during a play session, where a player's progress can cause skips of certain events to trigger, or an event flag not triggering properly. (Create a manual backup save if you play with another player who could have a different progress).
</details>

<details markdown="block">
<summary>How is progress saved for gameplay and items?</summary>

> **GAMEPLAY PROGRESS:**  
> - Progress is saved based on Host progression. Wanderer's progression will not sync if Host has progressed less than the Wanderers.  
> - A player on NG+, can join a player on NG. This can also be vice-versa.  
> - Any crafting or shop items to purchase from the Twin Maiden Husks in Roundtable Hold are dependent on the <b><u>HOST</u></b> of the world. If a Wanderer owns it in their world, it shouldn't be available in a Host's world if they haven't retrieved it yet when Wanderers join.  
> - If the Host <u><b>does not</b></u> own the crafting kit, or cookbook items, then it will <u><b>not</b></u> be available. Everyone should retrieve these items on their own just in case the Host is changed during gameplay.  
> - Quest progression can be erratic. Best to be solo when doing anything, but make sure to make a backup save before playing. Ending choices could have unknown effects during gameplay too.  
> 
> **ITEM PROGRESS:**  
> - Item pick ups are based on instanced loot, meaning any random drops picked up are different for each player.  
> - Loot that is given on persistent enemy defeat (Bosses and Scarabs for example) is collected by everyone joining the host when within the area limits (when all players are in Weeping Peninsula to get respective drops).  
> - Items like Golden Seed or Sacred Tear must be picked up individually. Wanderer's cannot gain items again if they already received them in their world upon joining Host.  
> - When it comes to bell bearing items, it is based on Host. Only Host should turn in items, restart session, and any who rejoin should see items in the shop. In the event of missing items for any bell bearings, consult [Workarounds](https://ersc-docs.github.io/workarounds/).  
>  
> **!!CAUTION!!**  
> If you are going to attempt playing with others who have different progressions (e.g. different endings, different NPC states), **you should make a backup of your save before joining!.**  
> Event flags toggled in the session may persist, so it's very possible to have mismatched progression and may ruin characters involved. See possible workarounds in [Workarounds](https://ersc-docs.github.io/workarounds/). Keep the same host when possible to reduce chances. This is coop, not an MMO.
</details>

<details markdown="block">
<summary>What happens if the game receives an update? Will the mod break?</summary>

> Get the latest version of the mod, and launch it without using any other mods on top - at least at first. Beware that both Seamless Coop and other mods will take time to update and guarantee compatibility with the latest version.  
> Small changes (like changes to `regulation.bin`) will not break Seamless Coop. However, everyone has to be on the same game and mod version in order to connect to each other.
</details>

<details markdown="block">
<summary>If I update Seamless Coop, what happens to my save?</summary>

> Save files are not affected by updating or reinstalling Seamless Coop, Elden Ring or verifying game files in steam.
</details>

<details markdown="block">
<summary>I want to move to another PC when playing, what do I need to do?</summary>

> Seamless Coop saves will have to be copied manually:

<details markdown="block">
<summary>I'm using Windows</summary>

1. Open File Explorer.  
2. Click the address line, and enter: `%appdata%/EldenRing/`  
3. Enter the folder that corresponds to your SteamID. It will have a lot of numbers.  
4. Copy `ER0000.co2`.  
5. Paste it in your new machine, in the same path.  
</details>

<details markdown="block">
<summary>I'm using Linux</summary>

> On your old PC:  
1. Enter the following command: `cd ~/.local/share/Steam/steamapps/compatdata find | grep ER0000.co2`  
2. Go to the found directory.  
3. Copy `ER0000.co2`  

> On your new PC:  
1. Start Seamless Coop and get to the main menu.  
2. Exit the game.  
3. Enter the following command: `cd ~/.local/share/Steam/steamapps/compatdata find | grep ER0000.co2`  
4. Go to the found directory.  
5. `rm ER0000.co2`  
6. Paste the backed up save file from your old PC.  
</details>

</details>

<details markdown="block">
<summary>Can I play the base game, or with a friend that does not own the DLC?</summary>

> Yes, but you will only be able to play the base game together.  
> Attempts to enter the DLC despite that can result in destroyed characters and infinite loading screens.
</details>

<details markdown="block">
<summary>How many players can be in a session.</summary>

> You can be a total of 6 players in total. Aka host + 5.
</details>


<details markdown="block">
<summary>What are the Seamless Coop item IDs?</summary>

> The usable items in Seamless Coop have the following IDs:  
> 8380001 - Tiny Great Pot (lobby open item)  
> 8380002 - Effigy of Malenia (lobby join item, cooperator)  
> 8380003 - Challenger's Lynchpin (lobby join item, invader)  
> 8380004 - Separation Mist (lobby disconnect item)  
> 8380005 - Judicator's Rulebook (friendly fire modes)  
> 8380006 - Rune Decanter (rune arc shop)  
</details>

## Messages, issues and solutions when using the Seamless Coop items

<details markdown="block">
<summary> Failed, no session found </summary>

> To connect, one player must use the Tiny Great Pot. After that, all other players must use the Effigy of Malenia.  
>
> Proceed with the following debugging steps:  
> 1. Purchase the game on Steam. Piracy is not supported and won't ever be. The mod will not work unless everyone has a unique copy.  
> 2. Make sure everyone playing has the same Elden Ring version. Version can be seen at the title screen, bottom right.  
> 3. Make sure everyone is running the same Seamless Coop version.  
> 4. If anyone uses other mods, you need to double check that the correct launcher is being used. It's possible one person did not launch the correct version of the game to play with others.  
>   <b><u>NOTE:</u></b> Make sure everyone is using the same regulation.bin file mods.  
>   <b><u>IMPORTANT NOTE:</u></b> Both of these versions are listed in the start menu. You can share pics to verify you match.  
> 5. Make sure everyone has set the same password in the seamlesscoopsettings.ini. You must save the file and restart the game entirely for the new password to be registered.  
> 6. Everyone must be connected to Steam's Friends network.  
> 7. If you have installed Riot's Vanguard installed try turning it off. If you have any other games anti cheat that is known to be intrusive turn them off as well.  
> 8. Verify game files in steam.  
> <b><u>NOTE:</u></b> During Steam maintenance, connectivity will go offline. This usually doesn't last more than a few minutes.  
> 8. Do not block any players  on Steam in your group.  
> 9. If all the above checks out, test out your connection in vanilla Elden Ring. If that works, Seamless Coop has been blocked by your firewall or antivirus.  
> <b>EXTRA: If you trust other people in the session and don't mind them knowing your IP address</b>, you can improve the connection quality by sharing your IP directly.  
> <b>In Steam, Steam => Settings => In-Game => Steam Networking and set it to "Always".</b>
</details>

<details markdown="block">
<summary> Failed, Steam timed out </summary>

> This is nothing to do with the mod - there is just no connection to Steam. Remember that the steam servers go down for maintenance <b><u>every Tuesday</u></b>. The mod can't fix poor internet connections that may cause this error.  
> Steam Server Check: https://steamstat.us/
</details>

<details markdown="block">
<summary> Failed: Search request timed out </summary>

> Steam must be open and connected online.
</details>

<details markdown="block">
<summary> Cooperator was (Unable to join session) </summary>

> You are able to find the session but something is blocking/hindering you from joining the session.  
> 1. Make sure no one has blocked anyone in the session on Steam.  
> 2. Make sure neither Steam nor Elden Ring are blocked by your firewall(s) or antivirus.  
> 3. Try without/with VPN enabled  
> 4. Try restarting your router.  
> 5. If you have installed Riot's Vanguard installed, try turning it off. If you have any other games' anti-cheat that is known to be intrusive, turn them off as well.
</details>

<details markdown="block">
<summary> k_ESteamNetworkingAvailability_Failed </summary>

> Something is blocking connection with steam  
> Make sure neither Steam nor Elden Ring are blocked by your firewall(s) or antivirus.  
> 
> If you are using an antivirus other than Windows Defender, that might be your issue.  
>
> - Try making exclusions in your antivirus for your `game` folder and `ersc.dll`  
> - Try restarting your router.  
> - If you have installed Riot's Vanguard installed, try turning it off. If you have any other games' anti-cheat that is known to be intrusive, turn them off as well.
</details>

<details markdown="block">
<summary> You must own Shadow of the Erdtree to join this session. </summary>

> This means you must own the DLC and have it installed to join this session, because the host is in the DLC area.  
> 
> If you are trying to join someone not in the DLC area, your password is most likely in use by other people.  
> Change your password into something better and try again.
</details>

## General connection issues

<details markdown="block">
<summary> General Connection issues </summary>

> 1. Try restarting your routers and PCs  
> 2. Try using ethernet instead of WiFi  
> 3. Try turning your VPN off/on  
> 4. As a last resort try another network entirely and make sure your internet provider is not having any disturbances.  
> <b><u>NOTE:</u></b> In Steam go to Steam -> Settings -> In-Game -> Steam Networking -> Choose Friends only (If you are steam friends) or Always. <b><u>This will share your IP address with people you connect with.</u></b>
</details>

<details markdown="block">
<summary> Desynced/Invisible enemies </summary>

> Rest at a grace.  
> Do the Steps above in "<b>General Connection Issues</b>".
</details>

## Errors and Crashes

<details markdown="block">
<summary> <b>"Inappropriate Activity Detected"</b> after game launch </summary>

> - <u>If it happens during Seamless Coop launch</u>.  
>   It means that the mod failed to hook into the game after being loaded. This is due to antiviruses false flagging and preventing it from working. Please disable or uninstall them.  
> 
> - <u>If it happens during vanilla launch</u>.  
>   It means that you have disabled EAC by using other mods/bypasses, such as Mod Engine 2 and Mod Loader. The most common hook is Mod Loader, which is done through dinput8.dll - renaming or moving it to another folder will let you run vanilla Elden Ring.  
> 
> - <u>If this happens when launch the game through Mod Engine 2.1's launchmod_eldenring.bat</u>.  
>   It means you have not followed the instructions in [Seamless Modding](https://ersc-docs.github.io/seamless-modding/) to use Seamless Coop with other mods.  
> 
> - <u>If it happens when launching the game through the <b>Randomizer</b>.</u>  
>   It means your version of Seamless Coop is no longer up to date, make sure you have the latest version of Seamless Coop installed in your <b>mods</b> folder. You can find the latest version of Seamless Coop here: [Seamless Coop](https://www.nexusmods.com/eldenring/mods/510/?tab=files).  
> 
> <b>NOTE:</b> Seamless Coop, by itself, can run in parallel to vanilla playthroughs without any file renaming.  
> The moment a dll hook without a launcher is added, switching between vanilla and modded playthroughs becomes more complicated. Consult ⁠[Seamless Modding](https://ersc-docs.github.io/seamless-modding/) for more info.
</details>

<details markdown="block">
<summary> Failed to launch Elden Ring.exe error 740 </summary>

> Run <b>ersc_launcher.exe</b> as admin.
</details>

<details markdown="block">
<summary> Failed to find "SeamlessCoop//ersc.dll" </summary>

> Use the latest launcher bundled with the game.  
> 
> White list the game folder in your antivirus. If you are using anything other than Windows Defender as an antivirus try disabling it.   
> 
> Make sure ersc.dll is present within the SeamlesCoop folder. Right click it and click on Properties. Press Unblock, if that option is visible.  
> 
> Make sure you've correctly installed the mod by following ⁠⁠⁠[How to install and update](https://ersc-docs.github.io/how-to-install-and-update/).
</details>

<details markdown="block">
<summary> I am getting crashes </summary>

> Most likely, not a Seamless Coop bug.  
> Due to how Elden Ring applies its updates, it will often result in corrupted files. Please verify files through Steam first.  
> 
> The current version of raytracing in Elden Ring isn't very stable.  
> Please turn it off in the ingame settings before submitting a report.  
> 
> Some software hooks into Elden Ring, which interferes with Seamless Coop's hooks and can cause a white screen hang, or crashes.  
> 
> As a rule of thumb, these are usually overlays and tuners.
> These are including, but not limited to:
> - AMD Ryzen Master
> - AMD Adrenaline
> - Rivia Tuner
> - MSI Afterburner
> - Medal
> - Overwolf
> - Process Lasso
> - System Explorer
> - And might also include Discord and GeForce overlays.
>
> Run <b>ersc_launcher.exe</b> as admin
</details>

<details markdown="block">
<summary> This version of seamless co-op(1.8.x) is depreciated and requires an update.  </summary>

> It means this version is no longer supported and a new version is available.  
> 
> You can download the latest version of Seamless Coop from its [Nexus Mods page](https://www.nexusmods.com/eldenring/mods/510/?tab=files). and follow the instalation steps in [How to install](https://ersc-docs.github.io/how-to-install-and-update/) to update to the new version.
</details>

<details markdown="block">
<summary> Game closes on launch with no messages.  </summary>

> Start by making sure steam is open in online mode.  
>
> Try verifying game files in steam. Should verify rougly 450-600 files.  
>
> Redownload the mod again to make sure nothing went wrong with the download. You can download it from the [Nexus page](https://www.nexusmods.com/eldenring/mods/510/?tab=files).  
> Install it like suggested in [How to Install](https://ersc-docs.github.io/how-to-install-and-update/).
</details>

## Known bugs

<details markdown="block">
<summary>I'm trying to invade/assist an NPC, and it doesn't work!</summary>

> Moreover, specific encounters are currently non-functional:  
> * Needle Knight Leda  
> * Sorceress Sellen/Witch-Hunter Jerren  
> * Millicent
> * Ansbach
> * Volcano Manor 3rd request Vargram. Can't be completed atm. <br /> 
> Refer to [Workarounds](https://ersc-docs.github.io/workarounds/) if you'd like to get them working, while solo.
</details>

<details markdown="block">
<summary>I get a long loading screen when entering an NPC invasion!</summary>

> Known bug, cause unknown - for now, just wait it out (around 30 seconds).
</details>

<details markdown="block">
<summary>I entered an evergaol and now I'm stuck as a spectator!</summary>

> Known bug, for now - don't die in evergaols.  
> Evergaol completion makes your camera stay on the original player. Cause hasn't been narrowed down yet.
</details>

<details markdown="block">
<summary>My friend disconnected in a bossfight, and now I'm stuck as a spectator!</summary>

> Known bug, for now - either win the bossfight or Alt+F4 if that happens.
</details>

<details markdown="block">
<summary>I can't lock on!</summary>

> Reloading the character should fix it.  
> This is due to Torrent sharing the same lock-on list as the player - and when it's despawned, it sometimes messes the entity entry list.
</details>

<details markdown="block">
<summary>The ensnaring chest at Agheel Lake doesn't teleport me to Caelid!</summary>

> Known bug, for now - doesn't work.
</details>

<details markdown="block">
<summary>Shadow enemies don't become regular enemies when exposed to light!</summary>

> Known bug. Currently they only become regular enemies for the host.
</details>

<details markdown="block">
<summary>Coop Items, greyed out use option and can't warp.</summary>

> Known bug. Incorrectly set flags.<br />
> A workaround is in [Workarounds](https://ersc-docs.github.io/workarounds/)
</details>

<details markdown="block">
<summary>The crater to Nokron does not appear after killing Radahn.</summary>

> Known bug. Incorrectly set flags.<br />
> A workaround is in [Workarounds](https://ersc-docs.github.io/workarounds/)
</details>

<details markdown="block">
<summary>Stuck at Ranni's Rise. Invisible wall and can't warp.</summary>

> Known bug. Incorrectly set flags.<br />
> A workaround is in [Workarounds](https://ersc-docs.github.io/workarounds/)
</details>

<details markdown="block">
<summary>Texture Corruption Ingame or missing textures.</summary>

> Not a Seamless Coop bug.<br />
> Verify game files through Steam by right clicking: <br />
> Elden Ring => Properties => Local Files => Verify integrity of game files.<br />
> A full data compare is around 450-600 files.
</details>

<details markdown="block">
<summary>Burning down the Sealing Tree, after Romina - missing interaction prompt in session.</summary>

> Known bug, mist out and do the interaction solo.
</details>

<details markdown="block">
<summary>"Touch Memory" interaction after DLC Radahn fight not showing..</summary>

> Known bug, mist out and do the interaction solo.
</details>

## Invasion bugs

<details markdown="block">
<summary>I get the host's world state! Graces, cookbooks and all!</summary>

> Known bug. For now - use dedicated invasion characters for that purpose.
</details>

<details markdown="block">
<summary>I can pick up items during an invasion!</summary>

> These are your own world items. Not a bug.
</details>

<details markdown="block">
<summary>I get boss drops during an invasion!</summary>

> Known bug. Cause unknown.
</details>
