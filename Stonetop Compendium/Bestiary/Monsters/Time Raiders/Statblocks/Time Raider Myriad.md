---
agility: 1
ancestry:
- Humanoid
- Time Raider
ev: 5 for four minions
file_basename: Time Raider Myriad
file_dpath: Monsters/Time Raiders/Statblocks
free_strike: 3
intuition: 1
item_id: time-raider-myriad
item_index: '06'
item_name: Time Raider Myriad
level: 3
might: 2
presence: 1
reason: 2
roles:
- Minion Brute
scc:
- mcdm.monsters.v1:monster.time-raiders.statblock:time-raider-myriad
scdc:
- 1.1.1:2.18.1:06
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '8'
type: monster/time-raiders/statblock
---

~~~ds-statblock
type: statblock
name: Time Raider Myriad
level: 3
roles:
  - Minion Brute
ancestry:
  - Humanoid
  - Time Raider
ev: 5 for four minions
stamina: "8"
immunities:
  - Psychic 3
speed: 5
size: 1M
stability: 0
free_strike: 3
with_captain: +1 damage bonus to strikes
might: 2
agility: 1
reason: 2
intuition: 1
presence: 1
features:
  - type: feature
    feature_type: ability
    name: Fifth Fist
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Psionic
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 2
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 2
        tier1: 3 damage; slide 1
        tier2: 5 damage; slide 2
        tier3: 6 damage; slide 3, prone
  - type: feature
    feature_type: trait
    name: Foresight
    icon: ⭐️
    effects:
      - effect: The myriad doesn't take a bane on strikes against creatures with
          concealment.
~~~