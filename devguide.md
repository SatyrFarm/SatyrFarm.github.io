## Creating new Farm Items

The farm is designed to be easily expandable. Starting from v2018.08 most of the options of the farm are configurable through the 'config' notecard. 

### Fields & trees
Adding a a field or a tree requires the following steps (we take Mango as an example)
- Create the new product for your field, SF Mango, by copying an existing product. 
- Set "EXPIRES=N" in the config notecard inside it, where N is the number of days before expiration. 
- Set all the inventory items in the product to full perms, and Take the object into inventory
- Add the product to the tree, along with 3 textures: Mango-New, Mango-Growing, Mango-Ripe. Make sure they are full perm
- Open the 'config' notecard of the tree and add  ",SF Mango" at the end of the "PRODUCTS=" line
- Reset scripts on tree. Now Mango should be an option.

Optional:

Set `MATURATION=D` if your product takes a few days to mature. D is the number of days before being ready.
Set `EXTRAPARAM=Hungry:-10|Thirsty:-10`  for your product to work with the HUD. -10 means the product will make you 10% less hungry and 10% less thirsty. These can be positive or negative numbers.

If you plan to create more complex functionality you should add an addon script to the field or tree. Do not modify the main script as your changes will be overwritten  in the next release of the farm. The tree.lsl script sends a number of link_messages when actions happen. Search the tree.lsl script for llMessageLinked lines to see those messages and use them in your addon. 



### Storage Boxes

Storage boxes are automatically configured. You can add a new storage option by simply adding the new SF Product item in the inventory of the storage box.


### Processing machines, Kitchens etc.

#### Recipes
To create a recipe, you just need to add a line in the RECIPES notecard inside any food-processing object like the Kitchen, Juicer, microbrewery etc. The format is:

`Mango Juice=Water, 50% Mango, Salt or 20% Sugar=200=SF Mango Juice`

where  the fields between '=' are:
- Menu item label
- Ingredients. Ingredients can contain " or" and percentages as shown
- Time it takes to cook in seconds
- The name of the object to rez from inventory


#### Creating new machines
You should be able to create new machines by adding and modifying options in the 'config' notecard. If your machine requires that you sit on it while processing, set `MUST_SIT=1` . The following conventions are also supported:
- If you name one of the prims in the linkset `show_while_cooking` it will be shown (alpha 0%) during cooking only, and hidden afterwards. You can set an arbitrary alpha level for the link like 0.5 by naming it `show_while_cooking 0.5`
- If you name one of the prims in the linkset `spin <0,2.0,0>` it will spin in the Y local axis with spin rate 2 while cooking. You can change the vector to point to the direction and spin rate you wish.

If you plan to create more complex functionality you should add an addon script to the processor. Do not modify the main script as your changes will be overwritten  in the next release of the farm. The kitchen script sends a number of link_messages when actions happen. Search the kitchen.lsl script for llMessageLinked lines to see those messages and use them in your addon. 

