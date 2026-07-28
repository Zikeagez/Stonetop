---
agility: 3
ancestry:
- Abyssal
- Demon
ev: 6 for four minions
file_basename: Orliq
file_dpath: Monsters/Demons/Statblocks
free_strike: 2
intuition: 0
item_id: orliq
item_index: '21'
item_name: Orliq
level: 4
might: -1
presence: -1
reason: 1
roles:
- Minion Harrier
scc:
- mcdm.monsters.v1:monster.demons.statblock:orliq
scdc:
- 1.1.1:2.35.1:21
size: 1T
source: mcdm.monsters.v1
speed: 6
stability: 0
stamina: '8'
type: monster/demons/statblock
---

~~~ds-statblock
type: statblock
name: Orliq
level: 4
roles:
  - Minion Harrier
ancestry:
  - Abyssal
  - Demon
ev: 6 for four minions
stamina: "8"
weaknesses:
  - Holy 5
speed: 6
movement: Fly
size: 1T
stability: 0
free_strike: 2
with_captain: +2 bonus to speed
might: -1
agility: 3
reason: 1
intuition: 0
presence: -1
features:
  - type: feature
    feature_type: ability
    name: Soul Prism
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Magic
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 3
        tier1: 2 corruption damage; slide 2
        tier2: 4 corruption damage; vertical slide 2
        tier3: 6 corruption damage; vertical slide 2
  - type: feature
    feature_type: trait
    name: Imposing Energy
    icon: ⭐️
    effects:
      - effect: Any enemy who starts their turn with two or more orliq adjacent to them
          is slowed (EoT).
  - type: feature
    feature_type: trait
    name: Soulsight
    icon: ⭐️
    effects:
      - effect: Any creature within 2 squares of the orliq can't be hidden from them.
~~~