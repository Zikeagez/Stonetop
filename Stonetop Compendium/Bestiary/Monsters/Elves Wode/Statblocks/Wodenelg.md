---
agility: 1
ancestry:
- Plant
- Wode Elf
ev: '6'
file_basename: Wodenelg
file_dpath: Monsters/Elves Wode/Statblocks
free_strike: 3
intuition: 0
item_id: wodenelg
item_index: '05'
item_name: Wodenelg
level: 1
might: 2
presence: -1
reason: -1
roles:
- Platoon Mount
scc:
- mcdm.monsters.v1:monster.elves-wode.statblock:wodenelg
scdc:
- 1.1.1:2.28.1:05
size: '2'
source: mcdm.monsters.v1
speed: 10
stability: 1
stamina: '30'
type: monster/elves-wode/statblock
---

~~~ds-statblock
type: statblock
name: Wodenelg
level: 1
roles:
  - Platoon Mount
ancestry:
  - Plant
  - Wode Elf
ev: "6"
stamina: "30"
speed: 10
size: "2"
stability: 1
free_strike: 3
might: 2
agility: 1
reason: -1
intuition: 0
presence: -1
features:
  - type: feature
    feature_type: ability
    name: Gore
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Charge
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        tier1: 5 damage
        tier2: 7 damage
        tier3: 9 damage
      - name: Effect
        effect: The wodenelg's rider can make a free strike at any point during the
          charge.
  - type: feature
    feature_type: trait
    name: Sure-Footed
    icon: ⭐️
    effects:
      - effect: The wodenelg ignores difficult terrain and doesn't provoke oppotunity
          attacks by moving.
  - type: feature
    feature_type: ability
    name: Where I End the Woods Begin
    icon: 👤
    cost: 3 Malice
    keywords:
      - "-"
    usage: Maneuver
    distance: Self
    target: Self
    effects:
      - name: Effect
        effect: The wodenelg and their rider become invisible until the start of the
          wodenelg's next turn.
  - type: feature
    feature_type: trait
    name: Mounted Stability
    icon: ⭐️
    effects:
      - effect: The wodenelg's rider has damage immunity 2.
  - type: feature
    feature_type: trait
    name: Shared Glamor
    icon: ⭐️
    effects:
      - effect: If the wodenelg's rider has the Masking Glamor trait, the wodenelg also
          has that trait.
~~~