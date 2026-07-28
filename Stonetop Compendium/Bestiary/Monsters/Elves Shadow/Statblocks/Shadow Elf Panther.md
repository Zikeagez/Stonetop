---
agility: 2
ancestry:
- Fey
- Humanoid
- Shadow Elf
ev: '12'
file_basename: Shadow Elf Panther
file_dpath: Monsters/Elves Shadow/Statblocks
free_strike: 6
intuition: 1
item_id: shadow-elf-panther
item_index: 09
item_name: Shadow Elf Panther
level: 4
might: 3
presence: 1
reason: -1
roles:
- Platoon Brute
scc:
- mcdm.monsters.v1:monster.elves-shadow.statblock:shadow-elf-panther
scdc:
- 1.1.1:2.27.1:09
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '70'
type: monster/elves-shadow/statblock
---

~~~ds-statblock
type: statblock
name: Shadow Elf Panther
level: 4
roles:
  - Platoon Brute
ancestry:
  - Fey
  - Humanoid
  - Shadow Elf
ev: "12"
stamina: "70"
speed: 5
movement: Climb
size: 1M
stability: 0
free_strike: 6
might: 3
agility: 2
reason: -1
intuition: 1
presence: 1
features:
  - type: feature
    feature_type: ability
    name: Dusk Cleave
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
      - roll: Power Roll + 3
        tier1: 9 damage
        tier2: 13 damage
        tier3: 16 damage; I < 3 bleeding (save ends)
      - name: Effect
        effect: The panther can make a free strike against a creature or object adjacent
          to the target.
  - type: feature
    feature_type: ability
    name: Bladestorm
    icon: ❇️
    cost: 3 Malice
    keywords:
      - Area
      - Weapon
    usage: Main action
    distance: 2 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 3
        tier1: 5 corruption damage
        tier2: 8 corruption damage; I < 2 dazed (save ends)
        tier3: 10 corruption damage; I < 3 dazed (save ends)
      - name: Effect
        effect: The panther has a double edge on strikes against targets dazed this way.
  - type: feature
    feature_type: trait
    name: Of the Umbra
    icon: ⭐️
    effects:
      - effect: The panther ignores concealment created by darkness. While the panther
          is in direct sunlight, they have damage weakness 3. While the panther
          has concealment, they have damage immunity 3.
~~~