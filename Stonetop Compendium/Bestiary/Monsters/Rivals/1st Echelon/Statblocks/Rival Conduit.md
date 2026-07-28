---
agility: 0
ancestry:
- Humanoid
- Rival
ev: '16'
file_basename: Rival Conduit
file_dpath: Monsters/Rivals/1st Echelon/Statblocks
free_strike: 5
intuition: 2
item_id: rival-conduit
item_index: '04'
item_name: Rival Conduit
level: 2
might: 1
presence: 0
reason: 0
roles:
- Elite Support
scc:
- mcdm.monsters.v1:monster.rivals.1st echelon.statblock:rival-conduit
scdc:
- 1.1.1:2.5.1.1:04
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 1
stamina: '80'
type: monster/rivals/1st echelon/statblock
---

~~~ds-statblock
type: statblock
name: Rival Conduit
level: 2
roles:
  - Elite Support
ancestry:
  - Humanoid
  - Rival
ev: "16"
stamina: "80"
speed: 5
size: 1M
stability: 1
free_strike: 5
might: 1
agility: 0
reason: 0
intuition: 2
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Thunder of Heavens
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
      - roll: Power Roll + 2
        tier1: 7 holy damage
        tier2: 10 holy damage
        tier3: 13 holy damage
      - name: Effect
        effect: The conduit or one ally within distance regains Stamina equal to half
          the damage dealt.
  - type: feature
    feature_type: ability
    name: Imbue with Might
    icon: 🏹
    cost: 2 Malice
    keywords:
      - Magic
      - Ranged
    usage: Maneuver
    distance: Ranged 10
    target: Self and five allies
    effects:
      - name: Effect
        effect: Each target gains an edge on their next strike.
  - type: feature
    feature_type: trait
    name: Stalwart Guardian
    icon: ⭐️
    effects:
      - effect: Strikes made against allies adjacent to the conduit take a bane.
  - type: feature
    feature_type: trait
    name: Rivalry
    icon: ⭐️
    effects:
      - effect: At the start of an encounter, the conduit chooses one creature within
          their line of effect. Both the conduit and the creature can add a d3
          roll to power rolls they make against each other.
~~~