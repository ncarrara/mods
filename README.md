# mods
Custom RPG mod for Age of Empire 2 2013 (HD)

It is a work in progress framework for Role Playing in Age of Empire 2. It's more like a set of templating files than an actual playable mod.

![Alt text](img/0.png?raw=true "Spells and Consumables")

Featuring:
  - casting spells directly from heroes.
  - using consumable items directly from heroes.
  - equip/desequip armor/weapons.
  - buy consumables from a merchant.
  - buy weapons/armors from the blacksmith building.
  
Actually implemented:
- health/mana/energy potions
- heavy armor
- 1 heroes
- 1 spell (fatal blow)
- merchant and custom backsmith

*rpg - dataset*
  Contains the .dat file with new units and items

*rpg - strings*
  Contains the modified strings for the new units and items

*rpg - map*
  Template map with triggers.

**How to install**

* Copy those 3 folders to steam\steamapps\common\Age2HD\mods
* Run Age of Empire  HD on steam
* Go to the workshop utility and activate the string (move the mod up to the list)
* Create a new game (single of multiplayer) and choose the custom rpg dataset and the rpg scenario.

**How to edit**

In order to edit the map with the customs unit, first, create a single game with the dataset. 
Then quit the game, and edit the template rpg.aoescenario witht he scenario editor.

I recommend these softwares to modify the dataset and the scenario:
  * Advanced Genie Editor [http://aok.heavengames.com/blacksmith/showfile.php?fileid=11002]
  * AoK Trigger Studio [http://aok.heavengames.com/blacksmith/showfile.php?fileid=12103]
