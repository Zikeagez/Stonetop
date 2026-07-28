---
agility: 2
ancestry:
- Abyssal
- Demon
ev: 3 for four minions
file_basename: Frenzied
file_dpath: Monsters/Demons/Statblocks
free_strike: 1
intuition: -1
item_id: frenzied
item_index: '22'
item_name: Frenzied
level: 1
might: 0
presence: -1
reason: -1
roles:
- Minion Harrier
scc:
- mcdm.monsters.v1:monster.demons.statblock:frenzied
scdc:
- 1.1.1:2.35.1:22
size: 1M
source: mcdm.monsters.v1
speed: 6
stability: 0
stamina: '4'
type: monster/demons/statblock
---

~~~ds-statblock
type: statblock
name: Frenzied
level: 1
roles:
  - Minion Harrier
ancestry:
  - Abyssal
  - Demon
ev: 3 for four minions
stamina: "4"
weaknesses:
  - Holy 3
speed: 6
size: 1M
stability: 0
free_strike: 1
with_captain: +2 bonus to speed
might: 0
agility: 2
reason: -1
intuition: -1
presence: -1
features:
  - type: feature
    feature_type: ability
    name: Rip and Tear
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
  - type: feature
    feature_type: trait
    name: Soulsight
    icon: ⭐️
    effects:
      - effect: Any creature within 2 squares of the frenzied can't be hidden from them.
~~~