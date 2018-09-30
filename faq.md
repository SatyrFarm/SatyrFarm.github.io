---
layout: default
title: Frequently Asked Questions
---


<h3 id="what-is-satyr-farm">What is Satyr Farm?</h3>

SatyrFarm is a complete farming system for roleplay or just for fun in Opensimulator regions. It contains farm plants, trees, storage, processing machines as well as multiple breedable animals

<h3 id="where-can-i-get-it">Where can I Get It?</h3>
You can get the current up-to-date farm package from the OpenSimWorld Region in Metropolis Grid: https://opensimworld.com/hop/74730-OpenSimWorld. The package contains the complete farm as well as some documentation and extra tools.

<h3 id="how-do-i-set-up-the-basics">How do i Set up the basics?</h3>
Easy! When you get a copy of SatyrFarm, then you can rez the <b>Satyr Farm Platforms</b> which have all the basics ready. Make sure you rez it in a large empty space, as it contains a lot of stuff.  As a general rule, we suggest that you start growing some crops before growing many animals, otherwise your animals might get really hungry! You should read the <a href="/quickstart">quickstart guide</a> for your first steps.

<h3 id="how-do-i-make-animals">How do I make animals</h3>
The package contains the SF Animal Rezzer box, which is used to rez new animals for your farm.

<h3 id="how-do-i-feed-the-animals">How do I feed the animals</h3>
The animals use various Feeder objects to feed themselves. The feeders are included in the package. Click your animal -&gt; Options -&gt; Help to find out which Feeder to use. Each feeder’s menu lists the foods you can add to it.

<h3 id="my-animals-are-spinning-in-place">My animals are spinning in place</h3>
If an  animal seems to be spinning in place, it is because you have moved it manually. Click “Stop”  to  have it start wandering again.

<h3 id="what-is-the-hud-for">What is the HUD for?</h3>
The  HUD  is for eating food that you make in the Kitchen, Oven, Coffee maker etc. Clicking “Consume” to try to eat anything that is around you.

<h3 id="what-is-the-sf-buffet-for-what-is-the-bar-for">What is the SF Buffet for? What is the Bar for?</h3>
The Bar and Buffet are party items that give you a glass or a plate to fill. Click “Get Glass” or plate and wear it  before getting a drink or food. The Buffet &amp; Bar are not related to the HUD and do not change your hungry/thirsty levels

<h3 id="when-do-animals-mate-how-do-they-give-milkwool-etc">When do animals mate? How do they give milk/wool etc?</h3>
Animals typically spend 15% of their lifetime as children with some exceptions. The lifetime of each animal varies but you can check their config notecard (LIFEDAYS variable) for an average. Eggs take a few days to hatch. Adult females can mate via the Mate option in the menu. Mammals will start giving milk after their first child. Some adult animals give wool periodically. You can also use the Options-&gt; Help function for this information.

<h3 id="how-does-the-farmer-npc-work">How does the Farmer NPC Work?</h3>
The Farmer NPC is constantly looking for farm items within his range (90m). It will try to get water from a Well and water every plant with &lt;30% water. It will harvest plants and put their harvest in the nearest Storage Rack. When he harvests Potatoes, he will cook slop in the nearest Kitchen, and then put the slop in Fridge. Therefore the NPC can completely sustain your farm, assuming that you have turned AutoFeed On on your feeders.

<h3 id="why-doesnt-the-farmercat-npc-work-in-my-region">Why doesn’t the Farmer/Cat NPC work in my region</h3>
The Farmer and Cat NPC boxes require the following permissions to be allowed in your opensim .ini  files:

<pre>
allow_osGetNotecard=true
allow_osMessageObject=true
</pre>

You need to change these settings or get your sim host to change them for you. The settings can be found either in your OpenSim.ini file (in the same folder where OpenSim.exe is)  or in the config-include/osslEnable.ini. You must also have enabled NPCs in your region (Set Enabled = true in the [NPC] section of your OpenSim.ini file).

<h3 id="my-farmercat-npc-does-not-move">My farmer/cat NPC does not move</h3>
After you rez the Farmer NPC, click again “Start” to have him begin farming. There must be a Well within 90m from him and some farm plants to water. If you are getting script errors or it is not moving, please see the previous question. For the cat NPC, make sure you place an SF Cat Feeder near the cat or the cat ll go hungry.

<h3 id="why-cant-i-see-the-farmer-npc">Why can’t I see the Farmer NPC</h3>
If the Farmer NPC does not appear in your region, it means its assets are missing from your grid. You can recreate the NPC using the contents of the NPC box. Wear the Smurf avi and the FarmerListener Object, and click “SaveAppearance” to recreate his notecard. You can of use any other avatar apart from the smurf to create any NPC you want. You can also change his name in the ‘config’ notecard.

<h3 id="can-i-upgrade-my-older-stuff">Can I upgrade my older stuff?</h3>
We recommend that you get the newest version  for all features to work. However, since version 2018.08.31, the package includes an updater that updates the scripts in older items. Click the package to get a drop-in script first. Then drag that script from your inventory into the contents of all your older plants, and the script will prepare them for update. When ready, click the updater box again and select Upgrade. Future versions of the farm will not require the drop-in scripts.

<h3 id="is-it-in-second-life-too">Is it in Second Life, too?</h3>

SatyrFarm is only available in opensim. It makes heavy use of the OSSL functions that are not available in SL. In addition, it is licensed for non-commercial use only, so it is unlikely to appear in SL.
