---
agility: 5
ancestry:
- Abyssal
- Demon
ev: 12 for four minions
file_basename: Tyburaki
file_dpath: Monsters/Demons/Statblocks
free_strike: 4
intuition: 3
item_id: tyburaki
item_index: '06'
item_name: Tyburaki
level: 10
might: 2
presence: -1
reason: 0
roles:
- Minion Harrier
scc:
- mcdm.monsters.v1:monster.demons.statblock:tyburaki
scdc:
- 1.1.1:2.35.1:06
size: '2'
source: mcdm.monsters.v1
speed: 8
stability: 0
stamina: '15'
type: monster/demons/statblock
---

~~~ds-statblock
type: statblock
name: Tyburaki
level: 10
roles:
  - Minion Harrier
ancestry:
  - Abyssal
  - Demon
ev: 12 for four minions
stamina: "15"
weaknesses:
  - Holy 5
speed: 8
movement: Swim
size: "2"
stability: 0
free_strike: 4
with_captain: +4 damage bonus to strikes
might: 2
agility: 5
reason: 0
intuition: 3
presence: -1
features:
  - type: feature
    feature_type: ability
    name: Tail Bite
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 3
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 5
        tier1: 4 damage
        tier2: 7 damage
        tier3: 9 damage
      - name: Effect
        effect: The tyburaki can make a free strike against each enemy adjacent to the
          target.
  - type: feature
    feature_type: trait
    name: Breacher
    icon: ⭐️
    effects:
      - effect: While swimming, the tyburaki can jump 5 squares as part of their
          movement.
  - type: feature
    feature_type: trait
    name: Soulsight
    icon: ⭐️
    effects:
      - effect: Any creature within 2 squares of the tyburaki can't be hidden from them.
~~~