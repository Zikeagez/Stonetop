---
agility: 3
ancestry:
- Fey
- Humanoid
- Shadow Elf
ev: 6 for four minions
file_basename: Shadow Elf Sniper
file_dpath: Monsters/Elves Shadow/Statblocks
free_strike: 3
intuition: 0
item_id: shadow-elf-sniper
item_index: '10'
item_name: Shadow Elf Sniper
level: 4
might: 1
presence: 0
reason: 0
roles:
- Minion Artillery
scc:
- mcdm.monsters.v1:monster.elves-shadow.statblock:shadow-elf-sniper
scdc:
- 1.1.1:2.27.1:10
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '7'
type: monster/elves-shadow/statblock
---

~~~ds-statblock
type: statblock
name: Shadow Elf Sniper
level: 4
roles:
  - Minion Artillery
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
free_strike: 3
with_captain: +2 damage bonus to strikes
might: 1
agility: 3
reason: 0
intuition: 0
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Lumina Arrow
    icon: 🏹
    ability_type: Signature Ability
    keywords:
      - Ranged
      - Strike
      - Weapon
    usage: Main action
    distance: Ranged 7
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 3
        tier1: 3 damage
        tier2: 5 damage
        tier3: 7 damage
      - name: Effect
        effect: The next strike made against the target gains an edge.
  - type: feature
    feature_type: trait
    name: Of the Umbra
    icon: ⭐️
    effects:
      - effect: The sniper ignores concealment created by darkness. While the sniper is
          in direct sunlight, they have damage weakness 3. While the sniper has
          concealment, they have damage immunity 3.
~~~