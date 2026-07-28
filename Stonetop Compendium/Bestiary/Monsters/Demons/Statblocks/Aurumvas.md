---
agility: 2
ancestry:
- Abyssal
- Demon
ev: '48'
file_basename: Aurumvas
file_dpath: Monsters/Demons/Statblocks
free_strike: 10
intuition: 3
item_id: aurumvas
item_index: '14'
item_name: Aurumvas
level: 10
might: 5
presence: 5
reason: 5
roles:
- Leader
scc:
- mcdm.monsters.v1:monster.demons.statblock:aurumvas
scdc:
- 1.1.1:2.35.1:14
size: '3'
source: mcdm.monsters.v1
speed: 8
stability: 2
stamina: '260'
type: monster/demons/statblock
---

~~~ds-statblock
type: statblock
name: Aurumvas
level: 10
roles:
  - Leader
ancestry:
  - Abyssal
  - Demon
ev: "48"
stamina: "260"
weaknesses:
  - Holy 5
speed: 8
movement: Fly
size: "3"
stability: 2
free_strike: 10
might: 5
agility: 2
reason: 5
intuition: 3
presence: 5
features:
  - type: feature
    feature_type: trait
    name: Absorb Soul
    icon: ⭐️
    effects:
      - effect: Whenever any demon is reduced to 0 Stamina within 10 squares of
          Aurumvas, the Director gains 1 Malice. Aurumvas loses this trait while
          he is dazed.
  - type: feature
    feature_type: ability
    name: Greedy Hands
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Magic
      - Melee
      - Strike
    usage: Main action
    distance: Melee 2
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 5
        tier1: 15 corruption damage; R < 4 weakened (save ends)
        tier2: 20 corruption damage; R < 5 weakened (save ends)
        tier3: 24 corruption damage; R < 6 weakened (save ends)
      - cost: 2 Malice
        effect: Aurumvas regains Stamina equal to the damage dealt.
  - type: feature
    feature_type: ability
    name: Covetous Bolts
    icon: 🏹
    cost: 3 Malice
    keywords:
      - Magic
      - Ranged
      - Strike
    usage: Main action
    distance: Ranged 20
    target: Two creatures
    effects:
      - roll: Power Roll + 5
        tier1: 15 psychic damage; P < 4 dazed (save ends)
        tier2: 20 psychic damage; P < 5 dazed (save ends)
        tier3: 24 psychic damage; P < 6 dazed (save ends)
      - cost: 2 Malice
        effect: While dazed this way, a target can't gain Heroic Resources.
  - type: feature
    feature_type: ability
    name: Greed Is Good
    icon: 🏹
    cost: 2 Malice
    keywords:
      - Ranged
    usage: Maneuver
    distance: Ranged 10
    target: Special
    effects:
      - name: Effect
        effect: Aurumvas chooses a supernatural treasure or an item made of gold and
          teleports to an unoccupied space adjacent to that object, then ends
          one effect on him that can be ended by a saving throw.
  - type: feature
    feature_type: trait
    name: More... More...
    icon: ⭐️
    effects:
      - effect: While Aurumvas is winded, he has a double edge on strikes.
  - type: feature
    feature_type: trait
    name: Soulsight
    icon: ⭐️
    effects:
      - effect: Any creature within 5 squares of Aurumvas can't be hidden from him.
  - type: feature
    feature_type: ability
    name: Time Is Money
    icon: ☠️
    ability_type: Villain Action 1
    keywords:
      - Area
      - Magic
    usage: "-"
    distance: 20 burst
    target: Self and each ally in the area
    effects:
      - name: Effect
        effect: Aurumvas warps time with his abyssal avarice. Each target can teleport
          up to their speed and make a free strike.
  - type: feature
    feature_type: ability
    name: Hostile Acquisition
    icon: ☠️
    ability_type: Villain Action 2
    keywords:
      - Ranged
    usage: "-"
    distance: Ranged 10
    target: Special
    effects:
      - name: Effect
        effect: Aurumvas chooses up to three treasures within distance that he has line
          of effect to and that aren't artifacts. Until the end of the
          encounter, ethereal golden snakes swirl around the target treasures.
          While an affected treasure is worn or held by a hero, each time that
          hero gains any amount of their Heroic Resource, the Director gains 1
          Malice.
  - type: feature
    feature_type: ability
    name: No Matter the Cost
    icon: ☠️
    ability_type: Villain Action 3
    keywords:
      - Area
      - Magic
      - Ranged
    usage: "-"
    distance: Four 3 cubes within 10
    target: Each creature in the area
    effects:
      - name: Effect
        effect: Aurumvas summons treasures from his vaults into the area, then causes
          them to explode.
      - roll: Power Roll + 5
        tier1: 10 fire damage; push 1
        tier2: 15 fire damage; push 2
        tier3: 19 fire damage; push 3
~~~