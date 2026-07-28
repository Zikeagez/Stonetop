---
agility: 2
ancestry:
- Human
- Humanoid
ev: 3 for four minions
file_basename: Human Archer
file_dpath: Monsters/Humans/Statblocks
free_strike: 2
intuition: 0
item_id: human-archer
item_index: '13'
item_name: Human Archer
level: 1
might: 0
presence: 0
reason: 0
roles:
- Minion Artillery
scc:
- mcdm.monsters.v1:monster.humans.statblock:human-archer
scdc:
- 1.1.1:2.20.1:13
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '3'
type: monster/humans/statblock
---

~~~ds-statblock
type: statblock
name: Human Archer
level: 1
roles:
  - Minion Artillery
ancestry:
  - Human
  - Humanoid
ev: 3 for four minions
stamina: "3"
immunities:
  - Corruption 1
  - psychic 1
speed: 5
size: 1M
stability: 0
free_strike: 2
with_captain: +5 bonus to ranged distance
might: 0
agility: 2
reason: 0
intuition: 0
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Crossbow
    icon: 🏹
    ability_type: Signature Ability
    keywords:
      - Ranged
      - Strike
      - Weapon
    usage: Main action
    distance: Ranged 10
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 2
        tier1: 2 damage
        tier2: 4 damage
        tier3: 5 damage
  - type: feature
    feature_type: trait
    name: Supernatural Insight
    icon: ⭐️
    effects:
      - effect: The archer ignores concealment if it's granted by a supernatural effect.
~~~