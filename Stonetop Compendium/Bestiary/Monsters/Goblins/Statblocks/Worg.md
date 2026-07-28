---
agility: 2
ancestry:
- Animal
- Goblin
ev: '3'
file_basename: Worg
file_dpath: Monsters/Goblins/Statblocks
free_strike: 1
intuition: 0
item_id: worg
item_index: '03'
item_name: Worg
level: 1
might: 1
presence: -1
reason: -1
roles:
- Horde Mount
scc:
- mcdm.monsters.v1:monster.goblins.statblock:worg
scdc:
- 1.1.1:2.40.1:03
size: 1L
source: mcdm.monsters.v1
speed: 5
stability: 1
stamina: '15'
type: monster/goblins/statblock
---

~~~ds-statblock
type: statblock
name: Worg
level: 1
roles:
  - Horde Mount
ancestry:
  - Animal
  - Goblin
ev: "3"
stamina: "15"
speed: 5
size: 1L
stability: 1
free_strike: 1
might: 1
agility: 2
reason: -1
intuition: 0
presence: -1
features:
  - type: feature
    feature_type: ability
    name: Bite
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Charge
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        tier1: 3 damage
        tier2: 4 damage
        tier3: 5 damage
  - type: feature
    feature_type: ability
    name: Sprint
    icon: 👤
    cost: 1 Malice
    keywords:
      - "-"
    usage: Maneuver
    distance: Self
    target: Self
    effects:
      - name: Effect
        effect: The worg moves up to their speed.
  - type: feature
    feature_type: trait
    name: Mounted Charger
    icon: ⭐️
    effects:
      - effect: If a worg used as a mount charges, their rider gains an edge on melee
          strikes until the end of the rider's turn.
  - type: feature
    feature_type: trait
    name: Shared Craft
    icon: ⭐️
    effects:
      - effect: If the worg's rider has the Crafty trait, the worg also has that trait.
~~~