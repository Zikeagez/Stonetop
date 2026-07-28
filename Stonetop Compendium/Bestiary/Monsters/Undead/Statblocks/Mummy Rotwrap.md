---
agility: -2
ancestry:
- Mummy
- Undead
ev: 9 for four minions
file_basename: Mummy Rotwrap
file_dpath: Monsters/Undead/Statblocks
free_strike: 4
intuition: 1
item_id: mummy-rotwrap
item_index: '33'
item_name: Mummy Rotwrap
level: 7
might: 4
presence: -2
reason: -2
roles:
- Minion Brute
scc:
- mcdm.monsters.v1:monster.undead.statblock:mummy-rotwrap
scdc:
- 1.1.1:2.8.1:33
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 1
stamina: '15'
type: monster/undead/statblock
---

~~~ds-statblock
type: statblock
name: Mummy Rotwrap
level: 7
roles:
  - Minion Brute
ancestry:
  - Mummy
  - Undead
ev: 9 for four minions
stamina: "15"
immunities:
  - Corruption 7
  - poison 7
weaknesses:
  - Fire 5
speed: 5
size: 1M
stability: 1
free_strike: 4
with_captain: +3 bonus to melee distance
might: 4
agility: -2
reason: -2
intuition: 1
presence: -2
features:
  - type: feature
    feature_type: ability
    name: Fetid Wrappings
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
      - roll: Power Roll + 4
        tier1: 4 damage
        tier2: 7 damage; pull 1
        tier3: 8 damage; pull 3
      - name: Effect
        effect: Each ally gains an edge on strikes made against the target until the end
          of the round.
~~~