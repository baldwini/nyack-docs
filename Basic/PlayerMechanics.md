# Movement
---
The player is able to move in all directions and is affected by gravity. They have the option to walk or sprint. Sprint should have a toggle-able option within game options. The player is able to jump and move vertically about half their height, one Unity unit, to reach areas across large gaps in the floor or to clamber small obstacles. The [[Skills#Speed|speed]] the player moves is dictated by their character's statistics.

# Inventory
---
The inventory holds all items the player picks up. There are set places for some equipment items like [[#Wearable Slots|clothing and armour]] pieces. Items can be pulled out of the inventory screen into the player's hands or ground as well as being placed back into the inventory. Almost all items will be visually represented on the player character even if not traditionally equip-able, specifically weapons, HERE The player inventory will based on slots; grid based is more 'realistic' as it shows that different objects have different shapes and sizes while slot based is way easier to manage and organize. However, we are combining the benefits from both to accommodate realism without making inventory management a separate 'Tetris-like' experience. That combination would be slot based in spirit but separating items based on size and weight which is predetermined by us the developers. The slot types would be simple, displayed as heavy and light item slots, in which light items would only fit into light item slots and heavy items would only fit into heavy item slots. The player's hands, which dictate their current actions, count as both slot types. For the player to get more heavy slots and light slots they would need to acquire wearable backpacks and or belts. Other slots will be for jewellery and equipped items. One handed weapons or items will only fill one slot while two-handed items will take both hand slots. Belt items can also be found in the game which allow the player to have additional slots to hold consumable items, displayed on the heads up display; some belts may only have one slot while others may give the player access to three at a time. Belts do not traditionally have [[Armour|damage resistance or damage negation]].

## Wearable Slots
The inventory will have a slots dedicated to [[Skills#Armour|armour]] pieces for the player's torso, head, hands, legs, and feet. The legs, hands, and feet will not have separate slots for both left and right. Armours will not cover multiple sections of the slots. The wearable items are also slot dependent; pouches are heavy, belts are heavy, clothing that isn't armour is light, armour is heavy, backpacks are neither as they are only wearable.

There will be three slots for different types of wearable equipment for each body part. Wearable items can only be put into the slot they are defined as, which include:
- Clothing, segmented by each body part as additional slots
- Belts, as an additional legs slot
- Backpacks, as an additional torso slot
- Jewellery, as an additional hands slot
- Face wear, as an additional head slot
- Anklet, as an additional feet slot

# Items
---
Items may act as objects that tell the player about world variables or act as "keys" that unlock near level segments. Other items will be consumables, player equipment, or ingredients. All items physically exist within the world and will be seen on enemies, in their hands, and/or backpack. If the player can a non-player character has an item it will drop from them if the non-player character are disoriented or messed with.

## Picking Up Items
---
- Drag Selector
	The drag selector will be used to select many items on the player's screen. This can be done by holding down the *E key* and using *left mouse button* to drag across the screen, when the *left mouse button* is let go then a menu will open up with all the items within the drag selection. When the items are *double clicked* in the drag selection menu they will be put into the player's inventory as the player character automatically walks over to the item in the game world and picks them up. Once the player character walks over to the item it will be placed into the inventory menu.

- Nearby Object
	When the player is next to an object that can be picked up then the player can press the *E key* with the cursor over the object in the game world and it will be placed into the player's inventory.

- Inventory Menu
	If the player is in their inventory menu then they can drag and drop items from the game world into the inventory menu. The player character will automatically walk over to the item dragged over; when the player character reaches the location of that item it will be placed into the player's inventory.

# Magic
---
The player will have the ability to cast spells, limited to two at a time. These will affect the player, hostiles, non-player characters, and or the nearby environment. Each spell can have fairly versatile usage, allowing for each spell to act as two or three. For example, a fire spell can be used to create a fireball that can be held by the player to emit light, set object ablaze, or be thrown as a projectile. Spells will be user created and tailored to player needs, this comes at a cost however. Spell effects will be locked into gemstones that can be erased. These gemstones can be locked into jewellery or held in the player's hand for casting. 

**Possible Ways of Casting**:
- Casting spells individually with your cursor
- A UI that pops up on the screen that lets the player cycle through spells

# Ready
---
Readying a weapon changes the controls for the *mouse buttons*. After a weapon is readied using the *R* key then the weapon will be pulled out or the players hands will posed at an angled stance. This will disable the feature that allows the player to inspect or pickup objects.
	The speed of the readying animation will be dependent on the type of weapon and [[Attributes|Dexterity]].

# Throwing
---
Throwing is governed by the [[Skills#Throwing|skill of the same name]]. To throw an item that the player character is holding they must have their cursor over three Unity units away from the player character and hit *middle mouse*. If the player has hit the assigned input to throw the currently held item while they are not aiming at a non-player character and they are aiming within three Unity units of their player character, then the player character will instead drop the item. Dropping will stand the object upright instead of using the physics system built into Unity and the game with play a different animation for doing this action.
# Contextual Interaction
---
- Weapons
	While the player is holding a *[[PlayerMechanics#Ready|readied]]* [[equipment#weapons|weapon]] or empty hands they may only attack, either light attack or heavy attack, by [[GameSettings#Controls|using one of the mouse buttons]]. They also have the additional option to throw the weapon wherever their cursor is pointed. The player will then player the cursor after they ready their weapon and their character's speed and movement will change.

- Tools
	If the player is holding a [[equipment#Tools|tool]] item the available options shift to being able to throw the tool they are holding, using the tool, or use a specific function that is unique to that individual type of tool. If a tool has a unique function then it is listed in the [[equipment]] section.

- Keys and Materials
	When the player is holding a [[Equipment#Keys|key]] or [[Equipment#Materials|material]] item they have the ability to use it, throw it, or inspect the object they have their cursor hovered over in the game world.