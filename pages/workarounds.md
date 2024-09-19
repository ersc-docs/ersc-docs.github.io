---
layout: page
title: Workarounds
permalink: /workarounds/
nav_order: 3
---
# Workarounds

<details markdown="block">
<summary>Infinite loading screen</summary>

> This could have multiple causes, but most likely you're stuck at an invalid location.  
> For example, DLC region without owning the correct DLC.
>   
> [The Grand Archives Cheat Table](https://github.com/The-Grand-Archives/Elden-Ring-CT-TGA/) has a script to get out of the loading screen.  
> You can find it at `Scripts -> Seamless Co-op -> Loading screen stuck fix` in the cheat table.<br />
> <b> You have to use CHEAT ENGINE to be able to use the table. </b>
</details>

<details markdown="block">
<summary>Coop items, use option greyed out and can't warp. </summary>


> If you coop items are greyed out and you can't warp to graces.
> <br/>
> 1. Download the debug tool : [Nordgaren's Elden Ring Debug Tool](https://github.com/Nordgaren/Elden-Ring-Debug-Tool/releases/latest) <br/>
> 2. Open the tool when you are loaded in on your character while solo. <br/>
> 3. Go to the grace tab in the tool and warp to a grace in Caelid. Example Outside the plaza. <br/>
> 4. In the debug tool go to the `misc` tab and type in `310`. <br/>
> 5. Press check <br/>
> 6. If the power button turns Green, click disable and quit to main menu. Then press continue from the main menu. 

This should fix this issue for you.
</details>

<details markdown="block">
<summary>The crater to Nokron is not there after killing Radahn. </summary>


> 1. Download the debug tool : [Nordgaren's Elden Ring Debug Tool](https://github.com/Nordgaren/Elden-Ring-Debug-Tool/releases/latest) <br/>
> 2. Open the tool when you are loaded in on your character while solo. <br/>
> 3. Go to the grace tab in the tool and warp to a grace in Caelid. Example Outside the plaza. <br/>
> 4. In the debug tool go to the `misc` tab and type in `310`. <br/>
> 5. Press check <br/>

<details markdown="block">
<summary>If the power button is RED </summary>


> 6. Click enable and quit to main menu.<br />
> 7. Press continue in the main menu. <br />
> 8. Check if you can see the crater marker on the map.<br />
> 9. Follow the steps for `If the power button is GREEN`
</details>

<details markdown="block">
<summary>If the power button is GREEN </summary>


> 6. Click disable and quit to main menu.<br />
> 7. Check if you can see the crater marker on the map.
</details>
<br/>
</details>

<details markdown="block">
<summary>Burnt and Unburnt capital at the same time. </summary>


> 1. Download the debug tool : [Nordgaren's Elden Ring Debug Tool](https://github.com/Nordgaren/Elden-Ring-Debug-Tool/releases/latest) <br/>
> 2. Open the tool when you are loaded in on your character while solo. <br/>
> 3. (recommended)Go to the grace tab in the tool and warp to a grace in Farum Azula.  <br/>
> 4. In the debug tool go to the `misc` tab and type in `9116`. <br/>
> 5. Press check <br/>

<details markdown="block">
<summary>If the power button is GREEN </summary>


> 6. Click Disable and quit to main menu.<br />
> 7. Press continue in the main menu. <br />
> 8. Follow the steps for `If the power button is RED`
</details>

<details markdown="block">
<summary>If the power button is RED </summary>


> 6. Click Enable.<br />
> 7. This should prompt the cutsceen and set all flags correctly.
</details>
<br/>
</details>

<details markdown="block">
<summary>Sealingtree is burnt and Romina is not there. </summary>


> 1. Download the debug tool : [Nordgaren's Elden Ring Debug Tool](https://github.com/Nordgaren/Elden-Ring-Debug-Tool/releases/latest) <br/>
> 2. Open the tool when you are loaded in on your character while solo. <br/>
> 3. Go to the `grace` tab in the tool and warp to `Church of the Bud: Main Entrance`.  <br/>

<details markdown="block">
<summary>I have not fought Romina or burnt the tree </summary>


<b>NOTE:</b> If you see a grace in the middle of the church it means Romina is dead in your world. <br />
> 6. In the `debug tool` go to the `misc` tab and type in `20010196` <br />
> 7. Click check, if it is GREEN click `Disable`. <br />
> 8. In the `debug tool` go to the `misc` tab and type in `330` <br />
> 9. Click check, if it is GREEN click `Disable`. <br />
> 10. Warp to `Church of the Bud: Main Entrance` sit of grace. <br />
< 11. This will set the world state to before the Sealingtree is burnt.
</details>

<details markdown="block">
<summary>I have fought Romina but there is no Sealingtree to burn.</summary>


> 6. In the `debug tool` go to the `misc` tab and type in `20010196` <br />
> 7. Click check, if it is RED click `Enable`. <br />
> 8. Warp to `Church of the Bud: Main Entrance` sit of grace. <br />
> 9. This will warp you to Enir-Ilim. <br /> 
</details>

</details>

<details markdown="block">
<summary>Festival won't start even with prerequisites completed. </summary>


> 1. Download the debug tool : [Nordgaren's Elden Ring Debug Tool](https://github.com/Nordgaren/Elden-Ring-Debug-Tool/releases/latest) <br/>
> 2. Open the tool when you are loaded in on your character while solo or if you are the host. <br/>
> 3. Recommended to have everyone in the session be in the plaza area before you set the flag in the next step. <br/>
> 4. In the debug tool go to the `misc` tab and type in `9411`. <br/>
> 5. Click on Enable. <br/>

</details>


<details markdown="block">
<summary>Stuck at Ranni's rise. Invisible wall and can't warp. </summary>


> [The Grand Archives Cheat Table](https://github.com/The-Grand-Archives/Elden-Ring-CT-TGA/) has a script to get out of Ranni's Rise.  
> You can find it at `Scripts -> Seamless Co-op -> Ranni's tower fix` in the cheat table.<br />
> <b> You have to use CHEAT ENGINE to be able to use the table. </b>

</details>

<details markdown="block">
<summary>Missing reward items from Quests/NPC/Bosses with dialogue </summary>


> Rewards from certain events like quests or NPC's may not drop for all. Event flags sync to the host and may have issues for wanderers present in a session. <br />
> These cases should be done while being solo to progress/obtain anything that may not be while in session.<br />
>
> If you are in dire need of any items missed, use the [debug tool](https://github.com/Nordgaren/Elden-Ring-Debug-Tool/releases/latest), and review the readme file for instructions to use.
</details>

<details markdown="block">
<summary>My Erdtree has the wrong state/is flickering!</summary>

> Typically caused by inherited flags from invasions.
>
> 1. Download the debug tool: [Nordgaren's Elden Ring Debug Tool](https://github.com/Nordgaren/Elden-Ring-Debug-Tool/releases/latest) <br />
> 2. Open the tool when you are loaded in on your character while solo.<br />
> 3. In the debug tool go to the `misc` tab. <br />

<details markdown="block">
<summary>If you are pre-Fire Giant or have not burnt the Erdtree: </summary>

> 1. Type in 300 and click Disable. <br />
> 2. Type in 301 and click Disable.<br />
> 3. Type in 302 and click Disable.<br />
> 4. Warp to a grace.<br />

</details>

<details markdown="block">
<summary>IF you have burnt the tree but not defeated Maliketh: </summary>

> 1. Type in 300 and click Disable.<br />
> 2. Type in 301 and click Disable.<br />
> 3. Type in 302 and click Enable.<br />
> 4. Warp to a grace.<br /> 

</details>

<details markdown="block">
<summary>If you have defeated Maliketh. </summary>

> 1. Type in 300 and click Enable.<br />
> 2. Type in 301 and click Enable.<br />
> 3. Type in 302 and click Disable.<br />
> 4. Warp to a grace.<br /> 

</details>

</details>

<details markdown="block">
<summary>The Forager near the Church of the Crusade can't be healed. </summary>

> Vanilla bug. Cause unknown, but most likely multiplayer-related.
> 
> 1. Download the debug tool: [Nordgaren's Elden Ring Debug Tool](https://github.com/Nordgaren/Elden-Ring-Debug-Tool/releases/latest) <br />
> 2. Open the tool when you are loaded in on your character while solo.<br />
> 3. In the debug tool go to the `misc` tab. <br />
> 4. Type in `4956` and click Disable.<br />
> 5. Quit to main menu, then press continue from main menu. Note that you will still have to heal the Forager yourself. <br />

</details>

<details markdown="block">
<summary>The Ruins of Unte are still blocked even after killing the Furnace Golem. </summary>

> You can climb up the back of the Ruins via a couple pieces of the back wall that jut out. If you don't feel like engaging in horse parkour, the wall can be broken manually.
>
> 1. Download the debug tool: [Nordgaren's Elden Ring Debug Tool](https://github.com/Nordgaren/Elden-Ring-Debug-Tool/releases/latest) <br />
> 2. Open the tool when you are loaded in on your character while solo.<br />
> 3. In the debug tool go to the `misc` tab. <br />
> 4. Type in `-2044506988` and click Enable.<br />
> 5. Quit to main menu, then press continue from main menu. <br />

</details>

<details markdown="block">
<summary>DLC final boss died instantly! </summary>

> Vanilla bug. Cause unknown, but most likely multiplayer-related.
> If you want to earn your keep, the boss can be respawned.
> 
> 1. Download the debug tool: [Nordgaren's Elden Ring Debug Tool](https://github.com/Nordgaren/Elden-Ring-Debug-Tool/releases/latest) <br />
> 2. Open the tool when you are loaded in on your character while solo.<br />
> 3. In the debug tool go to the `misc` tab. <br />
> 4. Type in `20010800` and click Disable.<br />
> 5. Rest at a site of grace.<br />

</details>

