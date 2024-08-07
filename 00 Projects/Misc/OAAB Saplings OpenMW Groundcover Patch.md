## Description:  

This patch enables OpenMW to utilise Melchior Dahrk's 'OAAB Saplings' as groundcover in OpenMW versions 0.47+, improving engine performance as opposed to the static models. This is no longer possible with the original OAAB Saplings mod since OpenMW's handling of groundcover changed in OpenMW 0.47.  
  
Alternatively, consider using Groundcoverizer by Benjamin Winger or Habasi by Alvazir. These tools can create groundcover for all the grass/kelp type flora statics in your whole mod loadout, reducing the likelihood of conflicts and giving more comprehensive performance improvements. They take a bit to get your head around, but the pay-off is worth it! However, the patches included with this are useful.  
  
## Requirements:  

This mod is a complete replacer for OAAB Saplings and includes the sapling meshes from OAAB Data, now placed in a 'meshes/grass' folder. 

- The original OAAB Saplings mod is not required.  
- If using the '01 patch for OAAB Saplings West Gash for BCOM and SWP', 'Beautiful Cities of Morrowind' and 'Stonewood Pass Reworked' by RandomPal are required.  
- The original 'OAAB Saplings West Gash for BCOM and SWP' patch is not required.  
- 'Melchior's Excellent Grazelands Acacia patch', 'SM Bitter Coast Tree Replacer patch' and 'Graht Morrowind Swamp Trees patch'
  
## Installation:  

Pick from the following folders

- 00 Core - **Required**. Contains saplings meshes stored in a grass folder, and the six OAAB Sapling ESPs. (Do not enable OAAB_Saplings_WG.esp if using the patch below)  
- 01 - Optional - **Only use one**:  
	- 01 BCOM patch for OAAB_Saplings_WG - patch for 'Beautiful Cities of Morrowind', fixes floaters in cell Balmora -3,-2 (credit to Sophie)  
	- 01 SWP + BCOM patch for OAAB_Saplings_WG - patch for 'The Stonewod Pass Reworked' and 'Beautiful Cities of Morrowind' (credit to Mrovkogon)  
- 02 OAAB_Saplings_AC BCOM Patch (credit to Sophie on MMC for the fix!)  
- 03 Melchior's Excellent Grazelands Acacia patch - Optional - requires original mod. Load after 00 Core.  
- 04 - Optional - **Only use one:**  
	- 04 SM Bitter Coast Tree Replacer patch - Optional - requires original mod. Load after 00 Core.   
	- 04 Graht Morrowind Swamp Trees patch - Optional - requires original mod. Load after 00 Core.  
- 05 Great Seawall of Vivec Patch - removes saplings from the walkway in cells 6 -13, 6 -14, 7-13. (credit to Sophie)  
  
### ENABLING GROUNDCOVER IN OPENMW - REQUIRED:  

1. Ensure Groundcover is enabled in OpenMW:

 Locate your 'Settings.cfg' folder in your operating system's User Directory:  
- Windows `C:\Users\ *Username* \Documents\my games\OpenMW`  
- GNU/Linux `~/.config/openmw/`  
- OS X `~/Library/Application Support/openmw/`

Add the following lines to the Settings.cfg:  
  
```
[Groundcover]  
enabled = true  
density = 1.0  
min chunk size = 0.5  
stomp mode = 2
stomp intensity = 0
```

- Use either **stomp intensity = '0' or '1'** - using stomp intensity 2 causes the meshes to respond wildly to the player colliding with them.  
  
2) Enable the desired groundcover plugins (DO NOT ACTIVATE THESE IN THE OPENMW LAUNCHER):

- Locate your openmw.cfg (in the same directory as settings.cfg) and add the following lines to the bottom of the document below the last `content=`:  

```
groundcover=OAAB_Saplings_AC.esp  
groundcover=OAAB_Saplings_AI.esp  
groundcover=OAAB_Saplings_BC.esp  
groundcover=OAAB_Saplings_GL.esp  
groundcover=OAAB_Saplings_SG.esp  
groundcover=OAAB_Saplings_WG.esp  
```

**References:**
- [Tips: Performance](https://modding-openmw.com/tips/performance/) (Modding-OpenMW.com) 
- [Groundcover Settings](https://elsid-openmw.readthedocs.io/en/latest/reference/modding/settings/groundcover.html) (OpenMW manual on Read the Docs) 
  
## How was this made?  

OpenMW groundcover mods need to load meshes from a folder called 'Grass'. I just placed the meshes there and changed the file path to the meshes in the plugins.  
  
## Acknowledgements:   

- **MelchiorDahrk** as author of the original [OAAB Saplings](https://www.nexusmods.com/morrowind/mods/50334) Mod, [Melchior's Excellent Grazelands Acacia](https://www.nexusmods.com/morrowind/mods/51058) and [Vanilla Friendly West Gash Tree Replacer](https://www.nexusmods.com/morrowind/mods/44173).  
- **Mrovkogon** as author of the original patch ['OAAB Saplings West Gash for BCOM and SWP'](https://www.nexusmods.com/morrowind/mods/50626)
- **MelchiorDahrk** and **XeroFoxx** for [Graht Morrowind Swamp Trees](https://www.nexusmods.com/morrowind/mods/49771)  
- **CMAugust** on the OpenMW Discord for identifying why the original OAAB Saplings no longer worked as groundcover in OpenMW  
- **Greatness7** for [Tes3conv](https://github.com/Greatness7/tes3conv)  
- **Hemaris** for inspiring this idea with their ['Turn Normal Grass and Kelp into Groundcover'](https://www.nexusmods.com/morrowind/mods/52010) and ['Stirk Performance Improver'](https://www.nexusmods.com/morrowind/mods/52058) mods.  
- The team at [OAAB_Data](https://www.nexusmods.com/morrowind/mods/49042)  
- Thanks to **Sophie** on the MMC Discord for creating the OAAB_Saplings_AC & WG BCOM patches, and the [Great Seawall of Vivec](https://www.nexusmods.com/morrowind/mods/53544) patch  
  
Make sure to endorse the original mods!