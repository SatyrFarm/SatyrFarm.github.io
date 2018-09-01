---
layout: default
title: Frequently Asked Questions
---
### What is Satyr Farm?

SatyrFarm is a complete farming system for roleplay or just for fun in Opensimulator regions. It contains farm plants, trees, storage, processing machines as well as multiple breedable animals

### Is it in Second Life, too?

SatyrFarm is only available in opensim. It makes heavy use of the OSSL functions that are not available in SL. In addition, it is licensed for non-commercial use only, so it is unlikely to appear in SL. 

### Where can I Get It?
You can get the current up-to-date farm package from the OpenSimWorld Region in Metropolis Grid: https://opensimworld.com/hop/74730-OpenSimWorld. The package contains the complete farm as well as some documentation and extra tools. 

### How do i Set up the basics?
Easy! When you get a copy of SatyrFarm, then you can rez the <b>Satyr Farm Platforms</b> which have all the basics ready. Make sure you rez it in a large empty space, as it contains a lot of stuff.  The package contains the SF Animal Rezzer box, which is used to rez new animals for your farm. As a general rule, we suggest that you start growing some crops before growing many animals, otherwise your animals might get really hungry! You should read the <a href="/quickstart">quickstart guide</a> for your first steps.


### Can I upgrade my older stuff? 
We recommend that you get the newest version  for all features to work. However, since version 2018.08.31, the package includes an updater that updates the scripts in older items. Click the package to get a drop-in script first. Then drag that script from your inventory into the contents of all your older plants, and the script will prepare them for update. When ready, click the updater box again and select Upgrade. Future versions of the farm will not require the drop-in scripts. 

### How does the Farmer NPC Work?
The Farmer NPC is constantly looking for farm items within his range (90m). It will try to get water from a Well and water every plant with <30% water. It will harvest plants and put their harvest in the nearest Storage Rack. When he harvests Potatoes, he will cook slop in the nearest Kitchen, and then put the slop in Fridge. Therefore the NPC can completely sustain your farm, assuming that you have turned AutoFeed On on your feeders.

### Why doesn't the Farmer NPC work in my region
The Farmer NPC requires the following settings in your opensim .ini  files: `allow_osGetNotecard=true` and `allow_osMessageObject=true`. These settings can be either in your OpenSim.ini file (in the same folder where OpenSim.exe)  or in the config-include/osslEnable.ini file. You must also have enabled NPCs in your region (Set Enabled = true in the [NPC] section of your OpenSim.ini file).  After you rez the NPC, click again to select Start. If all goes well, the NPC should start searching for the nearest Well.

### Why can't I see the Farmer NPC
If the Farmer NPC does not appear in your region, it means its assets are missing from your grid. You can recreate the NPC using the contents of the NPC box. Wear the Smurf avi and the FarmerListener Object, and click "SaveAppearance" to recreate his notecard. You can of use any other avatar apart from the smurf to create any NPC you want. You can also change his name in the 'config' notecard.

### My animals are spinning in place
If an  animal seems to be spinning in place, it is because you have moved it manually. Click "Stop"  to  have it start wandering again.
