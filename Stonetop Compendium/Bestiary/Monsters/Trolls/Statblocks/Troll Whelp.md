---
agility: 1
ancestry:
- Giant
- Troll
ev: 7 for four minions
file_basename: Troll Whelp
file_dpath: Monsters/Trolls/Statblocks
free_strike: 3
intuition: 0
item_id: troll-whelp
item_index: '02'
item_name: Troll Whelp
level: 5
might: 3
presence: 0
reason: -1
roles:
- Minion Brute
scc:
- mcdm.monsters.v1:monster.trolls.statblock:troll-whelp
scdc:
- 1.1.1:2.53.1:02
size: 1L
source: mcdm.monsters.v1
speed: 6
stability: 3
stamina: '10'
type: monster/trolls/statblock
---

~~~ds-statblock
type: statblock
name: Troll Whelp
level: 5
roles:
  - Minion Brute
ancestry:
  - Giant
  - Troll
ev: 7 for four minions
stamina: "10"
weaknesses:
  - Acid 5
  - fire
speed: 6
size: 1L
stability: 3
free_strike: 3
with_captain: +2 damage bonus to strikes
might: 3
agility: 1
reason: -1
intuition: 0
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Jaws and Claws
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 3
        tier1: 3 damage
        tier2: 6 damage; slide 1
        tier3: 7 damage; slide 2; M < 2 bleeding (save ends)
  - type: feature
    feature_type: trait
    name: Lingering Hunger
    icon: ⭐️
    effects:
      - effect: Whenever two or more whelps are simultaneously reduced to 0 Stamina by
          damage that isn't acid or fire damage, half of those whelps become
          troll limbjumbles with 4 Stamina.
~~~