---
agility: 2
ancestry:
- Human
- Humanoid
ev: '6'
file_basename: Human Trickshot
file_dpath: Monsters/Humans/Statblocks
free_strike: 4
intuition: 1
item_id: human-trickshot
item_index: '04'
item_name: Human Trickshot
level: 1
might: 0
presence: 0
reason: 0
roles:
- Platoon Artillery
scc:
- mcdm.monsters.v1:monster.humans.statblock:human-trickshot
scdc:
- 1.1.1:2.20.1:04
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '20'
type: monster/humans/statblock
---

~~~ds-statblock
type: statblock
name: Human Trickshot
level: 1
roles:
  - Platoon Artillery
ancestry:
  - Human
  - Humanoid
ev: "6"
stamina: "20"
immunities:
  - Corruption 1
  - psychic 1
speed: 5
size: 1M
stability: 0
free_strike: 4
might: 0
agility: 2
reason: 0
intuition: 1
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Trick Crossbow
    icon: ⚔️
    ability_type: Signature Ability
    keywords:
      - Melee
      - Ranged
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1 or ranged 15
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        tier1: 6 damage
        tier2: 9 damage
        tier3: 12 damage
      - name: Effect
        effect: This ability ignores cover and concealment.
      - cost: 3 Malice
        effect: This ability targets one additional target.
  - type: feature
    feature_type: trait
    name: Supernatural Insight
    icon: ⭐️
    effects:
      - effect: The trickshot ignores concealment if it's granted by a supernatural
          effect.
~~~