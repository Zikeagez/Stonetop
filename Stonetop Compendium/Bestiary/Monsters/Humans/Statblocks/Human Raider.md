---
agility: 2
ancestry:
- Human
- Humanoid
ev: 3 for four minions
file_basename: Human Raider
file_dpath: Monsters/Humans/Statblocks
free_strike: 1
intuition: 0
item_id: human-raider
item_index: '03'
item_name: Human Raider
level: 1
might: 0
presence: 0
reason: 0
roles:
- Minion Harrier
scc:
- mcdm.monsters.v1:monster.humans.statblock:human-raider
scdc:
- 1.1.1:2.20.1:03
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 0
stamina: '4'
type: monster/humans/statblock
---

~~~ds-statblock
type: statblock
name: Human Raider
level: 1
roles:
  - Minion Harrier
ancestry:
  - Human
  - Humanoid
ev: 3 for four minions
stamina: "4"
immunities:
  - Corruption 1
  - psychic 1
speed: 7
size: 1M
stability: 0
free_strike: 1
with_captain: Gain an edge on strikes
might: 0
agility: 2
reason: 0
intuition: 0
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Handaxes
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
        tier2: 2 damage
        tier3: 3 damage
      - name: Effect
        effect: If this ability is used as part of a charge, the raider can make a
          ranged free strike before using the ability.
  - type: feature
    feature_type: trait
    name: Supernatural Insight
    icon: ⭐️
    effects:
      - effect: The raider ignores concealment if it's granted by a supernatural effect.
~~~