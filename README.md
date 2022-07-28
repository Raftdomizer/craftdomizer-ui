# What is Raftdomizer?

In its current state, Raftdomizer allows for the user to load a file generated from http://www.example.com. The file generated, `RecipeOverride.json`, shuffles the resources, materials and/or quantities for each item in the crafting menu. Currently it is limited to the starting crafting menu but will be expanded upon in the future. Once the file is generated, it should be placed in `mods\ModData\RecipeRandomizer` folder. When the mod is loaded it will read the contents of the generated file and update the in-game recipes with what is in the `RecipeOverride.json` file. It is recommended that a fresh world is used for this and the user is open to adjust the file at any point they see fit.

# So it is not truely random?
The short answer is no. If anything it is an Crafting Menu adjuster. As such if the user finds that the crafting items are either too generous or difficult, they can be adjusted. In a future state, I would like to store this information in game and then allow the user to override it if they like

# Will this work with other mods?
Depends on what other mods it is loaded with. This mod does override a number of the vanilla recipes so any other mods that perform that operation may yield varying results.

# How are the random quantities for each crafted item determined?
When shuffling only cost, the new cost can either be 50% to 125% of its original cost with a minimum cost of 1 rounded down. For example, the number of planks required for an Engine is 20. The new cost could be as low as 10 planks and as much as 30 planks. For another example, a Stone Axe requires 3 stones, so the new cost can be as low as 1 and as high as 4.

For shuffle ingridents and cost, the baseline cost are below. Same rules apply where cost can be between 50% to 125% of cost
- Plank: 6
- Plastic: 4
- Palm Leaf: 9
- Scrap: 1
- Rope: 3
- Stone: 3
- Nail: 3

This is not a complete list and is subject to change


# Features
 - Shuffling of ingridents and quantities for the starting crafting menu
 - Shuffling of quantities for starting craft menu maintaining vanilla requirements

# Future
 - Tier/Sphere based progress to further randomization
 - Include flowers, fruits, seeds, vegetables, fish and their cooked variants as options to be shuffled
 - Allow Crafting Menu items to be used for other Crafting Menu items