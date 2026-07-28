---
agility: 2
ancestry:
- Humanoid
- Soulless
- War Dog
ev: '10'
file_basename: War Dog Firestarter
file_dpath: Monsters/War Dogs/Statblocks
free_strike: 3
intuition: 4
item_id: war-dog-firestarter
item_index: '45'
item_name: War Dog Firestarter
level: 8
might: 0
presence: 1
reason: 3
roles:
- Horde Hexer
scc:
- mcdm.monsters.v1:monster.war-dogs.statblock:war-dog-firestarter
scdc:
- 1.1.1:2.51.1:45
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '45'
type: monster/war-dogs/statblock
---

~~~ds-statblock
type: statblock
name: War Dog Firestarter
level: 8
roles:
  - Horde Hexer
ancestry:
  - Humanoid
  - Soulless
  - War Dog
ev: "10"
stamina: "45"
immunities:
  - Fire 8
speed: 5
size: 1M
stability: 0
free_strike: 3
might: 0
agility: 2
reason: 3
intuition: 4
presence: 1
features:
  - type: feature
    feature_type: ability
    name: Twin Flamebelchers
    icon: 🔳
    ability_type: Signature Ability
    keywords:
      - Area
      - Weapon
    usage: Main action
    distance: 10 x 1 line within 1
    target: Each creature and object in the area
    effects:
      - roll: Power Roll + 4
        tier1: 3 fire damage; A < 2 the target is seared (save ends)
        tier2: 6 fire damage; A < 3 the target is seared (save ends)
        tier3: 8 fire damage; A < 4 the target is seared (save ends)
      - name: Effect
        effect: A seared creature takes a bane on strikes and has damage weakness 5. If
          this ability obtains a tier 3 outcome against one or more creatures
          who are already seared, the firestarter can use Enflame as a free
          triggered action.
  - type: feature
    feature_type: ability
    name: Enflame
    icon: 🏹
    keywords:
      - Magic
      - Ranged
    usage: Maneuver
    distance: Ranged 10
    target: Special
    effects:
      - name: Effect
        effect: This ability targets each enemy within 2 squares of any seared creature
          within distance.
      - roll: Power Roll + 4
        tier1: 2 fire damage
        tier2: 4 fire damage; A < 3 the target is seared (save ends)
        tier3: 6 fire damage; A < 4 the target is seared (save ends)
  - type: feature
    feature_type: trait
    name: Loyalty Collar
    icon: ⭐️
    effects:
      - effect: When the firestarter is reduced to 0 Stamina, their loyalty collar
          explodes, dealing 3d6 damage to each adjacent enemy and object.
~~~