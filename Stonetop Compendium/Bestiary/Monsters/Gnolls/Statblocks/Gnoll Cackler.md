---
agility: 0
ancestry:
- Abyssal
- Gnoll
ev: '4'
file_basename: Gnoll Cackler
file_dpath: Monsters/Gnolls/Statblocks
free_strike: 2
intuition: 2
item_id: gnoll-cackler
item_index: '07'
item_name: Gnoll Cackler
level: 2
might: 0
presence: 2
reason: 2
roles:
- Horde Hexer
scc:
- mcdm.monsters.v1:monster.gnolls.statblock:gnoll-cackler
scdc:
- 1.1.1:2.6.1:07
size: 1S
source: mcdm.monsters.v1
speed: 5
stability: 1
stamina: '15'
type: monster/gnolls/statblock
---

~~~ds-statblock
type: statblock
name: Gnoll Cackler
level: 2
roles:
  - Horde Hexer
ancestry:
  - Abyssal
  - Gnoll
ev: "4"
stamina: "15"
speed: 5
size: 1S
stability: 1
free_strike: 2
might: 0
agility: 0
reason: 2
intuition: 2
presence: 2
features:
  - type: feature
    feature_type: ability
    name: Moment of Brutality
    icon: 🏹
    ability_type: Signature Ability
    keywords:
      - Magic
      - Ranged
      - Strike
    usage: Main action
    distance: Ranged 8
    target: One creature
    effects:
      - roll: Power Roll + 2
        tier1: 4 psychic damage; I < 0 the target makes a free strike against a creature
          of the cackler's choice
        tier2: 5 psychic damage; I < 1 the target makes a free strike against a creature
          of the cackler's choice
        tier3: 7 psychic damage; I < 2 the target uses a signature ability against a
          creature of the cackler's choice
      - name: Effect
        effect: An ally targeted by this ability ignores the damage and can make a free
          strike.
  - type: feature
    feature_type: ability
    name: Cackler's Cackletongue
    icon: ❇️
    cost: 4 Malice
    keywords:
      - Area
      - Magic
    usage: Maneuver
    distance: 2 burst
    target: Each creature in the area
    effects:
      - name: Effect
        effect: Each enemy target makes an **Intuition test**. If any target hasn't used
          their own Cackletongue maneuver on this turn, they can use it
          immediately at no cost.
        tier1: Frightened (save ends)
        tier2: Frightened (EoT)
        tier3: No effect
  - type: feature
    feature_type: trait
    name: Death Frenzy
    icon: ⭐️
    effects:
      - effect: Whenever a non-minion ally within 5 squares of the cackler is reduced to
          0 Stamina, the cackler moves up to their speed and can make a melee
          free strike.
~~~