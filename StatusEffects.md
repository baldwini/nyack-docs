- Weapons will give different type of status effects on hit

# Affliction
---
## Broken
*Modular*
- **Cure**: Mend Spell, Doctor non-player characters 
- **Cause**: Done by excessive dealt damage to specific limbs 
#### Effects
- **Head**: -10% HT, -3 INS

- **Ribs**: -30% HT

- **Arm, Left**: -10% HT, -100% Swing Speed Colossal Weapons, -70% Swing Speed Simple Weapons, -40% Swing Speed Light Weapons 

- **Arm, Right**: -10% HT, -100% Swing Speed Colossal Weapons, -70% Swing Speed Simple Weapons, -40% Swing Speed Light Weapons

- **Hand, Left**: -5% HT, -50% Swing Speed Colossal Weapons, -25% Swing Speed Simple Weapons, -20% Swing Speed Light Weapons

- **Hand, Right**: -5% HT, -50% Swing Speed Colossal Weapons, -25% Swing Speed Simple Weapons, -20% Swing Speed Light Weapons

	Two-handed Swing Speed
	(min(Hand Left Swing Speed, Arm Left Swing Speed) + min(Hand Right Swing Speed, Arm Right Swing Speed)) / 2 = Two-handed Swing Speed

- **Leg, Left**: -10% HT, -30% Speed (-60% Total Movement Speed Both Legs)

- **Leg, Right**: -10% HT, -30% Speed (-60% Total Movement Speed Both Legs)

- **Foot, Left**: -5% HT,  -15% Speed (-30% Total Movement Speed Both Feet)

- **Foot, Right**: -5% HT, -15% Speed (-30% Total Movement Speed Both Feet)

	Movement Speed
	( Leg Left + Leg Right + Foot Left + Foot Right ) = Movement Speed Penalty

Effects: (Per Limb)
Head -10% HP, -3 INS

Torso -30% HP

Arm Left -10% HP, -50% Swing Speed Colossal Weapons, -35% Swing Speed Simple Weapons, -30% Swing Speed Light Weapons

Arm Right -10% HP, -50% Swing Speed Colossal Weapons, -35% Swing Speed Simple Weapons, -30% Swing Speed Light Weapons

Leg Left -10% HP, -30% Speed (-60% Total Movement Speed Both Legs)

Leg Right -10% HP, -30% Speed (-60% Total Movement Speed Both Legs)

Foot Left -5% HP,  -15% Speed (-30% Total Movement Speed Both Feet)

Foot Right -5% HP, -15% Speed (-30% Total Movement Speed Both Feet)

Hand Left -5% HP, -50% Swing Speed Colossal Weapons, -25% Swing Speed 
Simple Weapons, -20% Swing Speed Light Weapons (Multiply by 2 for two-handed weapons) 

Hand Right -5% HP, -30% Swing Speed Colossal Weapons, -15% Swing Speed Simple Weapons, -20% Swing Speed Light Weapons (Multiply by 2 for two-handed weapons)

## Sleep Deprivation
*Phases*
	Sleep is required for the player to save the game; camps can be set up by the player to sleep outside towns. Different areas of the game will have protection levels based on distance from obelisk, nearby factions and towns, and the player's reputation with those towns or factions. These factors affect the difficulty of the [[Skills#Survival (INS-4)|Survival]] check, which is made every rest outside, if failed then a random encounter may begin. Failure to sleep will occasionally result in negative side effects for the player, growing based on how long the player hasn't slept.

- **Cure**: Sleeping
- **Cause**: Skipping Sleep

### Phase 1
- **Cause**: Skipping Sleep for 6 days

#### Effects
Hearing voices, irregular sounds, and flashes of lights

### Phase 2
- **Cause**: Skipping Sleep for 8 days

#### Effects
Fake enemies can hunt you, auditory hallucinations worsen, fake surface villagers will walk up to the player for trading (trading will result in the player throwing currency on the ground), Dialogues get scrambled, Fog of war appears, drop items randomly, uses primary items or magic randomly

### Phase 3
- **Cause**: Skipping Sleep for 10 days

#### Effects
Fake encounters may now hurt the player, auditory hallucinations continue, health points drain slowly (20 per day), Fog of war worsens, drop items randomly, uses primary items or magic randomly, dialogues are unreadable

## Starvation
*Phases*
- **Cure**: Eating
- **Cause**: Skipping Rations

### Peckish
- **Cause**: Skipping Rations for 2 days

#### Effects
-1 STR, 

### Hungry
- **Cause**: Skipping Rations for 4 days

#### Effects
-3 STR, -1 DXT

### Starving
- **Cause**: Skipping Rations for 5 days

#### Effects
-5 STR, -3 DXT, Movement becomes unreliable (swapping movement keys),

# Blight
---
## Poison
*Stack-able*
* **Cure**: Spell (unimplemented), acidic consumable, throwing powdery rocks near the player character
* **Cause**: Poison tipped weapons, drinking poison, walking and running into poison flora
#### Characteristics
* **Damage**: X Hit Points
* **Decay**: Number of Hit Points that will remove from the last damage value every time damage occurs
* **Tick**: Every X real-time seconds

	These values allow for different volatilises and duration of poisons.

#### Effect
* **Example**: Say Damage = 12, Decay = 3, Tick = 5 seconds...
	The player will take 12 Hit Points of damage, then 5 seconds later take 12 - 3 = 9 Hit Points of damage, then 5 seconds later take 6, then 3, then the poison has worn off... for a total of 30 damage over 15 seconds...
=======
Effects: (5 Hit point * Immunity) *Rounded Value* loss every 5 real-time seconds
