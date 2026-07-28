---
agility: 3
ancestry:
- Fey
- Humanoid
- Shadow Elf
ev: 6 for four minions
file_basename: Shadow Elf Dusk Mage
file_dpath: Monsters/Elves Shadow/Statblocks
free_strike: 2
intuition: 0
item_id: shadow-elf-dusk-mage
item_index: '01'
item_name: Shadow Elf Dusk Mage
level: 4
might: 0
presence: 0
reason: 2
roles:
- Minion Hexer
scc:
- mcdm.monsters.v1:monster.elves-shadow.statblock:shadow-elf-dusk-mage
scdc:
- 1.1.1:2.27.1:01
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '7'
type: monster/elves-shadow/statblock
---

~~~ds-statblock
type: statblock
name: Shadow Elf Dusk Mage
level: 4
roles:
  - Minion Hexer
ancestry:
  - Fey
  - Humanoid
  - Shadow Elf
ev: 6 for four minions
stamina: "7"
speed: 5
movement: Climb
size: 1M
stability: 0
free_strike: 2
with_captain: Gain an edge on strikes
might: 0
agility: 3
reason: 2
intuition: 0
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Gloom Bolt
    icon: 🏹
    ability_type: Signature Ability
    keywords:
      - Magic
      - Ranged
      - Strike
    usage: Main action
    distance: Ranged 5
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 3
        tier1: 2 damage
        tier2: 4 damage; A < 2 slowed (save ends)
        tier3: 6 damage; A < 3 slowed (save ends)
  - type: feature
    feature_type: trait
    name: Of the Umbra
    icon: ⭐️
    effects:
      - effect: The dusk mage ignores concealment created by darkness. While the dusk
          mage is in direct sunlight, they have damage weakness 3. While the
          dusk mage has concealment, they have damage immunity 3.
~~~