---
agility: 1
ancestry:
- Human
- Humanoid
ev: 3 for four minions
file_basename: Human Death Acolyte
file_dpath: Monsters/Humans/Statblocks
free_strike: 1
intuition: 0
item_id: human-death-acolyte
item_index: '05'
item_name: Human Death Acolyte
level: 1
might: 0
presence: 2
reason: 0
roles:
- Minion Hexer
scc:
- mcdm.monsters.v1:monster.humans.statblock:human-death-acolyte
scdc:
- 1.1.1:2.20.1:05
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '3'
type: monster/humans/statblock
---

~~~ds-statblock
type: statblock
name: Human Death Acolyte
level: 1
roles:
  - Minion Hexer
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
free_strike: 1
with_captain: +5 bonus to ranged distance
might: 0
agility: 1
reason: 0
intuition: 0
presence: 2
features:
  - type: feature
    feature_type: ability
    name: Necrotic Bolt
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
        tier1: 1 corruption damage
        tier2: 2 corruption damage
        tier3: 3 corruption damage
      - name: Effect
        effect: One creature within 5 squares regains 1 Stamina.
  - type: feature
    feature_type: trait
    name: Supernatural Insight
    icon: ⭐️
    effects:
      - effect: The death acolyte ignores concealment if it's granted by a supernatural
          effect.
~~~