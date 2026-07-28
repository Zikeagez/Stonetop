---
agility: 1
ancestry:
- Humanoid
- Soulless
- War Dog
ev: '3'
file_basename: War Dog Neuronite
file_dpath: Monsters/War Dogs/Statblocks
free_strike: 1
intuition: 0
item_id: war-dog-neuronite
item_index: '31'
item_name: War Dog Neuronite
level: 1
might: 0
presence: 2
reason: 0
roles:
- Horde Defender
scc:
- mcdm.monsters.v1:monster.war-dogs.statblock:war-dog-neuronite
scdc:
- 1.1.1:2.51.1:31
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '20'
type: monster/war-dogs/statblock
---

~~~ds-statblock
type: statblock
name: War Dog Neuronite
level: 1
roles:
  - Horde Defender
ancestry:
  - Humanoid
  - Soulless
  - War Dog
ev: "3"
stamina: "20"
immunities:
  - Psychic 2
speed: 5
movement: Fly
size: 1M
stability: 0
free_strike: 1
might: 0
agility: 1
reason: 0
intuition: 0
presence: 2
features:
  - type: feature
    feature_type: ability
    name: Synlirii Grafts
    icon: ❇️
    ability_type: Signature Ability
    keywords:
      - Area
      - Psionic
    usage: Main action
    distance: 1 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 2
        tier1: 1 psychic damage; vertical slide 1
        tier2: 2 psychic damage; vertical slide 2
        tier3: 3 psychic damage; vertical slide 3
  - type: feature
    feature_type: ability
    name: Posthumous Promotion
    icon: 🏹
    keywords:
      - Magic
      - Ranged
    usage: Maneuver
    distance: Ranged 10
    target: One war dog
    effects:
      - name: Effect
        effect: If the target has a loyalty collar, they are reduced to 0 Stamina.
  - type: feature
    feature_type: ability
    name: The Voice
    icon: ❇️
    cost: 1 Malice
    keywords:
      - Area
      - Psionic
    usage: Maneuver
    distance: 5 burst
    target: Each enemy in the area
    effects:
      - name: Effect
        effect: The neuronite chooses one ally within 10 squares. Each target is either
          taunted by the ally, or the ally has damage immunity 3 whenever any
          target makes a strike against them (the neuronite's choice). Either
          effect lasts until the start of the neuronite's next turn.
  - type: feature
    feature_type: trait
    name: Loyalty Collar
    icon: ⭐️
    effects:
      - effect: When the neuronite is reduced to 0 Stamina, their loyalty collar
          explodes, dealing 1d6 damage to each adjacent enemy and object.
~~~