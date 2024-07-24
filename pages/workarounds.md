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
> You can find it at `Scripts -> Seamless Co-op -> Loading screen stuck fix` in the cheat table.
</details>

<details markdown="block">
<summary>Coop items, use option greyed out and can't warp. </summary>

> If you coop items are greyed out and you can't warp to graces.
> <br/>
> 1. Download the debug tool : [Nordgaren's Elden Ring Debug Tool](https://github.com/Nordgaren/Elden-Ring-Debug-Tool/releases/latest) <br/>
> 2. Open the tool when you are loaded in on your character while solo. <br/>
> 3. Go to the grace tab in teh tool and warp to a grace in Caelid. Example Outside the plaza. <br/>
> 4. In the debug tool go to the `misc` tab and type in `310`. <br/>
> 5. Press check <br/>
> 6. If the power button turns Green, click disable and quit to main menu. Then press continue from the main menu. 

This should fix this issue for you.
</details>

<details markdown="block">
<summary>The crater to Nokron is not there after killing Radahn. </summary>

> <br/>
> 1. Download the debug tool : [Nordgaren's Elden Ring Debug Tool](https://github.com/Nordgaren/Elden-Ring-Debug-Tool/releases/latest) <br/>
> 2. Open the tool when you are loaded in on your character while solo. <br/>
> 3. Go to the grace tab in teh tool and warp to a grace in Caelid. Example Outside the plaza. <br/>
> 4. In the debug tool go to the `misc` tab and type in `310`. <br/>
> 5. Press check <br/>
> 6. If the power button turns Green,  Then press continue from the main menu.

<details markdown="block">
<summary>If the power button is RED </summary>


> 7. Click enable and quit to main menu.<br />
> 8. Press continiue in the main menu. <br />
> 9. Check if you can see the crater marker on the map.<br />
> 10. Follow the steps for `If the power button is GREEN`
</details>

<details markdown="block">
<summary>If the power button is GREEN </summary>


> 7. Click disable and quit to main menu.<br />
> 8. Check if you can see the crater marker on the map.<br />
</details>

</details>

<details markdown="block">
<summary> Stuck at Ranni's rise. Invisible wall and can't warp.  </summary>


> 1. Download the debug tool : [Nordgaren's Elden Ring Debug Tool](https://github.com/Nordgaren/Elden-Ring-Debug-Tool/releases/latest) <br/>
> 2. Extract the zip file with your prefered file archiver. <br />
> 3. Open the tool when you are loaded in on your character while solo. <br/>
> 4. Make sure you are close to Ranni's rise. <br />
> 5. In the Debug tool go to the `misc` tab at the bottom of the tool. <br />
> <br /> <b>NOTE:</b> <br />
> 1 = Enabled = GREEN. <br />
> 0 = Disabled = RED. <br /> 

<details markdown="block">
<summary>Short version. </summary>


> 6. Enter `1034509416` and click check. <br />

<details markdown="block">
<summary>If the power button is GREEN </summary>


> 7. Click disable and sit at the grace.<br />
> 8. Check if you can leave.<br />
> 9. If it has not do the steps for if the power button is RED. <br />
</details>

<details markdown="block">
<summary>If the power button is RED </summary>


> 7. Click enable and sit at the grace.<br />
> 8. Check if you can leave.<br />
> 9. Else follow the `Long and proper way`.
</details>

</details>

<details markdown="block">
<summary>Long and proper way. </summary>


> You will need to manually check all the flags one at a time for this step of Ranni's quest. <br />

```
Advancing Ranni's Questline to the point where she goes into her slumber -

// Choosing to enter Ranni's service
1034509410    1
1034509412    1
1034500738    1
1034500732    1
1034500736    1
1034505015    1
1034509361    1
1034500715    1
1034500710    1
1034500700    1
1034490701    1
1034490700    1
1034509413    1
1034509418    1

// Exhausting Iji's dialogue in Ranni's Rise
1034509355    1
1034509357    1
1034509358    1

// Exhausting Blaidd's dialogue in Ranni's Rise
1034509205    1
1045379208    1

// Exhausting Seluvis' dialogue in Ranni's Rise
1034509305    1
1034509306    1

// Exhausting all 3 dialogues activating Ranni's next dialogue/step
1034509417    1
1034500734    1

// Exhausting Ranni's dialogue after talking to all 3 spirits
1034509416    1
1034500738    0
1034500739    1
1034500733    1
1034502610    1
1034505002    1
1034505003    1
1034505004    1
1034500716    1
1034503600    1
```
> <br />
> Sit at a grace when you are done checking and setting the flags. <br />
> Check if you can leave.
</details>

</details>

