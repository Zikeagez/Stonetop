---
agility: 1
ancestry:
- Humanoid
- Radenwight
ev: 3 for 4 minions
file_basename: Radenwight Scrapper
file_dpath: Monsters/Radenwights/Statblocks
free_strike: 1
intuition: 0
item_id: radenwight-scrapper
item_index: '06'
item_name: Radenwight Scrapper
level: 1
might: -1
presence: 2
reason: 0
roles:
- Minion Defender
scc:
- mcdm.monsters.v1:monster.radenwights.statblock:radenwight-scrapper
scdc:
- 1.1.1:2.19.1:06
size: 1S
source: mcdm.monsters.v1
speed: 5
stability: 1
stamina: '5'
type: monster/radenwights/statblock
---

~~~ds-statblock
type: statblock
name: Radenwight Scrapper
level: 1
roles:
  - Minion Defender
ancestry:
  - Humanoid
  - Radenwight
ev: 3 for 4 minions
stamina: "5"
speed: 5
movement: Climb
size: 1S
stability: 1
free_strike: 1
with_captain: +2 bonus to melee distance
might: -1
agility: 1
reason: 0
intuition: 0
presence: 2
features:
  - type: feature
    feature_type: ability
    name: Buckler Bash
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Charge
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 2
        tier1: 1 damage
        tier2: 2 damage; taunted (EoT)
        tier3: 3 damage; taunted (EoT)
  - type: feature
    feature_type: ability
    name: Ready Rodent
    icon: ❗️
    keywords:
      - Melee
      - Weapon
    usage: Triggered action
    distance: Melee 1
    target: One creature
    trigger: An ally deals damage to the target.
    effects:
      - name: Effect
        effect: The scrapper makes a free strike against the target.
~~~