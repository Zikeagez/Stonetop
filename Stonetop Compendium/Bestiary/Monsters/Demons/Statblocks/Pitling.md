---
agility: 2
ancestry:
- Abyssal
- Demon
ev: 3 for four minions
file_basename: Pitling
file_dpath: Monsters/Demons/Statblocks
free_strike: 2
intuition: -2
item_id: pitling
item_index: '03'
item_name: Pitling
level: 1
might: -2
presence: -2
reason: -2
roles:
- Minion Artillery
scc:
- mcdm.monsters.v1:monster.demons.statblock:pitling
scdc:
- 1.1.1:2.35.1:03
size: 1T
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '3'
type: monster/demons/statblock
---

~~~ds-statblock
type: statblock
name: Pitling
level: 1
roles:
  - Minion Artillery
ancestry:
  - Abyssal
  - Demon
ev: 3 for four minions
stamina: "3"
weaknesses:
  - Holy 3
speed: 5
movement: Fly
size: 1T
stability: 0
free_strike: 2
with_captain: +2 bonus to speed
might: -2
agility: 2
reason: -2
intuition: -2
presence: -2
features:
  - type: feature
    feature_type: ability
    name: Spit
    icon: 🏹
    ability_type: Signature Ability
    keywords:
      - Ranged
      - Strike
      - Weapon
    usage: Main action
    distance: Ranged 10
    target: One creature per minion
    effects:
      - roll: Power Roll + 2
        tier1: 2 poison damage
        tier2: 4 poison damage
        tier3: 5 poison damage
  - type: feature
    feature_type: trait
    name: Horrid Stench
    icon: ⭐️
    effects:
      - effect: Any enemy who has three or more pitlings within 2 squares of them can't
          regain Stamina.
  - type: feature
    feature_type: trait
    name: Soulsight
    icon: ⭐️
    effects:
      - effect: Any creature within 2 squares of the pitling can't be hidden from them.
~~~