

## New gameplay style

The goal is to finish the final boss with a minimum of days.
A day pass when the player go to sleep at the Inn or at any other PNJ house that accept it.
For this to work, all the HP and mana restoration mechanisms will be removed, or dramatically changed.
The player will absolutely need to go to the town to restore HP and mana.

As a side-effect, the game will be both more challenging and less boring, because no one will have
an inventory full of potion, and finally the HP and mana capacity will be useful.

Also using the right spell at the right moment will be crucial.
Since less spell will be used, most spell will be upgraded to provide interesting edge during the battle.

It is possible to make the game in a way it is not a good idea to clear the level, but instead just go for
the quest objective and then get the next stairs.



## Bugfix improvements:

- [DONE] Fix the Flash spell bug



## Basic improvements:

- [DONE] Sleeping in town to restore health and mana
	- [DONE] The tavern/inn provide the basic restoration for 80 gold
	- [DONE] Pepin cost much but always provide full restoration for 150 gold
	- [DONE] Farnham is gratis but is hazardous, and can even lower high status because he make you drink all the night
	- Gillian is a bit better than the tavern/inn, is gratis, but only available under certain condition,
	  once you gain her favor
- Remove all potions, or change their use-case dramatically (e.g. provide better restoration when sleeping)
- Remove Level Up full restoration (eventually keeping a bit of bonus)
- Attribute mechanics changes:
	- Remove all player level usage, instead use the correct player attribute everywhere
	- On level up, make the warrior use less points to upgrade strength, sorcerer use less points to upgrade magic,
	  rogue use less points to upgrade dexterity
	- Spell strength should only depend on magic attribute and spell level:
		- usually brute force should depends more on the magic attribute
		- mana used should depends on spell level
		- more subtle things should depends on spell level (it's more skills than brute magic force), e.g. the time
		  a spell is active, the number of missile spawned
		- things that need to scale should depends on the magic attribute
- Fighting mechanics:
	- Chance to hit use dexterity, as well as chance to evade/block
	- Armor class is used as damage reduction instead of raising evasion, heavy armor may even lower evasion,
	  by lowering dexterity
	- So: dexterity should not enhance armor class anymore
	- Warrior has a bonus of evasion/block and CTH in melee (like a sort of hidden skill)
	- Rogue has a bonus of CTH with a bow (like a sort of hidden skill)
	- damage calculation must change, strength should not add to the weapon damage, but instead should multiply it,
	  so cutting weapon (e.g. 1-10) should be more random than club/hammer (5-9), also a warrior with a dagger should
	  not deal much damages
- Item enhancement:
	- The main idea is to allow different strategy, with no cutting clear best equipment
	- Heavy armor provide great damage reduction (absolute? rate? a mix of both?) but at the cost of dexterity
	  and movespeed, so it is not a net positive to have the best AC full plate armor
	- Robe should have better magical properties for the sorcerer (better chance to have magic bonus? improve spell level?)
	- Cape should have better properties for the rogue (not defined right now, could be fun to add concealment to the game)
	- make staves more useful
	- Life/mana stealing items becomes more useful in this gameplay, they do not need buff or nerf, just keep them
	  the way they are
- Improve all spell efficiency (since mana have to be saved most of time)
- [DONE] Totally redo mana shield:
	- Each spell level provide one point of damage reduction
	- Only redirect 30% of damage to mana at spell level 1, the more the level, the more damage is redirected
	- Anyway, only a portion of the total mana can be used, making big damage dealer still efficient
	- As a result, mana shield is less powerful, but it is finally meaningful to gain better spell level
- Flash spell changes:
	- beside the spell "normal" cost, it will always eat 1/4 to 1/3 of remaining mana
	- damage are proportional to mana used, improved by spell-level
	- the damage per mana used should be low, much lower than any other spell
	- but the damage per spell should be the higher
	- basically, we waste a lot of mana to deal the maximum damage in the minimum of time
	- it should be used as an emergency spell, when we are closed to be killed
	- it should also knock back every target
	- it would be useful in conjunction with the new/less OP mana shield, since there should always be
	  some damage dealt to HP
- Stone curse changes:
	- Increase the time of the curse
	- Magic resistance reduce the time of the curse
	- The monster gain some armor class instead of losing some
	- Could be used on multiplayer on an ally who is surrounded by monsters to buy some time (because of the AC boost)
- Improve Flame Wave: should be harder to block/evade, should eventually becomes the ultimate fire spell
  (except apocalypse, but it is not learnable)
- Make scroll more useful: check the spell-level of scroll spell, maybe taking into consideration the player
  actual spell-level if any
- Rebalance staves with charges (too powerful in the new mechanics)
- Monsters:
	- Unique monsters should be buffed, they are way too weak ATM, and they are too rare
	- Buff the Butcher, Leoric, and most quest monsters
- Controls:
	- More hotkeys for spells
	- A phasing spell hotkey that cast the spell immediately without changing the active spell, also maybe another
	  hotkey for teleport?
- Difficulty:
	- Allow difficulty setting in singleplayer



## Medium improvements:

- Map changes:
	- Less chest, but with better quality equipment, placed in room rather than open-space, and could be well guarded,
	  so it could provide some goal (part of the "do not clear the level but cherry-pick your action")
- Maybe: add a regen/bleeding/poison mechanism? 
	- so the healing spell would have some usefulness
	- the regen should be capped, or the whole “number of day to defeat the final boss” becomes useless
	- maybe implement some kind of “ghost” max hp, each time damages are received, the ghost max hp drop
	  and no healing can restore above that ghost value, only sleeping in town can raise that ghost value



## Greater improvements:

- Add a movespeed mechanic:
	- the rogue has +10% by default
	- items like heavy armor (i.e. better armors than hard leather armors) have a movespeed penalty
	- some magical items have bonus/curse on movespeed
	- maybe add a run skill, that uses mana for a temporary +50% movespeed boost
- Add hit speed mechanic:
	- dagger and light sword should be able to hit faster
	- hammer, two-handed sword and big axes should hit slower (but could have significant damage buff)
	- items like heavy armor (i.e. better armors than hard leather armors) have a hit speed penalty
	- some magical items have bonus/curse on hit speed
- Add some kind of necromantic spell: summoning squeleton ally (should be inspired by Golem):
	- Possibility to have at most one squeleton per spell-level at the same time
	- The squeleton spawn can be any of the cathedral squeleton, the higher the spell-level,
	  the higher the chance to summon a higher level squeleton
- Add the hellfire's berserk spell?
- Add a static discharge spell like in D2?
- Add a shield charge skill (like a spell) to the warrior that knock back and stun?
- Add an axe skill (like a spell) to the warrior that chop two or three adjacent monster at the same time?
- Add a defense shield stance (like a spell) to the warrior that improve defense but make him stand still
  (good for tanking team-play, if one day the mod is available on multiplayer), the defence bonus will only
  apply to the 3 front directions
- A concealment/assassin gameplay, allowing rogue to sneak past monsters, or eventually backstab them with a dagger
- Add a sort of ninja smoke bomb (like a spell) to the rogue? it would blind monster and allow to fly away,
  or in teamplay allow some good combo



## Exceptional/improbable improvements:

- Tristram is attacked by Leoric and its squeleton army

