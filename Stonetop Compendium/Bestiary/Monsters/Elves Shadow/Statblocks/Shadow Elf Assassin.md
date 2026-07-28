---
agility: 3
ancestry:
- Fey
- Humanoid
- Shadow Elf
ev: '16'
file_basename: Shadow Elf Assassin
file_dpath: Monsters/Elves Shadow/Statblocks
free_strike: 7
intuition: 1
item_id: shadow-elf-assassin
item_index: '12'
item_name: Shadow Elf Assassin
level: 6
might: 0
presence: 1
reason: 2
roles:
- Platoon Artillery
scc:
- mcdm.monsters.v1:monster.elves-shadow.statblock:shadow-elf-assassin
scdc:
- 1.1.1:2.27.1:12
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '70'
type: monster/elves-shadow/statblock
---

~~~ds-statblock
type: statblock
name: Shadow Elf Assassin
level: 6
roles:
  - Platoon Artillery
ancestry:
  - Fey
  - Humanoid
  - Shadow Elf
ev: "16"
stamina: "70"
speed: 5
movement: Climb
size: 1M
stability: 0
free_strike: 7
might: 0
agility: 3
reason: 2
intuition: 1
presence: 1
features:
  - type: feature
    feature_type: ability
    name: Lumina Assault
    icon: 🏹
    ability_type: Signature Ability
    keywords:
      - Ranged
      - Strike
      - Weapon
    usage: Main action
    distance: Ranged 15
    target: One creature or object
    effects:
      - roll: Power Roll + 3
        tier1: 10 damage
        tier2: 15 damage
        tier3: 18 damage
      - name: Effect
        effect: The next ability used against the target has a double edge.
      - cost: 5 Malice
        effect: Each non-minion ally within 3 squares of the target can make a free
          strike against them.
  - type: feature
    feature_type: ability
    name: Splitbow
    icon: 🔳
    cost: 2 Malice
    keywords:
      - Area
      - Ranged
      - Weapon
    usage: Main action
    distance: 4 x 1 line within 10
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 3
        tier1: 5 damage; I < 1 bleeding (save ends)
        tier2: 10 damage; I < 2 bleeding (save ends)
        tier3: 12 damage; I < 3 bleeding (save ends)
      - name: Effect
        effect: Each target is pushed up to 4 squares.
  - type: feature
    feature_type: trait
    name: Of the Umbra
    icon: ⭐️
    effects:
      - effect: The assassin ignores concealment created by darkness. While the assassin
          is in direct sunlight, they have damage weakness 3. While the assassin
          has concealment, they have damage immunity 3.
~~~