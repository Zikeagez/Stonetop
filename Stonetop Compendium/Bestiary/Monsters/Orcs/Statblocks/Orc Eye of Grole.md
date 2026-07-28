---
agility: 1
ancestry:
- Humanoid
- Orc
ev: '6'
file_basename: Orc Eye of Grole
file_dpath: Monsters/Orcs/Statblocks
free_strike: 4
intuition: 0
item_id: orc-eye-of-grole
item_index: '07'
item_name: Orc Eye of Grole
level: 1
might: 1
presence: 2
reason: 0
roles:
- Platoon Artillery
scc:
- mcdm.monsters.v1:monster.orcs.statblock:orc-eye-of-grole
scdc:
- 1.1.1:2.16.1:07
size: 1M
source: mcdm.monsters.v1
speed: 6
stability: 0
stamina: '20'
type: monster/orcs/statblock
---

~~~ds-statblock
type: statblock
name: Orc Eye of Grole
level: 1
roles:
  - Platoon Artillery
ancestry:
  - Humanoid
  - Orc
ev: "6"
stamina: "20"
immunities:
  - Cold
  - fire
  - or lightning
speed: 6
size: 1M
stability: 0
free_strike: 4
might: 1
agility: 1
reason: 0
intuition: 0
presence: 2
features:
  - type: feature
    feature_type: trait
    name: Elemental Affinity
    icon: ⭐️
    effects:
      - effect: The eye has an affinity for one of the following damage types cold,
          fire, or lightning. The chosen type determines the eye's damage
          immunity and the damage dealt by their abilities.
  - type: feature
    feature_type: ability
    name: Elemental Discharge
    icon: 🏹
    ability_type: Signature Ability
    keywords:
      - Magic
      - Ranged
      - Strike
    usage: Main action
    distance: Ranged 10
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        tier1: 6 damage; push 2, or the eye shifts up to 2 squares away from the target
        tier2: 9 damage; slide 4, or the eye shifts up to 4 squares away from the target
        tier3: 12 damage; slide 6, or the eye shifts up to 6 squares away from the
          target
      - name: Effect
        effect: This ability deals cold, fire, or lightning damage.
  - type: feature
    feature_type: ability
    name: Power Burst
    icon: 🔳
    cost: 3 Malice
    keywords:
      - Area
      - Magic
    usage: Main action
    distance: 5 x 2 line within 1
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 2
        tier1: 3 damage; push 2
        tier2: 5 damage; push 3
        tier3: 8 damage; push 4, prone
      - name: Effect
        effect: This ability deals cold, fire, or lightning damage, and any enemy
          targeted by the ability has damage weakness 3 to the same damage type
          (save ends).
  - type: feature
    feature_type: trait
    name: Relentless
    icon: ⭐️
    effects:
      - effect: If the eye is reduced to 0 Stamina, they can make a free strike before
          dying. If the target of the free strike is reduced to 0 Stamina, the
          eye is reduced to 1 Stamina instead.
~~~