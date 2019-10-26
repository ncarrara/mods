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
  
**How it works**

Hero:
* create a new unit by copying a ram (with Advance Genie Editor 3 (AGE3))
* transform the unit into a building, with building interface and unit type.

Spell:
* create a new unit, acting as spell. 
* make sure this unit is created from the hero (building)
* add a trigger that detect this unit, cast the spell, then delete the unit

Consumables:
* create a new units that die instantly, acting as consumable
* When dying, this unit must provide 1 point of a new ressource (for example AK unused 198).
* In Age of king trigger studio, add a trigger that detect this new resource, then trigger the effect, and remove the resource.
* When buying this new unit, make sure to rally the unit inside a close hero/ram/transport ship. That way the unit won't instantly die, it will stay inside the hero.

Item equip/desequip:
* create a new unit, act as an item (armor/weapon/etc)
* once created, use a trigger to teleport the unit to a part of the map
* move the unit to an area to equip the item, desequip by moving the unit out of the area



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
  
**Screenshots**

![Alt text](img/1.png?raw=true "Buy from the merchant")

![Alt text](img/2.png?raw=true "Armory")

![Alt text](img/3.png?raw=true "Effects")


![Alt text](img/4.png?raw=true "Map template")

![Alt text](img/5.png?raw=true "Equip heavy armor")
