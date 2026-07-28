---
agility: 1
ancestry:
- Eyestalk
- Horror
- Overmind
ev: '-'
file_basename: Mover Eye
file_dpath: Monsters/Xorannox the Tyract/Statblocks
free_strike: 3
intuition: 1
item_id: mover-eye
item_index: '02'
item_name: Mover Eye
level: 6
might: -1
presence: -1
reason: 4
roles:
- Controller
scc:
- mcdm.monsters.v1:monster.xorannox the tyract.statblock:mover-eye
scdc:
- 1.1.1:2.41.1:02
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '30'
type: monster/xorannox the tyract/statblock
---

~~~ds-statblock
type: statblock
name: Mover Eye
level: 6
roles:
  - Controller
ancestry:
  - Eyestalk
  - Horror
  - Overmind
ev: "-"
stamina: "30"
speed: 5
movement: Fly, hover
size: 1M
stability: 0
free_strike: 3
might: -1
agility: 1
reason: 4
intuition: 1
presence: -1
features:
  - type: feature
    feature_type: ability
    name: Telekinetic Beam
    icon: 🏹
    ability_type: Signature Ability
    keywords:
      - Psionic
      - Ranged
      - Strike
    usage: Main action
    distance: Ranged 6
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 4
        tier1: 11 damage; slide 4
        tier2: 17 damage; slide 5
        tier3: 20 damage; slide 6
  - type: feature
    feature_type: trait
    name: Psionic Barrier
    icon: ⭐️
    effects:
      - effect: The mover eye has damage immunity 15. When they use a main action, they
          lose this immunity until the end of the round.
~~~