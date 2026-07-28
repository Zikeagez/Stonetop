---
agility: 0
ancestry:
- Human
- Humanoid
ev: '10'
file_basename: Human Storm Mage
file_dpath: Monsters/Humans/Statblocks
free_strike: 5
intuition: 0
item_id: human-storm-mage
item_index: '15'
item_name: Human Storm Mage
level: 3
might: 0
presence: 1
reason: 2
roles:
- Platoon Controller
scc:
- mcdm.monsters.v1:monster.humans.statblock:human-storm-mage
scdc:
- 1.1.1:2.20.1:15
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '40'
type: monster/humans/statblock
---

~~~ds-statblock
type: statblock
name: Human Storm Mage
level: 3
roles:
  - Platoon Controller
ancestry:
  - Human
  - Humanoid
ev: "10"
stamina: "40"
immunities:
  - Corruption 3
  - psychic 3
speed: 5
size: 1M
stability: 0
free_strike: 5
might: 0
agility: 0
reason: 2
intuition: 0
presence: 1
features:
  - type: feature
    feature_type: ability
    name: Lightning Bolt
    icon: 🏹
    ability_type: Signature Ability
    keywords:
      - Magic
      - Ranged
      - Strike
    usage: Main action
    distance: Ranged 15
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        tier1: 7 lightning damage
        tier2: 10 lightning damage
        tier3: 13 lightning damage
      - cost: 5 Malice
        effect: The ability loses the Ranged and Strike keywords, takes the Area
          keyword, and is a 10 x 1 line within 15 that targets each enemy and
          object in the area.
  - type: feature
    feature_type: ability
    name: Gust of Wind
    icon: 🔳
    cost: 3 Malice
    keywords:
      - Area
      - Magic
    usage: Maneuver
    distance: 5 cube within 1
    target: Each enemy and object in the area
    effects:
      - roll: Power Roll + 2
        tier1: Slide 2; M < 0 slowed (save ends)
        tier2: Slide 4; M < 1 slowed (save ends)
        tier3: Slide 6; M < 2 slowed (save ends)
      - name: Effect
        effect: The gust of wind disperses gas or vapor and extinguishes any flames,
          including supernatural effects.
  - type: feature
    feature_type: trait
    name: Arcane Shield
    icon: ⭐️
    effects:
      - effect: >-
          Any melee ability targeting the storm mage takes a bane.


          Additionally, whenever the mage takes damage from an adjacent enemy,
          the enemy takes 2 lightning damage, and if they have R < 1 they are
          pushed up to 2 squares.
  - type: feature
    feature_type: trait
    name: Supernatural Insight
    icon: ⭐️
    effects:
      - effect: The storm mage ignores concealment if it's granted by a supernatural
          effect.
~~~