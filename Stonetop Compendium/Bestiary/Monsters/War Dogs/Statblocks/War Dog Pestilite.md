---
agility: 1
ancestry:
- Humanoid
- Soulless
- War Dog
ev: '5'
file_basename: War Dog Pestilite
file_dpath: Monsters/War Dogs/Statblocks
free_strike: 2
intuition: 0
item_id: war-dog-pestilite
item_index: '16'
item_name: War Dog Pestilite
level: 3
might: 0
presence: 2
reason: 0
roles:
- Horde Controller
scc:
- mcdm.monsters.v1:monster.war-dogs.statblock:war-dog-pestilite
scdc:
- 1.1.1:2.51.1:16
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '20'
type: monster/war-dogs/statblock
---

~~~ds-statblock
type: statblock
name: War Dog Pestilite
level: 3
roles:
  - Horde Controller
ancestry:
  - Humanoid
  - Soulless
  - War Dog
ev: "5"
stamina: "20"
immunities:
  - Poison 3
speed: 5
size: 1M
stability: 0
free_strike: 2
might: 0
agility: 1
reason: 0
intuition: 0
presence: 2
features:
  - type: feature
    feature_type: ability
    name: Plaguecaster
    icon: 🔳
    ability_type: Signature Ability
    keywords:
      - Area
      - Magic
      - Ranged
    usage: Main action
    distance: 3 cube within 10
    target: Each creature in the area
    effects:
      - roll: Power Roll + 2
        tier1: 2 poison damage; I < 0 frightened (save ends)
        tier2: 4 poison damage; I < 1 frightened (save ends)
        tier3: 5 poison damage; I < 2 frightened (save ends)
      - name: Effect
        effect: The area is filled with a cloud of pestilence that lasts until the start
          of the pestilite's next turn. Any creature who enters the area for the
          first time in a round or starts their turn there takes 2 poison
          damage.
  - type: feature
    feature_type: ability
    name: Posthumous Promotion
    icon: 🏹
    keywords:
      - Magic
      - Ranged
    usage: Maneuver
    distance: Ranged 10
    target: One war dog
    effects:
      - name: Effect
        effect: If the target has a loyalty collar, they are reduced to 0 Stamina.
  - type: feature
    feature_type: trait
    name: Loyalty Collar
    icon: ⭐️
    effects:
      - effect: When the pestilite is reduced to 0 Stamina, their loyalty collar
          explodes, dealing 1d6 damage to each adjacent enemy and object.
~~~