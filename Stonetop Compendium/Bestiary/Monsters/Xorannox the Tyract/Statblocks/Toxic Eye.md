---
agility: 1
ancestry:
- Eyestalk
- Horror
- Overmind
ev: '-'
file_basename: Toxic Eye
file_dpath: Monsters/Xorannox the Tyract/Statblocks
free_strike: 3
intuition: 1
item_id: toxic-eye
item_index: '05'
item_name: Toxic Eye
level: 6
might: -1
presence: -1
reason: 4
roles:
- Hexer
scc:
- mcdm.monsters.v1:monster.xorannox the tyract.statblock:toxic-eye
scdc:
- 1.1.1:2.41.1:05
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '30'
type: monster/xorannox the tyract/statblock
---

~~~ds-statblock
type: statblock
name: Toxic Eye
level: 6
roles:
  - Hexer
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
    name: Toxic Vapors
    icon: 🔳
    ability_type: Signature Ability
    keywords:
      - Area
      - Psionic
      - Ranged
    usage: Main action
    distance: 4 cube within 10
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 4
        tier1: 6 poison damage
        tier2: 10 poison damage; M < 3 weakened (save ends)
        tier3: 13 poison damage; M < 4 weakened (save ends)
  - type: feature
    feature_type: trait
    name: Psionic Barrier
    icon: ⭐️
    effects:
      - effect: The toxic eye has damage immunity 15. When they use a main action, they
          lose this immunity until the end of the round.
~~~