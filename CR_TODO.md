

## New gameplay style

The goal is to finish the final boss with a minimum of days.
A day pass when the player go to sleep at the Inn or at any other PNJ house that accept it.
For this to work, all the HP and mana restoration mechanisms will be removed, or dramatically changed.
The player will absolutely need to go to the town to restore HP and mana.

As a side-effect, the game will be both more challenging and less boring, because no one will have
an inventory full of potion, and finally the HP and mana capacity will be useful.

Also using the right spell at the right moment will be crucial.
Since less spell will be used, most spell will be upgraded to provide interesting edge during the battle.



## Bugfix improvements:

- [DONE] Fix the Flash spell bug



## Basic improvements:

- [DONE] Sleeping in town to restore health and mana
	- [DONE] The tavern/inn provide the basic restoration
	- [DONE] Pepin cost much but always provide full restoration
	- [DONE] Farnham is gratis but is hazardous
	- Gillian is a bit better than the tavern/inn, is gratis, but only available under certain condition
- Remove all potions, or change their use-case dramatically (e.g. provide better restoration when sleeping)
- Remove Level Up full restoration (eventually keeping a bit of bonus)
- Improve all spell efficiency (since mana have to be saved most of time)
- [DONE] Totally redo mana shield:
	- Each spell level provide one point of damage reduction
	- Only redirect 30% of damage to mana at spell level 1, the more the level, the more damage is redirected
	- Anyway, only a portion of the total mana can be used, making big damage dealer still efficient
	- As a result, mana shield is less powerful, but it is finally meaningful to gain better spell level
- Change Flash spell:
	- beside the spell "normal" cost, it will always eat 1/4 to 1/3 of remaining mana
	- damage are proportional to mana used, improved by spell-level
	- the damage per mana used should be low, much lower than any other spell
	- but the damage per spell should be the higher
	- basically, we waste a lot of mana to deal the maximum damage in the minimum of time
	- it should be used as an emergency spell, when we are closed to be killed
	- it should also knock back every target
	- it would be useful in conjunction with the new/less OP mana shield, since there should always be
	  some damage dealt to HP
- Improve Flame Wave: should be harder to block
- Make scroll more useful: check the spell-level of scroll spell, maybe taking into consideration the player
  actual spell-level if any
- Rebalance staves with charges (too powerful in the new mechanics)



## Medium improvements:

- Maybe: add a regen/bleeding/poison mechanism? 
	- so the healing spell would have some usefulness
	- the regen should be capped, or the whole “number of day to defeat the final boss” becomes useless
	- maybe implement some kind of “ghost” max hp, each time damages are received, the ghost max hp drop
	  and no healing can restore above that ghost value, only sleeping in town can raise that ghost value



## Greater improvements:

- Add some kind of necromantic spell: summoning squeleton ally (should be inspired by Golem):
	- Possibility to have at most one squeleton per spell-level at the same time
	- The squeleton spawn can be any of the cathedral squeleton, the higher the spell-level,
	  the higher the chance to summon a higher level squeleton
- Add a movespeed mechanism:
	- the rogue has +10% by default
	- items like heavy armor (i.e. better armors than hard leather armors) have a movespeed penalty
	- some magical items have bonus/curse on movespeed
	- maybe add a run skill, that uses mana for a temporary +50% movespeed boost



## Exceptional/improbable improvements:

- Tristram is attacked by Leoric and its squeleton army

