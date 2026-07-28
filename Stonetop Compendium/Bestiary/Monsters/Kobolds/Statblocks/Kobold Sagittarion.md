---
agility: 2
ancestry:
- Humanoid
- Kobold
ev: 3 for four minions
file_basename: Kobold Sagittarion
file_dpath: Monsters/Kobolds/Statblocks
free_strike: 2
intuition: 0
item_id: kobold-sagittarion
item_index: '12'
item_name: Kobold Sagittarion
level: 1
might: 0
presence: 0
reason: 0
roles:
- Minion Artillery
scc:
- mcdm.monsters.v1:monster.kobolds.statblock:kobold-sagittarion
scdc:
- 1.1.1:2.10.1:12
size: 1S
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '3'
type: monster/kobolds/statblock
---

~~~ds-statblock
type: statblock
name: Kobold Sagittarion
level: 1
roles:
  - Minion Artillery
ancestry:
  - Humanoid
  - Kobold
ev: 3 for four minions
stamina: "3"
speed: 5
size: 1S
stability: 0
free_strike: 2
with_captain: +5 bonus to ranged distance
might: 0
agility: 2
reason: 0
intuition: 0
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Composite Bow
    icon: 🏹
    ability_type: Signature Ability
    keywords:
      - Ranged
      - Strike
      - Weapon
    usage: Main action
    distance: Ranged 10
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 2
        tier1: 2 damage
        tier2: 4 damage
        tier3: 5 damage
      - name: Effect
        effect: While adjacent to any ally, the sagittarion gains an edge on this
          ability.
  - type: feature
    feature_type: trait
    name: Shield? Shield!
    icon: ⭐️
    effects:
      - effect: While adjacent to an ally who also has this trait, the sagittarion has
          stability 1, has cover, and grants cover to allies.
~~~