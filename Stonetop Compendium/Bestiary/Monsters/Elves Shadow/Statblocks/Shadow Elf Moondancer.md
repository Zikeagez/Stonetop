---
agility: 3
ancestry:
- Fey
- Humanoid
- Shadow Elf
ev: '14'
file_basename: Shadow Elf Moondancer
file_dpath: Monsters/Elves Shadow/Statblocks
free_strike: 6
intuition: 2
item_id: shadow-elf-moondancer
item_index: '03'
item_name: Shadow Elf Moondancer
level: 5
might: 1
presence: 0
reason: 1
roles:
- Platoon Harrier
scc:
- mcdm.monsters.v1:monster.elves-shadow.statblock:shadow-elf-moondancer
scdc:
- 1.1.1:2.27.1:03
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 0
stamina: '70'
type: monster/elves-shadow/statblock
---

~~~ds-statblock
type: statblock
name: Shadow Elf Moondancer
level: 5
roles:
  - Platoon Harrier
ancestry:
  - Fey
  - Humanoid
  - Shadow Elf
ev: "14"
stamina: "70"
speed: 7
movement: Climb
size: 1M
stability: 0
free_strike: 6
might: 1
agility: 3
reason: 1
intuition: 2
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Crescent Sweep
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
      - roll: Power Roll + 3
        tier1: 9 damage
        tier2: 13 damage
        tier3: 16 damage
      - name: Effect
        effect: Until the end of the current turn, the moondancer ignores opportunity
          attacks from the target.
  - type: feature
    feature_type: ability
    name: Dissolve
    icon: ❗️
    keywords:
      - Magic
    usage: Triggered action
    distance: Self
    target: Self
    trigger: The moondancer takes damage from a strike.
    effects:
      - name: Effect
        effect: The moondancer can teleport up to 10 squares to a space with concealment
          created by darkness.
  - type: feature
    feature_type: trait
    name: Of the Umbra
    icon: ⭐️
    effects:
      - effect: The moondancer ignores concealment created by darkness. While the
          moondancer is in direct sunlight, they have damage weakness 3. While
          the moondancer has concealment, they have damage immunity 3.
~~~