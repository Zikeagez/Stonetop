---
agility: 0
ancestry:
- Human
- Humanoid
ev: '8'
file_basename: Human Knave
file_dpath: Monsters/Humans/Statblocks
free_strike: 4
intuition: 0
item_id: human-knave
item_index: '02'
item_name: Human Knave
level: 2
might: 2
presence: 0
reason: 1
roles:
- Platoon Defender
scc:
- mcdm.monsters.v1:monster.humans.statblock:human-knave
scdc:
- 1.1.1:2.20.1:02
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '50'
type: monster/humans/statblock
---

~~~ds-statblock
type: statblock
name: Human Knave
level: 2
roles:
  - Platoon Defender
ancestry:
  - Human
  - Humanoid
ev: "8"
stamina: "50"
immunities:
  - Corruption 2
  - psychic 2
speed: 5
size: 1M
stability: 0
free_strike: 4
might: 2
agility: 0
reason: 1
intuition: 0
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Morningstar and Javelin
    icon: ⚔️
    ability_type: Signature Ability
    keywords:
      - Melee
      - Ranged
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1 or ranged 5
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        tier1: 6 damage
        tier2: 9 damage
        tier3: 12 damage; M < 2 the target has a double bane on their next power roll
      - name: Effect
        effect: The target is taunted (EoT).
  - type: feature
    feature_type: trait
    name: I'm Your Enemy
    icon: ⭐️
    effects:
      - effect: Whenever an adjacent creature the knave has taunted deals damage to a
          creature other than the knave, the knave can make a free strike
          against them.
  - type: feature
    feature_type: trait
    name: Overwhelm
    icon: ⭐️
    effects:
      - effect: An enemy who starts their turn adjacent to the knave can't shift.
  - type: feature
    feature_type: trait
    name: Supernatural Insight
    icon: ⭐️
    effects:
      - effect: The knave ignores concealment if it's granted by a supernatural effect.
~~~