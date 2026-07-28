
~~~ds-statblock
type: statblock
name: Basilisk
level:  
roles:
  - Companion
ancestry:
  - Beast
  - Companion
immunities:
  - Poison 3
speed: 5
size: 1L
stability: 2
free_strike: 1+M
might: 2
agility: 1
reason: -1
intuition: 2
presence: 2
features:
  - type: feature
    feature_type: trait
    name: Skills
    icon: 🗡
    effects:
      - name: 
        effect: Alertness
  - type: feature
    feature_type: ability
    name: 🗡️🏹 Petrify
    icon: 🗡️🏹
    usage: Maneuver
    keywords:
      - Companion
      - Magic
      - Ranged
      - Weapon
    distance: Melee 1 or ranged 5
    target: 🎯One enemy
    effects:
      - name: Description
        effect: _Transfixed by the basilisk's magical gaze or struck by their poisoned claws, the foe's body begins to calcify._
      - name: Effect
        effect: The target takes corruption damage equal to 3 + the basilisk's Might score and is stoned (save ends (see **Stoned**)).
  - type: feature
    feature_type: trait
    name: ⭐️ Stoned
    icon: ⭐️
    effects:
      - effect: A stoned creature is magically turning to stone. Each time a creature fails the saving throw to end this effect, they take corruption damage equal to the basilisk's Might score. A stoned creature or a creature adjacent to them can use a maneuver to cut the encroaching stone from the stoned target's body, ending the effect and dealing damage to the target equal to twice the basilisk's Might score that can't be reduced in any way. A creature reduced to 0 Stamina while they are stoned, or by an ability that causes a creature to become stoned, is turned to stone until they are restored to life by magical means.


~~~


> **Level 3 Basilisk Advancement Feature**
> ⭐**Foes Forever Frozen**
> Whenever the basilisk makes a strike against a creature while rampaging, the target is stoned (save ends).


>**Level 6 Basilisk Advancement Feature**
>⭐**Rock Smasher**
>Whenever you deal rolled damage to a stoned creature while the basilisk is rampaging, you deal extra damage equal to twice your Might score.

> **Level 10 Basilisk Advancement Feature**
> ⭐**Heart of Stone**
> While the basilisk is rampaging, you and the basilisk have damage immunity 10 as you become nearly impervious living statues.


"\"Your companion lunges into the fray, attacking wildly with teeth, claws, or other weapons.\""