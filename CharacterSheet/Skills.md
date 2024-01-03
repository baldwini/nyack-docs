# Spending Points
---
First-time skill purchases in character creation will increase the skill score by 2. All other skill purchases afterwards, will increase the skill score by only 1. Gaining new skills after character creation can be achieved by trading something in return for training from non-player characters. All modifiers from the skill list below show their unacquainted modifier, before the +2 increase.

# Acquired Skills
---
## Pick Pocket
*DXT-4*
Pick Pocketing a non-player character multiple times will increase the Complexity Rating by 1, with Complexity Rating being given to each item in an non-player character's inventory. Player's may choose to take multiple items at once.

## Barter
*INS-3*
Art of the deal.

- **Example**: Skill in practice...
	A high Barter skill score should be around 50% off normal price, with additional markdown or gain being applied for local and personal reputation scores; while a low Barter could be around a 300% price increase.

## Repair
*INS-4*
The ability to repair broken [[Equipment|items]] and machinery.

- **Example**: Skill in practice...
	5 Repair should allow perfect repair on items and objects with Complexity Rating of 5 or less

## Lock-pick
*DXT-4*
Lock-pick will allow the unlocking of locked doors and chests.

## Disarm
*INS-4*
Disarming will cover the plausibility of successfully disarming a  trap.

## Light Weapons
*DXT-2*
[[Equipment#Light|Light Weapons]] will allow for reaching damage values more reliably with light-class weapons. It is common for these weapons to have less effects than simple-class and colossal-class weapons, they are also the cheapest and easiest to find. This class of weapons are also the most thrown the most reliably, they are faster to throw and do more damage when thrown.
- **Example**: Skill in practice...
	Higher values of the Light Weapons skill will only do maximum damage unless critically hitting, the minimum value of -7 will do minimum damage only.

## Simple Weapons
*DXT-4*
[[Equipment#Simple|Simple Weapons]] will allow for reaching damage values more reliably with simple-class weapons. It is the most common for this class of weapons to have effects than both light-class or colossal-class weapons.

## Colossal Weapons
*DXT-5*
[[Equipment#Colossal|Colossal Weapons]] have high STR requirements to Wield correctly. Colossal Weapons are more harder to come by, cost more, but traditionally have more effects than either light-class but not simple-class weapons.

## Throwing
*DXT-4*
Throwing effects throwing speed and distance. When the player throws outside the distance it is a Complexity Rating check based on distance, target size, and thrown object weight.

## Alchemy
*INS-4*
Alchemy allows for the creation of potions. A check is done when using every player-created potion, if the player passes the check the potency of the potion is increased. The player may fail the check, if the player has a negative in the skill then the potion has a random negative effect, however if the player has a positive in the skill then nothing happens to the created potion and it is used normally.
- **Example**: Potion side effects...
	Increased damage, health regeneration, and or longevity of a potion

## Survival
*INS-4*
Survival allows for player's to rest outside safe areas without harm as well as avoid less hazardous random encounters when exploring.

# Innate Skills
---
## Carry Weight
*STR*
STR 0 - 100 WT
+- 15 WT per level of STR

## Speed
*STR & DXT*
- **Movement Speed** = Speed Score * (1 - (Current Inventory Weight / Carry Weight Maximum))
- **Sprint Movement Speed** = Movement Speed * 1.5
- **Swing Speed** = (Speed Score * 1.5) / Weapon Weight
	Swing Speed is the speed that Animator.speed plays at (1 is default speed, 2 is double speed)

- **Round(Speed Score)** = 5 + (.67 * Dexterity) + (.33 * Strength)

## Health
*VGR*
- **Round(Health Point Total)** = 25 + (Vigour * 4.8)

## Immunity
*VGR*
- Immunity is calculated based on the Vigour attribute; it is represented on the table below.
	Vigour 5 = 0.5 Immunity
	Vigour 4 = 0.6 Immunity
	Vigour 3 = 0.7 Immunity
	Vigour 2 = 0.8 Immunity
	Vigour 1 = 0.9 Immunity
	Vigour 0 = 1 Immunity
	Vigour -1 = 1.2 Immunity
	Vigour -2 = 1.4 Immunity
	Vigour -3 = 1.6 Immunity
	Vigour -4 = 1.8 Immunity
	Vigour -5 = 2 Immunity

## Armour
*STR*
- **[[Attributes#Strength|Strength]] Requirements**: Each attribute score away from the strength requirement is a movement speed and swing speed penalty of 33%, although some armours may have innate speed penalties.

- **Armour defence**: Defined by Damage Resistance and Damage Negation values. Damage values first get subtracted by DN then multiplied by decimal percentages. Armour will have DR and DN for different types of damage. Some of those damage types may be: Pierce, Bludgeon, Slash, Fire, and Electric.
- **Example**: Damage calculation with a Bronze Helmet...
	*Bronze Helmet*: DR 40% / DN 5
	Raw Damage - DN = X * (1 - DR) = Actual Damage

- **Armour Pieces**: Armours are separated into different segments based on [[Equipment#Armour|armour types]]. Some pieces only provide defence of a specific body part while other pieces of armour provide defence to multiple areas. Pieces of armour will have their own individual weights.

# Speech Skills

## Intimidation
*STR*
Additional dialogue option that appears due to the player's [[Attributes#Strength|strength attribute]] score. The check that allows this to be an option for the player will be dependant on the quest or event.
## Deceive
*DXT*
Additional dialogue option that appears due to the player's [[Attributes#Dexterity|dexerity attribute]] score. The check that allows this to be an option for the player will be dependant on the quest or event.
## Discern
*INS*
Additional dialogue option that appears due to the player's [[Attributes#Insight|insight attribute]] score. The check that allows this to be an option for the player will be dependant on the quest or event.