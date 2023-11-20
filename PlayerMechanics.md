# Movement
---
The player is able to move in all directions and is affected by gravity. They have the option to walk or sprint. Sprint should have a toggleable option within game options. The player is able to jump and move vertically about half their height, one Unity unit, to reach areas across large gaps in the floor or to clamber small obstacles. The [[Skills#Speed|speed]] the player moves is dictated by their character's statistics.

# Inventory
---
The inventory holds all items the player picks up. There are set places for some equipment items like swords and armor pieces. Items can be pulled out of the bag into the player's hands or ground as well as being placed back into the bag. All items will be visually represented on the player character even if not traditionally equip-able. The player inventory will have to be grid based or slot based; grid based is more 'realistic' as it shows that different objects have different shapes and sizes while slot based is way easier to manage and organize. The inventory will have a slots dedicated to armor pieces for the player's torso, head, hands, legs, arms, and feet. The legs, arms, hands, and feet will have separate slots for both left and right. Some armors will cover multiple sections of the slots. For example, a pair of pants can cover both right and left legs. Other slots will be for jewelry and equipped items. One handed weapons or items will only fill one slot while two-handed items will take both equipment slots. Belt items can also be found in the game which allow the player to have additional slots to hold consumable items, displayed on the heads up display; some belts may only have one slot while others may give the player access to three at a time. Belts do not traditionally have [[Armor|damage resistance or damage negation]].

# Items
---
Items may act as objects that tell the player about world variables or act as "keys" that unlock near level segments. Other items will be consumables, player equipment, or ingredients. All items physically exist within the world and will be seen on enemies, in their hands, and/or backpack. If the player can a non-player character has an item it will drop from them if the non-player character are disoriented or messed with.

# Magic
---
The player will have the ability to cast spells, limited to two at a time. These will affect the player, hostiles, non-player characters, and or the nearby environment. Each spell can have fairly versatile usage, allowing for each spell to act as two or three. For example, a fire spell can be used to create a fireball that can be held by the player to emit light, set object ablaze, or be thrown as a projectile. Spells will be user created and tailored to player needs, this comes at a cost however. Spell effects will be locked into gemstones that can be erased. These gemstones can be locked into jewelry or held in the player's hand for casting. 

We have a few different options for selection below:
- Casting spells individually with your cursor
- A UI that pops up on the screen that lets the player cycle through spells