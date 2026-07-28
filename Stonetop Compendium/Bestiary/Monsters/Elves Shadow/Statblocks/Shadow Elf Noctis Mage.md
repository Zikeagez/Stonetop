---
agility: 2
ancestry:
- Fey
- Humanoid
- Shadow Elf
ev: '16'
file_basename: Shadow Elf Noctis Mage
file_dpath: Monsters/Elves Shadow/Statblocks
free_strike: 6
intuition: 1
item_id: shadow-elf-noctis-mage
item_index: '13'
item_name: Shadow Elf Noctis Mage
level: 6
might: 0
presence: 1
reason: 3
roles:
- Platoon Hexer
scc:
- mcdm.monsters.v1:monster.elves-shadow.statblock:shadow-elf-noctis-mage
scdc:
- 1.1.1:2.27.1:13
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '70'
type: monster/elves-shadow/statblock
---

~~~ds-statblock
type: statblock
name: Shadow Elf Noctis Mage
level: 6
roles:
  - Platoon Hexer
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
free_strike: 6
might: 0
agility: 2
reason: 3
intuition: 1
presence: 1
features:
  - type: feature
    feature_type: ability
    name: Blotting Bolt
    icon: 🏹
    ability_type: Signature Ability
    keywords:
      - Magic
      - Ranged
      - Strike
    usage: Main action
    distance: Ranged 5
    target: One creature or object
    effects:
      - roll: Power Roll + 3
        tier1: 9 damage
        tier2: 14 damage
        tier3: 17 damage
      - name: Effect
        effect: The target takes a bane on their next strike.
      - cost: 3 Malice
        effect: The target instead has a double bane on the next ability they use.
  - type: feature
    feature_type: ability
    name: Enemies in the Dark
    icon: 🏹
    cost: 3 Malice
    keywords:
      - Magic
      - Ranged
      - Strike
    usage: Main action
    distance: Ranged 5
    target: Two enemies
    effects:
      - roll: Power Roll + 3
        tier1: 8 damage; R < 1 the target makes a free strike against one enemy of the
          noctis mage's choice.
        tier2: 10 damage; R < 2 the target makes a free strike against one enemy of the
          noctis mage's choice.
        tier3: 13 damage; R < 3 the target uses a signature ability against one enemy of
          the noctis mage's choice.
  - type: feature
    feature_type: trait
    name: Of the Umbra
    icon: ⭐️
    effects:
      - effect: The noctis mage ignores concealment created by darkness. While the
          noctis mage is in direct sunlight, they have damage weakness 3. While
          the noctis mage has concealment, they have damage immunity 3.
~~~