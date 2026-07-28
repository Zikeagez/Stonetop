---
agility: 1
ancestry:
- Goblin
- Hobgoblin
- Humanoid
- Infernal
ev: 6 for four minions
file_basename: Hobgoblin Brandbearer
file_dpath: Monsters/Hobgoblins/Statblocks
free_strike: 2
intuition: 0
item_id: hobgoblin-brandbearer
item_index: '11'
item_name: Hobgoblin Brandbearer
level: 4
might: 0
presence: 3
reason: 2
roles:
- Minion Hexer
scc:
- mcdm.monsters.v1:monster.hobgoblins.statblock:hobgoblin-brandbearer
scdc:
- 1.1.1:2.22.1:11
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '7'
type: monster/hobgoblins/statblock
---

~~~ds-statblock
type: statblock
name: Hobgoblin Brandbearer
level: 4
roles:
  - Minion Hexer
ancestry:
  - Goblin
  - Hobgoblin
  - Humanoid
  - Infernal
ev: 6 for four minions
stamina: "7"
immunities:
  - Fire 2
speed: 5
size: 1M
stability: 0
free_strike: 2
with_captain: Gain an edge on strikes
might: 0
agility: 1
reason: 2
intuition: 0
presence: 3
features:
  - type: feature
    feature_type: ability
    name: Searing Grasp
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Magic
      - Melee
      - Strike
    usage: Main action
    distance: Melee 1
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 3
        tier1: 2 fire damage
        tier2: 4 fire damage; M < 2 fire weakness 5 (save ends)
        tier3: 6 fire damage; M < 3 fire weakness 5 (save ends)
  - type: feature
    feature_type: trait
    name: Open Furnace
    icon: ⭐️
    effects:
      - effect: Whenever an enemy takes fire damage, they take 1 extra fire damage for
          each brandbearer adjacent to them.
  - type: feature
    feature_type: trait
    name: Infernal Ichor
    icon: ⭐️
    effects:
      - effect: When the brandbearer is reduced to 0 Stamina, they spray burning blood.
          Each creature adjacent to the brandbearer takes 2 fire damage.
~~~