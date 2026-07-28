---
agility: 0
ancestry:
- Fey
- High Elf
- Humanoid
ev: '8'
file_basename: High Elf Deathtouch
file_dpath: Monsters/Elves High/Statblocks
free_strike: 5
intuition: 0
item_id: high-elf-deathtouch
item_index: '13'
item_name: High Elf Deathtouch
level: 2
might: 2
presence: 1
reason: 1
roles:
- Platoon Artillery
scc:
- mcdm.monsters.v1:monster.elves-high.statblock:high-elf-deathtouch
scdc:
- 1.1.1:2.14.1:13
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '30'
type: monster/elves-high/statblock
---

~~~ds-statblock
type: statblock
name: High Elf Deathtouch
level: 2
roles:
  - Platoon Artillery
ancestry:
  - Fey
  - High Elf
  - Humanoid
ev: "8"
stamina: "30"
speed: 5
size: 1M
stability: 0
free_strike: 5
might: 2
agility: 0
reason: 1
intuition: 0
presence: 1
features:
  - type: feature
    feature_type: ability
    name: Heartpiercer
    icon: 🏹
    ability_type: Signature Ability
    keywords:
      - Ranged
      - Strike
      - Weapon
    usage: Main action
    distance: Ranged 15
    target: One creature
    effects:
      - roll: Power Roll + 2
        tier1: 7 damage
        tier2: 10 damage
        tier3: 13 damage; R < 1 bleeding (save ends); I < 1 frightened (save ends); P <
          1 restrained (save ends)
      - cost: 5 Malice
        effect: The ability takes the Area keyword and loses the Strike keyword, its
          distance becomes a 3 cube within 10, and it targets each enemy in the
          area.
  - type: feature
    feature_type: ability
    name: Kiss of Death
    icon: 🗡
    keywords:
      - Magic
      - Melee
    usage: Maneuver
    distance: Melee 1
    target: One willing ally
    effects:
      - name: Effect
        effect: The target has a +5 bonus to speed and automatically obtains a tier 3
          outcome on power rolls. They can still roll to determine if they score
          a critical hit. At the end of their next turn, the target immediately
          dies.
  - type: feature
    feature_type: trait
    name: Otherworldly Grace
    icon: ⭐️
    effects:
      - effect: At the start of each of their turns, the deathtouch can choose one
          effect on them that can be ended by a saving throw. That effect
          instead ends at the end of their turn.
~~~