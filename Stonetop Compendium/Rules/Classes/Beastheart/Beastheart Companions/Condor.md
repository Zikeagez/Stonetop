

~~~ds-statblock
type: statblock
name: Condor
level:  
roles:
  - Companion
ancestry:
  - Animal
  - Companion
speed: 7
size: 1M
stability: 0
free_strike: 1+M
might: 2
agility: 1
reason: -1
intuition: 2
presence: 1
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
    name: 🗡️ Flurry of Wings
    icon: 🗡️
    usage: Maneuver
    keywords:
      - Companion
      - Melee
      - Weapon
    distance: 📐 Melee 1
    target: 🎯One creature or object
    effects:
      - name: Description
        effect: _I can't draw a bead on them with that infernal bird flapping in my face!_
      - name: Effect
        effect: The target takes damage equal to 3 + the condor's Might score. Additionally, enemies are weakened while adjacent to the condor until the end of your next turn.
      - name: Spend 1 Ferocity
        effect: An enemy who would be weakened by this ability is taunted instead.
  - type: feature
    feature_type: trait
    name: ⭐️ Moving Target
    icon: ⭐️
    effects:
      - effect: While the boar is flying and has a speed greater than 0, ranged strikes against them take a bane.


~~~

> **Level 3 Condor Advancement Feature**
> ⭐**Dive Bomb**
>Whenever the condor makes a strike while rampaging, they deal extra damage equal to the number of squares they've moved on their turn (to a maximum of 5).


>**Level 6 Condor Advancement Feature**
>⭐**Borne Aloft**
>While the condor is rampaging, you gain wings and can fly. While flying, you gain a +2 bonus to speed. If you are midair when the condor's rampage ends, you take no damage from the fall.

> **Level 10 Condor Advancement Feature**
> ⭐**Flight of the Condor**
>While the condor is rampaging, you and the condor gain a +5 bonus to speed.


