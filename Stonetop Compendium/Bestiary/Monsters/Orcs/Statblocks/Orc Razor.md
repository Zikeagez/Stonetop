---
agility: 1
ancestry:
- Humanoid
- Orc
ev: 3 for four minions
file_basename: Orc Razor
file_dpath: Monsters/Orcs/Statblocks
free_strike: 2
intuition: 0
item_id: orc-razor
item_index: '10'
item_name: Orc Razor
level: 1
might: 2
presence: 0
reason: 0
roles:
- Minion Brute
scc:
- mcdm.monsters.v1:monster.orcs.statblock:orc-razor
scdc:
- 1.1.1:2.16.1:10
size: 1L
source: mcdm.monsters.v1
speed: 6
stability: 0
stamina: '5'
type: monster/orcs/statblock
---

~~~ds-statblock
type: statblock
name: Orc Razor
level: 1
roles:
  - Minion Brute
ancestry:
  - Humanoid
  - Orc
ev: 3 for four minions
stamina: "5"
speed: 6
size: 1L
stability: 0
free_strike: 2
with_captain: +1 damage bonus to strikes
might: 2
agility: 1
reason: 0
intuition: 0
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Boot and Blade
    icon: 🏹
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 2
        tier1: 2 damage
        tier2: 4 damage; push 3
        tier3: 5 damage; push 3 or prone
      - name: Effect
        effect: The razor gains an edge against any target affected by a condition.
  - type: feature
    feature_type: trait
    name: Bloodfire Burn
    icon: ⭐️
    effects:
      - effect: If the razor is reduced to 0 Stamina, they can make a free strike before
          dying.
~~~