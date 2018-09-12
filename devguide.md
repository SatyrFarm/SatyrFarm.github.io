<h2 id="creating-new-farm-items">Creating new Farm Items</h2>

The farm is designed to be easily expandable. Starting from v2018.08 most of the options of the farm are configurable through the ‘config’ notecard.

<h3 id="fields--trees">Plants, trees etc. (plant.lsl)</h3>
Adding a a field or a tree requires the following steps (we take Mango as an example)
<ul>
  <li>Create the new product for your field, SF Mango, by copying an existing product.</li>
  <li>Set <code>EXPIRES=N</code> in the config notecard inside it, where N is the number of days before expiration.</li>
  <li>Set all the inventory items in the product to full perms, and Take the object into inventory</li>
  <li>Add the product to the tree, along with 3 textures: Mango-New, Mango-Growing, Mango-Ripe. Make sure they are full perm</li>
  <li>Open the ‘config’ notecard of the tree and add  <code>,SF Mango</code> at the end of the <code>PRODUCTS=</code> line</li>
  <li>Reset scripts on tree. Now Mango should be an option.</li>
</ul>

Optional:

Set <code>MATURATION=D</code> if your product takes a few days to mature. D is the number of days before being ready.
Set <code>EXTRAPARAM=Hungry:-10|Thirsty:-10 </code> for your product to work with the HUD. -10 means the product will make you 10% less hungry and 10% less thirsty. These can be positive or negative numbers.

If you plan to create more complex functionality you should add an addon script to the field or tree. Do not modify the main script as your changes will be overwritten  in the next release of the farm. The tree.lsl script sends a number of link_messages when actions happen. Search the tree.lsl script for llMessageLinked lines to see those messages and use them in your addon.

<h3 id="storage-boxes">Storage Boxes (storage.lsl)</h3>

Storage boxes are automatically configured. You can add a new storage option by simply adding the new SF Product item in the inventory of the storage box.

<h3 id="processing-machines-kitchens-etc">Kitchen (kitchen.lsl)</h3>

<h4 id="recipes">Recipes</h4>
To create a recipe, you just need to add a line in the RECIPES notecard inside any food-processing object like the Kitchen, Juicer, microbrewery etc. The format is:

<pre>Mango Juice=Water, 50% Mango, Salt or 20% Sugar=200=SF Mango Juice</pre>

where  the fields between ‘=’ are:
<ul>
  <li>Menu item label</li>
  <li>Ingredients. Ingredients can contain “ or” and percentages as shown</li>
  <li>Time it takes to cook in seconds</li>
  <li>The name of the object to rez from inventory</li>
</ul>

<h4 id="creating-new-machines">Creating new machines (kitchen.lsl)</h4>
You should be able to create new machines by using the kitchen.lsl script. The recipe format is described above. You can add and modifying options in the ‘config’ notecard. If your machine requires that you sit on it while processing, set <code>MUST_SIT=1 </code>. The following conventions are also supported:
<ul>
  <li>If you name one of the prims in the linkset <code>show_while_cooking</code> it will be shown (alpha 0%) during cooking only, and hidden afterwards. You can set an arbitrary alpha level for the link like 0.5 by naming it <code>show_while_cooking 0.5</code></li>
  <li>If you name one of the prims in the linkset <code>spin &lt;0,2.0,0&gt;</code> it will spin in the specified vector local axis with spin rate of 2 while cooking. You can change the vector to point to the direction and spin rate that you wish.</li>
</ul>

If you plan to create more complex functionality you should add an addon script to the processor. Do not modify the main script as your changes will be overwritten  in the next release of the farm. The kitchen script sends a number of link_messages when actions happen. Search the kitchen.lsl script for llMessageLinked lines to see those messages and use them in your addon.

<h3>Animals (kitchen.lsl)</h3>
See the tools/animal_pose_maker.lsl for instructions how to create poses for a new animal.

Animal configuration is saved in 'an_config' notecard.

Prims configuration:
<ul>
<li>Prims named  <code>adult_prim</code> are only shown in adult animals</li>
<li>Prims named  <code>child_prim</code> are only shown in child animals</li>
<li>Prims named  <code>egg_prim</code> are only shown if the animal is in Egg state</li>
<li>Prims named  <code>adult_male_prim</code> are only shown in adult male animals. Similarly for <code>adult_female_prim</code></li>
<li>Prims named  <code>adult_random_prim</code> will be visible with 50% probability when the animal becomes adult(for non-standard features like horns)</li>
</ul>
