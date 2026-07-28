---
agility: 2
ancestry:
- Abyssal
- Demon
ev: 6 for four minions
file_basename: Grulqin
file_dpath: Monsters/Demons/Statblocks
free_strike: 3
intuition: -1
item_id: grulqin
item_index: '16'
item_name: Grulqin
level: 4
might: 3
presence: -1
reason: -1
roles:
- Minion Brute
scc:
- mcdm.monsters.v1:monster.demons.statblock:grulqin
scdc:
- 1.1.1:2.35.1:16
size: 1L
source: mcdm.monsters.v1
speed: 8
stability: 1
stamina: '9'
type: monster/demons/statblock
---

~~~ds-statblock
type: statblock
name: Grulqin
level: 4
roles:
  - Minion Brute
ancestry:
  - Abyssal
  - Demon
ev: 6 for four minions
stamina: "9"
weaknesses:
  - Holy 5
speed: 8
size: 1L
stability: 1
free_strike: 3
with_captain: +2 damage bonus to strikes
might: 3
agility: 2
reason: -1
intuition: -1
presence: -1
features:
  - type: feature
    feature_type: ability
    name: Spinning Bone Blade
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
      - roll: Power Roll + 3
        tier1: 3 damage
        tier2: 5 damage
        tier3: 7 damage
      - name: Effect
        effect: The grulqin gains an edge on this ability if they previously moved 3 or
          more squares in a straight line on their turn.
  - type: feature
    feature_type: trait
    name: Soulsight
    icon: ⭐️
    effects:
      - effect: Any creature within 2 squares of the grulqin can't be hidden from them.
~~~