---
agility: 3
ancestry:
- Fey
- Humanoid
- Shadow Elf
ev: '14'
file_basename: Shadow Elf Duskcaller
file_dpath: Monsters/Elves Shadow/Statblocks
free_strike: 6
intuition: 2
item_id: shadow-elf-duskcaller
item_index: '07'
item_name: Shadow Elf Duskcaller
level: 5
might: 0
presence: 1
reason: 3
roles:
- Platoon Controller
scc:
- mcdm.monsters.v1:monster.elves-shadow.statblock:shadow-elf-duskcaller
scdc:
- 1.1.1:2.27.1:07
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '60'
type: monster/elves-shadow/statblock
---

~~~ds-statblock
type: statblock
name: Shadow Elf Duskcaller
level: 5
roles:
  - Platoon Controller
ancestry:
  - Fey
  - Humanoid
  - Shadow Elf
ev: "14"
stamina: "60"
speed: 5
movement: Climb
size: 1M
stability: 0
free_strike: 6
might: 0
agility: 3
reason: 3
intuition: 2
presence: 1
features:
  - type: feature
    feature_type: ability
    name: Night Knife
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
        tier3: 16 damage
      - name: Effect
        effect: If the duskcaller has concealment, they can target one additional
          creature or object.
  - type: feature
    feature_type: ability
    name: The Lay of Cor'thoroth
    icon: 🔳
    keywords:
      - Area
      - Magic
      - Ranged
    usage: Maneuver
    distance: 2 cube within 3
    target: Special
    effects:
      - name: Effect
        effect: Until the start of the duskcaller's next turn, the area is filled with
          darkness.
      - cost: 2 Malice
        effect: The size of the cube increases by 3.
  - type: feature
    feature_type: trait
    name: Of the Umbra
    icon: ⭐️
    effects:
      - effect: The duskcaller ignores concealment created by darkness. While the
          duskcaller is in direct sunlight, they have damage weakness 3. While
          the duskcaller has concealment, they have damage immunity 3.
~~~