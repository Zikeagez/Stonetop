---
agility: 2
ancestry:
- Angulotl
ev: 3 for 4 minions
file_basename: Angulotl Pollywog
file_dpath: Monsters/Angulotls/Statblocks
free_strike: 1
intuition: -2
item_id: angulotl-pollywog
item_index: '05'
item_name: Angulotl Pollywog
level: 1
might: 0
presence: 0
reason: -2
roles:
- Minion Harrier
scc:
- mcdm.monsters.v1:monster.angulotls.statblock:angulotl-pollywog
scdc:
- 1.1.1:2.31.1:05
size: 1S
source: mcdm.monsters.v1
speed: 6
stability: 0
stamina: '4'
type: monster/angulotls/statblock
---

~~~ds-statblock
type: statblock
name: Angulotl Pollywog
level: 1
roles:
  - Minion Harrier
ancestry:
  - Angulotl
ev: 3 for 4 minions
stamina: "4"
immunities:
  - Poison 2
speed: 6
movement: Climb, swim
size: 1S
stability: 0
free_strike: 1
with_captain: +2 bonus to speed
might: 0
agility: 2
reason: -2
intuition: -2
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Nip
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: One creature per minion
    effects:
      - roll: Power Roll + 2
        tier1: 1 poison damage
        tier2: 2 poison damage; the pollywog can shift 1 square
        tier3: 3 poison damage; the pollywog shifts up to 3 squares
  - type: feature
    feature_type: trait
    name: Quick Snack
    icon: ⭐️
    effects:
      - effect: Any angulotl who can target the pollywog with a melee free strike can
          eat them as a maneuver. The angulotl regains 4 Stamina and is wet
          until the end of their next turn.
~~~