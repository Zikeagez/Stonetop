---
agility: 2
ancestry:
- Humanoid
- Rival
ev: '28'
file_basename: Rival Elementalist
file_dpath: Monsters/Rivals/2nd Echelon/Statblocks
free_strike: 6
intuition: 2
item_id: rival-elementalist
item_index: '03'
item_name: Rival Elementalist
level: 5
might: 0
presence: 0
reason: 3
roles:
- Elite Controller
scc:
- mcdm.monsters.v1:monster.rivals.2nd echelon.statblock:rival-elementalist
scdc:
- 1.1.1:2.5.2.1:03
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 1
stamina: '120'
type: monster/rivals/2nd echelon/statblock
---

~~~ds-statblock
type: statblock
name: Rival Elementalist
level: 5
roles:
  - Elite Controller
ancestry:
  - Humanoid
  - Rival
ev: "28"
stamina: "120"
speed: 5
size: 1M
stability: 1
free_strike: 6
might: 0
agility: 2
reason: 3
intuition: 2
presence: 0
features:
  - type: feature
    feature_type: ability
    name: The Thriving Wilds
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
      - roll: Power Roll + 3
        tier1: 9 damage; slide 1; M < 1 3 acid damage
        tier2: 14 damage; slide 2; M < 2 5 acid damage
        tier3: 17 damage; slide 3; M < 3 7 acid damage
  - type: feature
    feature_type: ability
    name: The Depths Hunger
    icon: 🔳
    cost: 4 Malice
    keywords:
      - Area
      - Green
      - Magic
      - Ranged
    usage: Main action
    distance: 4 cube within 10
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 3
        tier1: 5 damage
        tier2: 9 damage; restrained (EoT)
        tier3: 11 damage; restrained (save ends)
      - name: Effect
        effect: The area is difficult terrain for enemies until the end of the
          encounter. Any enemy in the area has acid weakness 3.
  - type: feature
    feature_type: ability
    name: Fissures of Darkness
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
        effect: The elementalist can teleport up to 3 squares. Each creature adjacent to
          the space they leave takes 3 corruption damage.
  - type: feature
    feature_type: trait
    name: Rivalry
    icon: ⭐️
    effects:
      - effect: At the start of an encounter, the elementalist chooses one creature
          within their line of effect. Both the elementalist and the creature
          can add a d3 roll to power rolls they make against each other.
~~~