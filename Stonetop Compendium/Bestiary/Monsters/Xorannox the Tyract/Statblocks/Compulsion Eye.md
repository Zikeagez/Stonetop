---
agility: 1
ancestry:
- Eyestalk
- Horror
- Overmind
ev: '-'
file_basename: Compulsion Eye
file_dpath: Monsters/Xorannox the Tyract/Statblocks
free_strike: 3
intuition: 1
item_id: compulsion-eye
item_index: '03'
item_name: Compulsion Eye
level: 6
might: -1
presence: -1
reason: 4
roles:
- Controller
scc:
- mcdm.monsters.v1:monster.xorannox the tyract.statblock:compulsion-eye
scdc:
- 1.1.1:2.41.1:03
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '30'
type: monster/xorannox the tyract/statblock
---

~~~ds-statblock
type: statblock
name: Compulsion Eye
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
    name: Compulsion Beam
    icon: 🏹
    ability_type: Signature Ability
    keywords:
      - Psionic
      - Ranged
      - Strike
    usage: Main action
    distance: Ranged 6
    target: One creature
    effects:
      - roll: Power Roll + 4
        tier1: I < 2 the target is charmed
        tier2: I < 3 the target is charmed
        tier3: I < 4 the target is charmed
      - name: Effect
        effect: As a free triggered action, a charmed target immediately moves up to
          their speed and can make a free strike against an enemy of Xorannox's
          choice. The target is then no longer charmed.
  - type: feature
    feature_type: trait
    name: Psionic Barrier
    icon: ⭐️
    effects:
      - effect: The compulsion eye has damage immunity 15. When they use a main action,
          they lose this immunity until the end of the round.
~~~