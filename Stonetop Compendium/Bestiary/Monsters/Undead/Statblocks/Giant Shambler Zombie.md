---
agility: -3
ancestry:
- Undead
- Soulless
ev: 12 for four minions
file_basename: Giant Shambler Zombie
file_dpath: Monsters/Undead/Statblocks
free_strike: 5
intuition: 1
item_id: giant-shambler-zombie
item_index: '17'
item_name: Giant Shambler Zombie
level: 10
might: 5
presence: -2
reason: -3
roles:
- Minion Brute
scc:
- mcdm.monsters.v1:monster.undead.statblock:giant-shambler-zombie
scdc:
- 1.1.1:2.8.1:17
size: '3'
source: mcdm.monsters.v1
speed: 4
stability: 5
stamina: '17'
type: monster/undead/statblock
---

~~~ds-statblock
type: statblock
name: Giant Shambler Zombie
level: 10
roles:
  - Minion Brute
ancestry:
  - Undead
  - Soulless
ev: 12 for four minions
stamina: "17"
immunities:
  - Corruption 10
  - poison 10
speed: 4
size: "3"
stability: 5
free_strike: 5
with_captain: +4 damage bonus to strikes
might: 5
agility: -3
reason: -3
intuition: 1
presence: -2
features:
  - type: feature
    feature_type: ability
    name: Rotten Kick
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 2
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 5
        tier1: 5 damage; push 2
        tier2: 8 damage; push 4
        tier3: 10 damage; push 6
  - type: feature
    feature_type: trait
    name: Meat Shield
    icon: ⭐️
    effects:
      - effect: Each ally adjacent to the shambler has damage immunity 3.
~~~