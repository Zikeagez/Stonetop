---
agility: 0
ancestry:
- Humanoid
- Rival
ev: '40'
file_basename: Rival Conduit
file_dpath: Monsters/Rivals/3rd Echelon/Statblocks
free_strike: 8
intuition: 4
item_id: rival-conduit
item_index: '04'
item_name: Rival Conduit
level: 8
might: 3
presence: 2
reason: 1
roles:
- Elite Support
scc:
- mcdm.monsters.v1:monster.rivals.3rd echelon.statblock:rival-conduit
scdc:
- 1.1.1:2.5.3.1:04
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 1
stamina: '200'
type: monster/rivals/3rd echelon/statblock
---

~~~ds-statblock
type: statblock
name: Rival Conduit
level: 8
roles:
  - Elite Support
ancestry:
  - Humanoid
  - Rival
ev: "40"
stamina: "200"
speed: 5
size: 1M
stability: 1
free_strike: 8
might: 3
agility: 0
reason: 1
intuition: 4
presence: 2
features:
  - type: feature
    feature_type: ability
    name: Celestial Furor
    icon: ⚔️
    ability_type: Signature Ability
    keywords:
      - Magic
      - Melee
      - Ranged
      - Strike
    usage: Main action
    distance: Melee 1 or ranged 10
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 4
        tier1: 12 holy damage; vertical slide 2
        tier2: 17 holy damage; vertical slide 3
        tier3: 21 holy damage; vertical slide 4
      - name: Effect
        effect: The conduit or one ally within distance regains Stamina equal to half
          the damage dealt.
  - type: feature
    feature_type: ability
    name: Imbue with Power
    icon: 🏹
    cost: 3 Malice
    keywords:
      - Magic
      - Ranged
    usage: Maneuver
    distance: Ranged 10
    target: Self and five allies
    effects:
      - name: Effect
        effect: Each target has a double edge on their next strike.
  - type: feature
    feature_type: trait
    name: Unwavering Defender
    icon: ⭐️
    effects:
      - effect: Damage dealt to any ally adjacent to the conduit is halved.
  - type: feature
    feature_type: trait
    name: Rivalry
    icon: ⭐️
    effects:
      - effect: At the start of an encounter, the conduit chooses one creature within
          their line of effect. Both the conduit and the creature can add a d3
          roll to power rolls they make against each other.
~~~