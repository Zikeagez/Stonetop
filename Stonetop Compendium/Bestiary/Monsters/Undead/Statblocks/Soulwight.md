---
agility: 1
ancestry:
- Undead
ev: '3'
file_basename: Soulwight
file_dpath: Monsters/Undead/Statblocks
free_strike: 1
intuition: 0
item_id: soulwight
item_index: '16'
item_name: Soulwight
level: 1
might: 2
presence: 1
reason: 0
roles:
- Horde Hexer
scc:
- mcdm.monsters.v1:monster.undead.statblock:soulwight
scdc:
- 1.1.1:2.8.1:16
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '10'
type: monster/undead/statblock
---

~~~ds-statblock
type: statblock
name: Soulwight
level: 1
roles:
  - Horde Hexer
ancestry:
  - Undead
ev: "3"
stamina: "10"
immunities:
  - Corruption 1
  - poison 1
speed: 5
size: 1M
stability: 0
free_strike: 1
might: 2
agility: 1
reason: 0
intuition: 0
presence: 1
features:
  - type: feature
    feature_type: ability
    name: Soulstealer Longsword
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        tier1: 3 corruption damage
        tier2: 4 corruption damage; M < 1 slowed (save ends)
        tier3: 5 corruption damage; M < 2 slowed and weakened (save ends)
      - name: Effect
        effect: The target appears to rapidly age each time they take damage from this
          ability. The target regains their former appearance when the soulwight
          is destroyed.
  - type: feature
    feature_type: ability
    name: Stolen Vitality
    icon: 🏹
    cost: 3 Malice
    keywords:
      - Magic
      - Ranged
    usage: Maneuver
    distance: Ranged 5
    target: One ally
    effects:
      - name: Effect
        effect: The target regains 10 Stamina. The soulwight can't use this maneuver
          again until after they strike a creature with their Soulstealer
          Longsword.
  - type: feature
    feature_type: trait
    name: Arise
    icon: ⭐️
    effects:
      - effect: The first time the soulwight is reduced to 0 Stamina by damage that
          isn't fire damage or holy damage and their body isn't destroyed, they
          instead have 1 Stamina and fall prone.
~~~