---
agility: 3
ancestry:
- Fey
- Humanoid
- Shadow Elf
ev: '16'
file_basename: Shadow Elf Mournblade
file_dpath: Monsters/Elves Shadow/Statblocks
free_strike: 7
intuition: 2
item_id: shadow-elf-mournblade
item_index: '14'
item_name: Shadow Elf Mournblade
level: 6
might: 2
presence: 0
reason: 1
roles:
- Platoon Ambusher
scc:
- mcdm.monsters.v1:monster.elves-shadow.statblock:shadow-elf-mournblade
scdc:
- 1.1.1:2.27.1:14
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '80'
type: monster/elves-shadow/statblock
---

~~~ds-statblock
type: statblock
name: Shadow Elf Mournblade
level: 6
roles:
  - Platoon Ambusher
ancestry:
  - Fey
  - Humanoid
  - Shadow Elf
ev: "16"
stamina: "80"
speed: 5
movement: Climb
size: 1M
stability: 0
free_strike: 7
might: 2
agility: 3
reason: 1
intuition: 2
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Knife in the Dark
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
        tier1: 10 damage
        tier2: 15 damage
        tier3: 18 damage
      - name: Effect
        effect: The mournblade is invisible to the target until the start of the
          mournblade's next turn.
  - type: feature
    feature_type: ability
    name: Shadow Step
    icon: 👤
    keywords:
      - Magic
    usage: Maneuver
    distance: Self
    target: Self
    effects:
      - name: Effect
        effect: If the mournblade has concealment, they can teleport up to 10 squares to
          a space with concealment created by darkness.
  - type: feature
    feature_type: trait
    name: Of the Umbra
    icon: ⭐️
    effects:
      - effect: The mournblade ignores concealment created by darkness. While the
          mournblade is in direct sunlight, they have damage weakness 3. While
          the mournblade has concealment, they have damage immunity 3.
~~~