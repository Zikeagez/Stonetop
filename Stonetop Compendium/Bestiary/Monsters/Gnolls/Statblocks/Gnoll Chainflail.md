---
agility: 0
ancestry:
- Abyssal
- Gnoll
ev: 4 for four minions
file_basename: Gnoll Chainflail
file_dpath: Monsters/Gnolls/Statblocks
free_strike: 3
intuition: 0
item_id: gnoll-chainflail
item_index: '04'
item_name: Gnoll Chainflail
level: 2
might: 2
presence: -2
reason: 1
roles:
- Minion Artillery
scc:
- mcdm.monsters.v1:monster.gnolls.statblock:gnoll-chainflail
scdc:
- 1.1.1:2.6.1:04
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 1
stamina: '4'
type: monster/gnolls/statblock
---

~~~ds-statblock
type: statblock
name: Gnoll Chainflail
level: 2
roles:
  - Minion Artillery
ancestry:
  - Abyssal
  - Gnoll
ev: 4 for four minions
stamina: "4"
speed: 5
size: 1M
stability: 1
free_strike: 3
with_captain: +1 damage bonus to strikes
might: 2
agility: 0
reason: 1
intuition: 0
presence: -2
features:
  - type: feature
    feature_type: ability
    name: Chain Shotput
    icon: 🏹
    ability_type: Signature Ability
    keywords:
      - Ranged
      - Strike
      - Weapon
    usage: Main action
    distance: Ranged 8
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 2
        tier1: 3 damage
        tier2: 4 damage; push 1
        tier3: 6 damage; push 3
  - type: feature
    feature_type: trait
    name: Death Circle
    icon: ⭐️
    effects:
      - effect: Whenever a non-minion ally within 5 squares of the chainflail is reduced
          to 0 Stamina, the chainflail can move up to their speed.
~~~