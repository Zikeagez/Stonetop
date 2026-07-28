---
agility: 1
ancestry:
- Eyestalk
- Horror
- Overmind
ev: '-'
file_basename: Necrotic Eye
file_dpath: Monsters/Xorannox the Tyract/Statblocks
free_strike: 3
intuition: 1
item_id: necrotic-eye
item_index: '07'
item_name: Necrotic Eye
level: 6
might: -1
presence: -1
reason: 4
roles:
- Hexer
scc:
- mcdm.monsters.v1:monster.xorannox the tyract.statblock:necrotic-eye
scdc:
- 1.1.1:2.41.1:07
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '30'
type: monster/xorannox the tyract/statblock
---

~~~ds-statblock
type: statblock
name: Necrotic Eye
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
    name: Necro Beam
    icon: 🏹
    ability_type: Signature Ability
    keywords:
      - Psionic
      - Ranged
      - Strike
    usage: Main action
    distance: Ranged 10
    target: One creature or object
    effects:
      - roll: Power Roll + 4
        tier1: 11 corruption damage
        tier2: 17 corruption damage; M < 3 bleeding (save ends)
        tier3: 20 corruption damage; M < 4 bleeding (save ends)
      - name: Effect
        effect: If this damage or the Stamina loss from bleeding this way reduces a
          target creature's Stamina to 0, that creature dies.
  - type: feature
    feature_type: trait
    name: Psionic Barrier
    icon: ⭐️
    effects:
      - effect: The necrotic eye has damage immunity 15. When they use a main action,
          they lose this immunity until the end of the round.
~~~