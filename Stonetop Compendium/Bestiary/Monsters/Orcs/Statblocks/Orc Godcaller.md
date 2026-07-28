---
agility: 0
ancestry:
- Humanoid
- Orc
ev: '6'
file_basename: Orc Godcaller
file_dpath: Monsters/Orcs/Statblocks
free_strike: 3
intuition: 1
item_id: orc-godcaller
item_index: '05'
item_name: Orc Godcaller
level: 1
might: 1
presence: 2
reason: 0
roles:
- Platoon Support
scc:
- mcdm.monsters.v1:monster.orcs.statblock:orc-godcaller
scdc:
- 1.1.1:2.16.1:05
size: 1M
source: mcdm.monsters.v1
speed: 6
stability: 0
stamina: '30'
type: monster/orcs/statblock
---

~~~ds-statblock
type: statblock
name: Orc Godcaller
level: 1
roles:
  - Platoon Support
ancestry:
  - Humanoid
  - Orc
ev: "6"
stamina: "30"
speed: 6
size: 1M
stability: 0
free_strike: 3
might: 1
agility: 0
reason: 0
intuition: 1
presence: 2
features:
  - type: feature
    feature_type: ability
    name: Power Chord
    icon: ⚔️
    ability_type: Signature Ability
    keywords:
      - Magic
      - Melee
      - Ranged
      - Strike
    usage: Main action
    distance: Melee 1 or ranged 10
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        tier1: 5 sonic damage
        tier2: 7 sonic damage
        tier3: 9 sonic damage; P < 2 weakened (save ends)
  - type: feature
    feature_type: ability
    name: Cadenza
    icon: 🏹
    keywords:
      - Magic
      - Ranged
    usage: Main action
    distance: Ranged 10
    target: One ally
    effects:
      - name: Effect
        effect: The target moves up to their speed and can use a main action.
      - cost: 3 Malice
        effect: The godcaller targets a second ally.
  - type: feature
    feature_type: ability
    name: Rallying Ostinato
    icon: 🏹
    cost: 2 Malice
    keywords:
      - Magic
      - Ranged
    usage: Maneuver
    distance: Ranged 10
    target: Self and three allies
    effects:
      - name: Effect
        effect: Each target regains 15 Stamina and ignores difficult terrain until the
          end of the encounter.
  - type: feature
    feature_type: trait
    name: Relentless
    icon: ⭐️
    effects:
      - effect: If the godcaller is reduced to 0 Stamina, they can make a free strike
          before dying. If the target of the free strike is reduced to 0
          Stamina, the godcaller is reduced to 1 Stamina instead.
~~~