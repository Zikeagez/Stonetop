~~~ds-statblock
type: statblock
name: Knight of Blood
level: .
roles:
  - Minion Controller
ancestry:
  - Elemental (Earth, Fire, Rot, Water)
ev: 7 essence for two minions
speed: 6
size: 1L
stamina: 16|16
movement: 
weaknesses:
stability: R
free_strike: 7
might: 4
agility: 2
reason: 0
intuition: 0
presence: 3
features:
  - type: feature
    feature_type: ability
    name: Free Strike Damage Type - Corruption
  - type: feature
    feature_type: trait
    name: ⭐ Scarlet Death
    icon: ⭐️
    effects:
      - effect: The knight's melee strikes inflict `P < STRONG` bleeding (save ends). While bleeding this way, the target can't roll lower than a 3 on the die used to resolve bleeding damage.
  - type: feature
    feature_type: trait
    cost: 2 Essence
    name: ⭐ Red River
    icon: ⭐️
    effects:
      - effect: When the knight is reduced to 0 Stamina, they move up to their speed ignoring opportunity attacks. Each square that they exit during this movement pools with blood until the end of the encounter. Each affected square is considered difficult terrain for enemies and deals 3 corruption damage ot an enemy when they first enter it on a turn. Whenever a bleeding enemy starts their turn within 10 squares of the blood pool, they are pulled 2 toward the nearest affected square, ignoring stability.
~~~


