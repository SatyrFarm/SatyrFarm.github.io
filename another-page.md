---
layout: default
---

## Quickstart Guide

For the latest  SatyrFarm package, visit OpenSimWorld:  hypergrid.org:8002:OpenSimWorld 

### Farm Basics

- You  must be in the same group as the farm objects to use them. Everyone in the same group can use your farm.
- To get a bucket of water, click the Well. A bucket will be rezzed in front of the well.
- You can touch a bucket and it will follow you. Touch it again to put it down.
- The names of the objects starting with "SF " must not be changed. The names are important for the functipning of the farm.
- Bring a bucket near a plant, then touch a plant to water it. Alternatively you can turn on the AutoWatering feature of the plants, which will automatically take water from the nearest SF Water Tower when needed.
- ** DO  NOT TAKE ITEMS IN INVENTORY, THEY WILL BECOME UNUSABLE **. Put them in the storage barrels instead. (This is not like G&S). Only the animals can be taken to inventory and they will not starve while they are in inventory although they will keep growing**. 
- Autowatering requires the presence of a SF Water Tower in a distance less than 96m.  Similarly AutoFood requires an SF Storage rack or SF Fridge with enough food within 96m radius. 
- The SF Windpump automatically fills up the nearest water tower. the Water Tower can automatically water everything if you have autoWater enabled
- The SF Rack and Fridge are for storing harvested items for longer term. Animal feeders can automatically take items from them if you turn on the  AutoFood option.

### Animals

- Use the SF Animal Rezzer to rez new animals. They will be randomly female or male  on rez. 
- Animals feed from a the various SF Feeder objects. Grass-eating animals use the "SF Feeder" feeder. Dogs use SF Dog Feeder, Pigs use SF Pig Feeder etc.
- When you select "Stop" from the animal menu, the animal will start wandering randomly up to 5 meters away from the stopping point. 
- After female animals become adult, they can mate. You have to select "Mate" - they won't mate on their own. 
- If an  animal seems to be spinning in place, it is because you have moved it manually. Click "Stop"  again to  have it start wandering.

### Kitchen

You can add recipes to the SF Kitchen. The RECIPES notecard contains a recipe in each line. There are 2 formats. Old and New ones
The Old format is each recipe in a single line with the following  fields separated by '=': 
- Name of Recipe in the menu
- Ingredients separated by commas (without the "SF" prefix), each incredient can contain "or" and percentages
- Time to cook (in seconds)
- The object to rez from the kitchen's inventory after cooking (with the "SF" prefix)
- Extra parameter (optional)
E.g.
Cake=Water,25% Flour,Apples or Tomatoes or 25% Orange Juice ,Eggs=300=SF YummyCake

The Distillery, Juicer, Wine maker, Olive oil maker use the same script as the kitchen and work in  the same way

### Storage barrels

Storage boxes can store any of the SF* products. You only need to add a copy of the product inside and it will appear in the menus. To add a  buckets or  products to the storage barrels, it  must be 100% full. 


### Drink Maker

The drink maker is a bar that needs to be stocked with bar-related products and is used to mix them. It is a combination of storage & kitchen and uses similar recipe format (But see the script for details of recipe parameters)


### Selling products
- You can sell your excess harvested items to the OSW Farm Seller truck to win game points if you connect it to your opensimworld.com account. Your current score (points) will be shown in your opensimworld profile. 

- For sims with  real or fake money systems, you can use the "SF Market OSMoney". There is a notecard inside where you set the price of each item. The first number between the '=' is  the price at which the SF Market sells the items, and the second number is the price at which the Market buys them. 

- For sims without money system, you can use the "SF Market NoMoney", which works exactly same way, but instead of simulator money, it  stores the money balances in the script's memory.


### Making  custom products

Please make use of the latest scripts from the SatyrFarm repository for your custom products. If you plant to distribute them , you must ensure that every item and all the items that it contains in its inventory recursively must be full perm, otherwise your product will not work for other users. 


### License
The farm scripts are licensed under the Creative Commons Attribution-NonCommercial (CC-BY-NC) 4.0 International License. To view a copy of this license, visit http://creativecommons.org/licenses/by-nc/4.0/ or send a letter to Creative Commons, PO Box 1866, Mountain View, CA 94042, USA. You are free to modify / create your own items for non-commercial reasons.

To our knowledge all the farm objects and meshes are Freebies and we thank the makers for their work. If you have better open source meshes to contribute, please contact us



[back](./)
