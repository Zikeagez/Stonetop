---
agility: 0
ancestry:
- Humanoid
- Time Raider
ev: '10'
file_basename: Time Raider Mind Punk
file_dpath: Monsters/Time Raiders/Statblocks
free_strike: 5
intuition: 2
item_id: time-raider-mind-punk
item_index: '10'
item_name: Time Raider Mind Punk
level: 3
might: 2
presence: 1
reason: 2
roles:
- Platoon Hexer
scc:
- mcdm.monsters.v1:monster.time-raiders.statblock:time-raider-mind-punk
scdc:
- 1.1.1:2.18.1:10
size: '2'
source: mcdm.monsters.v1
speed: 5
stability: 2
stamina: '40'
type: monster/time-raiders/statblock
---

~~~ds-statblock
type: statblock
name: Time Raider Mind Punk
level: 3
roles:
  - Platoon Hexer
ancestry:
  - Humanoid
  - Time Raider
ev: "10"
stamina: "40"
immunities:
  - Psychic 3
speed: 5
size: "2"
stability: 2
free_strike: 5
might: 2
agility: 0
reason: 2
intuition: 2
presence: 1
features:
  - type: feature
    feature_type: ability
    name: Repelling Psihander
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Psionic
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: Two creatures adjacent to each other
    effects:
      - roll: Power Roll + 2
        tier1: 6 damage
        tier2: 8 damage; M < 1 dazed (save ends)
        tier3: 11 damage; M < 2 dazed (save ends)
      - name: Effect
        effect: A target who ends their next turn adjacent to the other target falls
          prone.
  - type: feature
    feature_type: ability
    name: Mindpunk
    icon: ❇️
    cost: 2 Malice
    keywords:
      - Area
      - Psionic
    usage: Main action
    distance: 3 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 2
        tier1: 4 psychic damage; R < 0 prone
        tier2: 6 psychic damage; push 1; R < 1 prone and can't stand (save ends)
        tier3: 9 psychic damage; push 2; R < 2 prone and can't stand (save ends)
  - type: feature
    feature_type: trait
    name: Foresight
    icon: ⭐️
    effects:
      - effect: The mind punk doesn't take a bane on strikes against creatures with
          concealment.
~~~