---
layout: default
title: Frequently Asked Questions
---
### What is Satyr Farm?

SatyrFarm is a complete farming system for roleplay or just for fun in Opensimulator regions. It contains farm plants, trees, storage, processing machines as well as multiple breedable animals

### Where can I Get It?
You can get the current up-to-date farm package from the OpenSimWorld Region in Metropolis Grid: https://opensimworld.com/hop/74730-OpenSimWorld. The package contains the complete farm as well as some documentation and extra tools. 

### How do i Set up the basics?
Easy! When you get a copy of SatyrFarm, then you can rez the <b>Satyr Farm Platforms</b> which have all the basics ready. Make sure you rez it in a large empty space, as it contains a lot of stuff.  As a general rule, we suggest that you start growing some crops before growing many animals, otherwise your animals might get really hungry! You should read the <a href="/quickstart">quickstart guide</a> for your first steps.

### How do I make animals ###
The package contains the SF Animal Rezzer box, which is used to rez new animals for your farm. 

### How do I feed the animals ###
The animals use various Feeder objects to feed themselves. The feeders are included in the package. Click your animal -> Options -> Help to find out which Feeder to use. Each feeder's menu lists the foods you can add to it.

### My animals are spinning in place
If an  animal seems to be spinning in place, it is because you have moved it manually. Click "Stop"  to  have it start wandering again.

### What is the HUD for? ###
The  HUD  is for eating food that you make in the Kitchen, Oven, Coffee maker etc. Clicking "Consume" to try to eat anything that is around you. 

### What is the SF Buffet for? What is the Bar for? ###
The Bar and Buffet are party items that give you a glass or a plate to fill. Click "Get Glass" or plate and wear it  before getting a drink or food. The Buffet & Bar are not related to the HUD and do not change your hungry/thirsty levels

### How does the Farmer NPC Work?
The Farmer NPC is constantly looking for farm items within his range (90m). It will try to get water from a Well and water every plant with <30% water. It will harvest plants and put their harvest in the nearest Storage Rack. When he harvests Potatoes, he will cook slop in the nearest Kitchen, and then put the slop in Fridge. Therefore the NPC can completely sustain your farm, assuming that you have turned AutoFeed On on your feeders.

### Why doesn't the Farmer/Cat NPC work in my region
The Farmer and Cat NPC boxes require the following permissions to be allowed in your opensim .ini  files:
<pre>
allow_osGetNotecard=true
allow_osMessageObject=true
</pre>
You need to change these settings or get your sim host to change them for you. The settings can be found either in your OpenSim.ini file (in the same folder where OpenSim.exe is)  or in the config-include/osslEnable.ini. You must also have enabled NPCs in your region (Set `Enabled = true` in the `[NPC]` section of your OpenSim.ini file).  

### My farmer/cat NPC does not move ###
After you rez the Farmer NPC, click again "Start" to have him begin farming. There must be a Well within 90m from him and some farm plants to water. If you are getting script errors or it is not moving, please see the previous question. For the cat NPC, make sure you place an SF Cat Feeder near the cat or the cat ll go hungry.

### Why can't I see the Farmer NPC
If the Farmer NPC does not appear in your region, it means its assets are missing from your grid. You can recreate the NPC using the contents of the NPC box. Wear the Smurf avi and the FarmerListener Object, and click "SaveAppearance" to recreate his notecard. You can of use any other avatar apart from the smurf to create any NPC you want. You can also change his name in the 'config' notecard.

### Can I upgrade my older stuff? 
We recommend that you get the newest version  for all features to work. However, since version 2018.08.31, the package includes an updater that updates the scripts in older items. Click the package to get a drop-in script first. Then drag that script from your inventory into the contents of all your older plants, and the script will prepare them for update. When ready, click the updater box again and select Upgrade. Future versions of the farm will not require the drop-in scripts. 

### Is it in Second Life, too?

SatyrFarm is only available in opensim. It makes heavy use of the OSSL functions that are not available in SL. In addition, it is licensed for non-commercial use only, so it is unlikely to appear in SL. 
