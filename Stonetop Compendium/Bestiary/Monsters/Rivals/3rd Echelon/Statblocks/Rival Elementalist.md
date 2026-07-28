---
agility: 2
ancestry:
- Humanoid
- Rival
ev: '40'
file_basename: Rival Elementalist
file_dpath: Monsters/Rivals/3rd Echelon/Statblocks
free_strike: 8
intuition: 3
item_id: rival-elementalist
item_index: '03'
item_name: Rival Elementalist
level: 8
might: 0
presence: 0
reason: 4
roles:
- Elite Controller
scc:
- mcdm.monsters.v1:monster.rivals.3rd echelon.statblock:rival-elementalist
scdc:
- 1.1.1:2.5.3.1:03
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 1
stamina: '180'
type: monster/rivals/3rd echelon/statblock
---

~~~ds-statblock
type: statblock
name: Rival Elementalist
level: 8
roles:
  - Elite Controller
ancestry:
  - Humanoid
  - Rival
ev: "40"
stamina: "180"
speed: 5
size: 1M
stability: 1
free_strike: 8
might: 0
agility: 2
reason: 4
intuition: 3
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Verdant Rains
    icon: 🏹
    ability_type: Signature Ability
    keywords:
      - Green
      - Magic
      - Ranged
      - Strike
    usage: Main action
    distance: Ranged 10
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 4
        tier1: 12 damage; slide 2; M < 2 4 acid damage
        tier2: 17 damage; slide 3; M < 3 6 acid damage
        tier3: 21 damage; slide 4; M < 4 8 acid damage
      - name: Effect
        effect: One ally within distance ends one condition on themself.
  - type: feature
    feature_type: ability
    name: The Chasm Engulfs
    icon: 🔳
    cost: 4 Malice
    keywords:
      - Area
      - Green
      - Magic
      - Ranged
    usage: Main action
    distance: 5 cube within 10
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 4
        tier1: 6 damage
        tier2: 10 damage; restrained (EoT)
        tier3: 14 damage; restrained (save ends)
      - name: Effect
        effect: The area is difficult terrain for enemies until the end of the
          encounter. Any enemy in the area has acid weakness 5.
  - type: feature
    feature_type: ability
    name: Maw of the Abyss
    icon: ❗️
    keywords:
      - Magic
      - Void
    usage: Triggered action
    distance: Self
    target: Self
    trigger: The elementalist takes damage.
    effects:
      - name: Effect
        effect: The elementalist can teleport up to 4 squares. Each creature adjacent to
          the space they leave or appear in takes 4 corruption damage.
  - type: feature
    feature_type: trait
    name: Rivalry
    icon: ⭐️
    effects:
      - effect: At the start of an encounter, the elementalist chooses one creature
          within their line of effect. Both the elementalist and the creature
          can add a d3 roll to power rolls they make against each other.
~~~