---
agility: 2
ancestry:
- Animal
- Orc
ev: 3 for four minions
file_basename: Mohler
file_dpath: Monsters/Orcs/Statblocks
free_strike: 2
intuition: 1
item_id: mohler
item_index: '01'
item_name: Mohler
level: 1
might: 0
presence: -3
reason: -4
roles:
- Minion Ambusher
scc:
- mcdm.monsters.v1:monster.orcs.statblock:mohler
scdc:
- 1.1.1:2.16.1:01
size: 1S
source: mcdm.monsters.v1
speed: 7
stability: 1
stamina: '4'
type: monster/orcs/statblock
---

~~~ds-statblock
type: statblock
name: Mohler
level: 1
roles:
  - Minion Ambusher
ancestry:
  - Animal
  - Orc
ev: 3 for four minions
stamina: "4"
speed: 7
movement: Burrow
size: 1S
stability: 1
free_strike: 2
with_captain: +2 bonus to speed
might: 0
agility: 2
reason: -4
intuition: 1
presence: -3
features:
  - type: feature
    feature_type: ability
    name: Earth Bump
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 2
        tier1: 2 damage
        tier2: 4 damage
        tier3: 5 damage
      - name: Effect
        effect: The distance increases to melee 2. If the mohler is 1 or more squares
          beneath the target before they use this ability, a target who has M <
          1 is also knocked prone.
  - type: feature
    feature_type: trait
    name: Seismic Sense
    icon: ⭐️
    effects:
      - effect: The mohler doesn't need line of effect to use abilities against
          creatures or objects touching the ground.
  - type: feature
    feature_type: trait
    name: Ground Grinder
    icon: ⭐️
    effects:
      - effect: The mohler can use the Dig maneuver at the start of the encounter.
          Additionally, while the mohler burrows within 1 square below the
          ground, the ground above where they burrow is difficult terrain.
~~~