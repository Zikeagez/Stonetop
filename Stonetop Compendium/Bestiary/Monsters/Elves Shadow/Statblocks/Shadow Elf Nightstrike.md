---
agility: 3
ancestry:
- Fey
- Humanoid
- Shadow Elf
ev: 6 for four minions
file_basename: Shadow Elf Nightstrike
file_dpath: Monsters/Elves Shadow/Statblocks
free_strike: 3
intuition: 1
item_id: shadow-elf-nightstrike
item_index: 08
item_name: Shadow Elf Nightstrike
level: 4
might: 1
presence: 0
reason: 0
roles:
- Minion Ambusher
scc:
- mcdm.monsters.v1:monster.elves-shadow.statblock:shadow-elf-nightstrike
scdc:
- 1.1.1:2.27.1:08
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '8'
type: monster/elves-shadow/statblock
---

~~~ds-statblock
type: statblock
name: Shadow Elf Nightstrike
level: 4
roles:
  - Minion Ambusher
ancestry:
  - Fey
  - Humanoid
  - Shadow Elf
ev: 6 for four minions
stamina: "8"
speed: 5
movement: Climb
size: 1M
stability: 0
free_strike: 3
with_captain: Gain an edge on strikes
might: 1
agility: 3
reason: 0
intuition: 1
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Vault
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 2
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 3
        tier1: 3 damage
        tier2: 5 damage
        tier3: 7 damage
      - name: Effect
        effect: The nightstrike shifts to leap over the target and into an unoccupied
          space adjacent to the target, opposite from the nightstrike's original
          space.
  - type: feature
    feature_type: trait
    name: Of the Umbra
    icon: ⭐️
    effects:
      - effect: The nightstrike ignores concealment created by darkness. While the
          nightstrike is in direct sunlight, they have damage weakness 3. While
          the nightstrike has concealment, they have damage immunity 3.
~~~