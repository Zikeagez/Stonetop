---
agility: 0
ancestry:
- Human
- Humanoid
ev: 3 for four minions
file_basename: Human Guard
file_dpath: Monsters/Humans/Statblocks
free_strike: 2
intuition: 0
item_id: human-guard
item_index: '14'
item_name: Human Guard
level: 1
might: 2
presence: 0
reason: 0
roles:
- Minion Brute
scc:
- mcdm.monsters.v1:monster.humans.statblock:human-guard
scdc:
- 1.1.1:2.20.1:14
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '5'
type: monster/humans/statblock
---

~~~ds-statblock
type: statblock
name: Human Guard
level: 1
roles:
  - Minion Brute
ancestry:
  - Human
  - Humanoid
ev: 3 for four minions
stamina: "5"
immunities:
  - Corruption 1
  - psychic 1
speed: 5
size: 1M
stability: 0
free_strike: 2
with_captain: +2 bonus to speed
might: 2
agility: 0
reason: 0
intuition: 0
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Halberd
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
      - roll: Power Roll + 2
        tier1: 2 damage
        tier2: 4 damage
        tier3: 5 damage
      - name: Effect
        effect: If the guard is flanked, they can make a free strike against a different
          target adjacent to them.
  - type: feature
    feature_type: trait
    name: Supernatural Insight
    icon: ⭐️
    effects:
      - effect: The guard ignores concealment if it's granted by a supernatural effect.
~~~