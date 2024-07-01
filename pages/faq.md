---
layout: page
title: Frequently Asked Questions
permalink: /faq/
nav_order: 4
---
# FAQ

## General use
<details markdown="block">
<summary>Why am I not getting the Seamless Coop items?</summary>

>You need to rest at a grace to obtain the Seamless Coop items.    
>If you didn't get them - please try verifying your game files through Steam and trying again:  
>Right click Elden Ring in Steam => Properties => Installed Files => Verify integrity of game files
</details>
<details markdown="block">
<summary>Can I get achievements when playing this mod?</summary>

>Yes, you can.  
>List of items that *could* potentially not allow achievements to trigger:
>  - Potential that sometimes Steam will go down during a play session momentarily and prevent achievement unlocks. Missing achievements could be gained with `Steam Achievement Manager` which is a tool used to debug situations like this.
>  - A mismatch in events not triggering the achievement to unlock. This could happen during a play session, where a player's progress can cause skips of certain events to trigger, or an event flag not triggering properly. (Create a manual backup save if you play with another player who could have a different progress).
</details>

<details markdown="block">
<summary>How is progress saved for gameplay and items?</summary>


> **GAMEPLAY PROGRESS:**
> - Progress is saved based on Host progression. Wanderer's progression will not sync if Host has progressed less than the Wanderers.
>  - A player on NG+, can join a player on NG. This can also be vice-versa.
> - Any crafting or shop items to purchase from the Twin Maiden Husks in Roundtable Hold are dependent on the **__HOST__** of the world. If a Wanderer owns it in their world, it shouldn't be available in a Host's world if they haven't retrieved it yet when Wanderers join. 
 > - If the Host <u>**does not**</u> own the crafting kit, or cookbook items, then it will <u>**not**</u> be available. Everyone should retrieve these items on their own just in case the Host is changed during gameplay.
> - Quest progression can be erratic. Best to be solo when doing anything, but make sure to make a backup save before playing. Ending choices could have unknown effects during gameplay too.  
>  
> **ITEM PROGRESS:**
> - Item pick ups are based on instanced loot, meaning any random drops picked up are diferent for each player. 
> - Loot that is given on persistent enemy defeat (Bosses and Scarabs for example) is collected by everyone joining the host when within the area limits (when all players ar
e in Weeping Penninsula to get respective drops).
> - Items like Golden Seed or Sacred Tear must be picked up individually. Wanderer's cannot gain items again if they already received them in their world upon joining Host.
> - When it comes to bell bearing items, it is based on Host. Only Host should turn in items, restart session, and any who rejoin should see items in the shop. In the event of missing items for any bell bearings, consult [(Discord) Missing reward items from Quests/NPC/Bosses with dialogue](https://discord.com/channels/979042878091329587/1129602576996900864).
>  
> **‼️CAUTION‼️**  
> If you are going to attempt playing with others who have different progressions (e.g. different endings, different NPC states), **you should make a backup of your save before joining!.**  
> Event flags toggled in the session may persist, so it's very possible to have mismatched progression and may ruin characters involved. See possible work arounds in [(Discord) #troubleshooting](https://discord.com/channels/979042878091329587/1097343990480777266). Keep the same host when possible to reduce chances. This is a coop, not an MMO.
</details>

<details markdown="block">
<summary>What happens if the game receives an update? Will the mod break?</summary>

> Refer to [(Discord) Elden Ring received an official update, what to do?](https://discord.com/channels/979042878091329587/1097350937573593160).  
>  
> **Note**:  Major updates like DLC tend to break the mod due to changes done to provide content (changes in regulation.bin file cause seamless to break if something major is adjusted). Hot fixes on the other hand could only be minor changes that won't change much and still allow mods to be compatible, if it's small parameter changes.
</details>

<details markdown="block">
<summary>How can I set the deathcount to be the player banner?</summary>

> In the ini, put 4 as your overhead_palyer_display:  
> `overhead_player_display = 4`

</details>

## Known bugs

<details markdown="block">
<summary>I'm stuck in an infinite loading screen!</summary>

> Download Nordgaren's [Debug Tool](https://cdn.discordapp.com/attachments/979043448491491332/1253885339022524529/Elden_Ring_Debug_Tool_0.8.6.0_Preview.7z?ex=6682aff8&is=66815e78&hm=540d0182d3a91d01ade1917ded13b4f9e1a51c236e3b7b643a16b16de5262a65&)  
> 1. Launch Seamless Coop
> 2. While in the loading screen, launch the Debug Tool as Administrator.
> 3. Check that on the bottom, it says: `Loaded: Yes`
> 4. Go to the Misc tab.
> 5. Enable flags: 105, 115.
> 6. Wait for the infinite loading screen to start again. This time, it should complete.
> 7. Go to the Grace tab.
> 8. Under Manage Graces, type Table of Lost Grace.
> 9. Press the Set button.
</details>

<details markdown="block">
<summary>I'm getting a long blackscreen when I sit at a grace/use an evergaol!</summary>

> Known bug, known cause (waits for all the enemies to properly load for all clients before exiting the blackscreen).
</details>

<details markdown="block">
<summary>I get a long loading screen when entering an NPC invasion!</summary>

> Known bug, cause unknown - for now, just wait it out (around 30 seconds).
</details>

<details markdown="block">
<summary>Whenever my partner mounts Torrent, they're flickering/invisible!</summary>

> Visual bug.  
> Torrent tends to go to (0,0,0) in some areas. Reloading the areas (through warping to the local grace) should fix it.
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
<summary>I'm infinitely falling after fighting Radahn!</summary>

> Known bug - for now, use [The Grand Archives cheat table](https://github.com/The-Grand-Archives/Elden-Ring-CT-TGA/releases/) to warp to a grace.
</details>

<details markdown="block">
<summary>I can't lock on!</summary>

> Reloading the character should fix it.  
> This is due to Torrent sharing the same lock-on list as the player - and when it's despawned, it sometimes messes the entity entry list.
</details>

<details markdown="block">
<summary>Active Graces don't synchronize to far away players!</summary>

> Known bug, due to interacting with graces being limited to loaded chunks. For now, activate graces individually, or play close to each other.
</details>

<details markdown="block">
<summary>I completed an NPC invasion, but it didn't count! I can still see the sign!</summary>

> Known bug, NPC invasions currently only work when in session with other players. Play Seamless **Coop** together.
</details>

<details markdown="block">
<summary>The ensnaring chest at Agheel Lake doesn't teleport me to Caelid!</summary>

> Known bug, for now - doesn't work.
</details>

<details markdown="block">
<summary>I crash while on moving carriages!</summary>

> Known bug, for now - don't do it.
</details>

<details markdown="block">
<summary>Rold's Lift disconnects everyone!</summary>

> Known bug, for now - don't do it, or reconnect after doing it.  
> Happens due to the area movement script having a disconnect event, which will have to be disabled.
</details>

<details markdown="block">
<summary>I cannot enter Evergaols that have Stonesword Keys!</summary>

> Known bug, for now - cannot be done.
</details>

<details markdown="block">
<summary>I cannot complete Ansbach's quest!</summary>

> Known bug, unique NPC invasion. For now, cannot be done in Seamless Coop.
</details>

<details markdown="block">
<summary>Millicent's invasion doesn't complete!</summary>

> Known bug, due to unique invasion completion state.  
> For now, cannot be done in Seamless Coop.
</details>


## Invasion bugs

<details markdown="block">
<summary>I get the host's world state! Graces, cookbooks and all!</summary>

> Known bug. For now - use dedicated invasion characters for that purpose.
</details>

<details markdown="block">
<summary>I can invade mid boss-fight!</summary>

> Known bug.
</details>
