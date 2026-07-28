---
agility: 3
ancestry:
- Soulless
- War Dog
ev: '6'
file_basename: War Dog Equivite
file_dpath: Monsters/War Dogs/Statblocks
free_strike: 3
intuition: -2
item_id: war-dog-equivite
item_index: '12'
item_name: War Dog Equivite
level: 4
might: 3
presence: 0
reason: -1
roles:
- Horde Brute
scc:
- mcdm.monsters.v1:monster.war-dogs.statblock:war-dog-equivite
scdc:
- 1.1.1:2.51.1:12
size: '2'
source: mcdm.monsters.v1
speed: 8
stability: 2
stamina: '53'
type: monster/war-dogs/statblock
---

~~~ds-statblock
type: statblock
name: War Dog Equivite
level: 4
roles:
  - Horde Brute
ancestry:
  - Soulless
  - War Dog
ev: "6"
stamina: "53"
speed: 8
size: "2"
stability: 2
free_strike: 3
might: 3
agility: 3
reason: -1
intuition: -2
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Fuse-Iron Lance
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Charge
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 2
    target: One creature or object
    effects:
      - roll: Power Roll + 3
        tier1: 6 damage
        tier2: 8 damage
        tier3: 10 damage; I < 3 frightened (save ends)
      - name: Effect
        effect: This ability gains an edge while charging.
      - cost: 2 Malice
        effect: The ability deals an extra 3 fire damage to the target and each enemy
          adjacent to the target.
  - type: feature
    feature_type: ability
    name: Blazing Charge
    icon: 🗡
    keywords:
      - Melee
      - Weapon
    usage: Maneuver
    distance: Special; see below
    target: Special
    effects:
      - name: Effect
        effect: The equivite moves up to their speed and ignores difficult terrain. Any
          mundane size 1 object whose space they move through is destroyed. The
          equivite makes one power roll against each enemy whose space they move
          through for the first time.
      - roll: Power Roll + 3
        tier1: 2 damage; push 1
        tier2: 4 damage; push 2
        tier3: 5 damage; push 3; M < 3 prone
  - type: feature
    feature_type: trait
    name: Loyalty Collar
    icon: ⭐️
    effects:
      - effect: When the equivite is reduced to 0 Stamina, their loyalty collar
          explodes, dealing 2d6 damage to each adjacent enemy and object.
~~~