---
agility: 0
ancestry:
- Humanoid
- Rival
ev: '16'
file_basename: Rival Tactician
file_dpath: Monsters/Rivals/1st Echelon/Statblocks
free_strike: 5
intuition: 0
item_id: rival-tactician
item_index: '06'
item_name: Rival Tactician
level: 2
might: 2
presence: 0
reason: 1
roles:
- Elite Artillery
scc:
- mcdm.monsters.v1:monster.rivals.1st echelon.statblock:rival-tactician
scdc:
- 1.1.1:2.5.1.1:06
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 2
stamina: '60'
type: monster/rivals/1st echelon/statblock
---

~~~ds-statblock
type: statblock
name: Rival Tactician
level: 2
roles:
  - Elite Artillery
ancestry:
  - Humanoid
  - Rival
ev: "16"
stamina: "60"
speed: 5
size: 1M
stability: 2
free_strike: 5
might: 2
agility: 0
reason: 1
intuition: 0
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Dual Targeting Shot
    icon: 🏹
    ability_type: Signature Ability
    keywords:
      - Ranged
      - Strike
      - Weapon
    usage: Main action
    distance: Ranged 10
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 2
        tier1: 7 damage
        tier2: 11 damage
        tier3: 14 damage
      - cost: 2 Malice
        effect: Two allies within distance can make a free strike against one of the
          targets.
  - type: feature
    feature_type: ability
    name: I'll Cover You!
    icon: 🏹
    cost: 3 Malice
    keywords:
      - Ranged
      - Strike
      - Weapon
    usage: Main action
    distance: Ranged 5
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        tier1: 8 damage; M < 0 weakened (save ends)
        tier2: 13 damage; M < 1 weakened (save ends)
        tier3: 16 damage; M < 2 weakened (save ends)
      - name: Effect
        effect: One ally adjacent to the target regains 5 Stamina.
  - type: feature
    feature_type: ability
    name: Overwatch
    icon: ❗️
    keywords:
      - Ranged
    usage: Triggered action
    distance: Ranged 10
    target: The triggering enemy
    trigger: An enemy within distance willingly moves.
    effects:
      - name: Effect
        effect: At any point during the movement, the tactician makes a free strike
          against the target.
  - type: feature
    feature_type: trait
    name: Rivalry
    icon: ⭐️
    effects:
      - effect: At the start of an encounter, the tactician chooses one creature within
          their line of effect. Both the tactician and the creature can add a d3
          roll to power rolls they make against each other.
~~~