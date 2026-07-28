---
agility: 0
ancestry:
- Dwarf
- Humanoid
ev: '8'
file_basename: Dwarf Warden
file_dpath: Monsters/Dwarves/Statblocks
free_strike: 5
intuition: 1
item_id: dwarf-warden
item_index: '06'
item_name: Dwarf Warden
level: 2
might: 2
presence: 0
reason: 0
roles:
- Platoon Brute
scc:
- mcdm.monsters.v1:monster.dwarves.statblock:dwarf-warden
scdc:
- 1.1.1:2.52.1:06
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 3
stamina: '59'
type: monster/dwarves/statblock
---

~~~ds-statblock
type: statblock
name: Dwarf Warden
level: 2
roles:
  - Platoon Brute
ancestry:
  - Dwarf
  - Humanoid
ev: "8"
stamina: "59"
speed: 5
size: 1M
stability: 3
free_strike: 5
might: 2
agility: 0
reason: 0
intuition: 1
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Concussive Maul
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
        tier1: 7 damage; push 1
        tier2: 10 damage; push 3
        tier3: 13 damage; push 5; M < 2 restrained (save ends)
      - name: Effect
        effect: A target restrained by a dwarf can be force moved by this ability. This
          forced movement doesn't end the restrained condition unless the
          Director determines otherwise.
  - type: feature
    feature_type: ability
    name: Concussive Shockwave
    icon: 🔳
    cost: 5 Malice
    keywords:
      - Area
      - Weapon
    usage: Main action
    distance: 3 cube within 1
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 2
        tier1: 5 damage; push 2; A < 0 slowed (save ends)
        tier2: 8 damage; push 2; A < 1 slowed (save ends)
        tier3: 11 damage; push 2; A < 2 slowed (save ends)
      - name: Effect
        effect: A target restrained by a dwarf can be force moved by this ability. This
          forced movement doesn't end the restrained condition unless the
          Director determines otherwise.
  - type: feature
    feature_type: trait
    name: Escort the Prisoners
    icon: ⭐️
    effects:
      - effect: Whenever the warden moves, they can carry an adjacent restrained enemy
          as if the enemy were grabbed by them.
~~~