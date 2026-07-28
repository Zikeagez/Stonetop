---
agility: 4
ancestry:
- Humanoid
- Soulless
- War Dog
ev: '48'
file_basename: Iron Champion Doru
file_dpath: Monsters/War Dogs/Statblocks
free_strike: 10
intuition: 4
item_id: iron-champion-doru
item_index: '29'
item_name: Iron Champion Doru
level: 10
might: 5
presence: 2
reason: 1
roles:
- Elite Brute
scc:
- mcdm.monsters.v1:monster.war-dogs.statblock:iron-champion-doru
scdc:
- 1.1.1:2.51.1:29
size: 1L
source: mcdm.monsters.v1
speed: 5
stability: 2
stamina: '260'
type: monster/war-dogs/statblock
---

~~~ds-statblock
type: statblock
name: Iron Champion Doru
level: 10
roles:
  - Elite Brute
ancestry:
  - Humanoid
  - Soulless
  - War Dog
ev: "48"
stamina: "260"
speed: 5
size: 1L
stability: 2
free_strike: 10
might: 5
agility: 4
reason: 1
intuition: 4
presence: 2
features:
  - type: feature
    feature_type: ability
    name: Houndaxe
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 2
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 5
        tier1: 15 damage
        tier2: 21 damage; Doru gains an edge on his next power roll; M < 4 slide 3
        tier3: 25 damage; Doru has a double edge on his next power roll; M < 5 slide 5
      - name: Effect
        effect: The damage from this ability can't be reduced in any way.
      - cost: 3 Malice
        effect: This ability targets one additional target.
  - type: feature
    feature_type: ability
    name: Bloody Whirlwind
    icon: ❇️
    cost: 2 Malice
    keywords:
      - Area
      - Weapon
    usage: Main action
    distance: 3 burst
    target: Each creature and object in the area
    effects:
      - roll: Power Roll + 5
        tier1: 5 damage; A < 3 bleeding (save ends)
        tier2: 11 damage; A < 4 bleeding (save ends)
        tier3: 15 damage; A < 5 bleeding (save ends)
      - name: Effect
        effect: This ability deals an extra 5 damage for each winded target in the area.
  - type: feature
    feature_type: ability
    name: Hunting Leap
    icon: 🏹
    keywords:
      - Ranged
    usage: Maneuver
    distance: Ranged 5
    target: One creature or object
    effects:
      - name: Effect
        effect: Doru jumps to an unoccupied space adjacent to the target, then can make
          a free strike against them. If the target is bleeding or winded, the
          distance of the ability becomes Ranged 10 and the free strike deals an
          extra 5 damage.
  - type: feature
    feature_type: ability
    name: Laugh It Off
    icon: ❗️
    keywords:
      - "-"
    usage: Triggered action
    distance: Self
    target: Self
    trigger: An enemy makes a strike against Doru.
    effects:
      - name: Effect
        effect: The triggering strike takes a bane and Doru gains an edge on his next
          power roll.
  - type: feature
    feature_type: trait
    name: Iron Juggernaut
    icon: ⭐️
    effects:
      - effect: Doru can't be made slowed or restrained. Additionally, he can move while
          grabbed, and a creature grabbing him moves along with him unless they
          let go.
  - type: feature
    feature_type: trait
    name: The Scarless
    icon: ⭐️
    effects:
      - effect: Doru regains 10 Stamina at the start of each of his turns unless he took
          acid or fire damage since the start of his previous turn. Whenever he
          regains Stamina this way, the Director can spend 2 Malice to end one
          effect on Doru that can be ended by a saving throw.
  - type: feature
    feature_type: trait
    name: Champion's Loyalty Collar
    icon: ⭐️
    effects:
      - effect: When Doru is reduced to 0 Stamina, his loyalty collar explodes, dealing
          20 damage to each enemy and object within 3 squares of him.
~~~