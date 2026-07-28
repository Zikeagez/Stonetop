---
agility: 1
ancestry:
- Humanoid
- Lizardfolk
ev: '6'
file_basename: Lizardfolk Bloodeye
file_dpath: Monsters/Lizardfolks/Statblocks
free_strike: 3
intuition: 2
item_id: lizardfolk-bloodeye
item_index: '02'
item_name: Lizardfolk Bloodeye
level: 1
might: 1
presence: 0
reason: 0
roles:
- Platoon Hexer
scc:
- mcdm.monsters.v1:monster.lizardfolks.statblock:lizardfolk-bloodeye
scdc:
- 1.1.1:2.7.1:02
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '20'
type: monster/lizardfolks/statblock
---

~~~ds-statblock
type: statblock
name: Lizardfolk Bloodeye
level: 1
roles:
  - Platoon Hexer
ancestry:
  - Humanoid
  - Lizardfolk
ev: "6"
stamina: "20"
speed: 5
movement: Swim
size: 1M
stability: 0
free_strike: 3
might: 1
agility: 1
reason: 0
intuition: 2
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Bola Knock
    icon: 🏹
    ability_type: Signature Ability
    keywords:
      - Ranged
      - Strike
      - Weapon
    usage: Main action
    distance: Ranged 5
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        tier1: 5 damage; A < 0 restrained (save ends)
        tier2: 7 damage; A < 1 restrained (save ends)
        tier3: 9 damage; A < 2 restrained (save ends)
  - type: feature
    feature_type: ability
    name: Bloodshot
    icon: 🏹
    cost: 2 Malice
    keywords:
      - Ranged
      - Strike
      - Weapon
    usage: Main action
    distance: Ranged 10
    target: One creature
    effects:
      - roll: Power Roll + 2
        tier1: 5 acid damage; M < 0 the target has line of effect only within 4 squares
          (save ends)
        tier2: 7 acid damage; M < 1 the target has line of effect only within 3 squares
          (save ends)
        tier3: 9 acid damage; M < 2 the target has line of effect only within 2 squares
          (save ends)
  - type: feature
    feature_type: trait
    name: Reptilian Escape
    icon: ⭐️
    effects:
      - effect: While the bloodeye has a tail, whenever they are grabbed, prone, slowed,
          or weakened, they can lose their tail to immediately end that
          condition, then shift up to 2 squares.
~~~