---
agility: 3
ancestry:
- Humanoid
- Soulless
- War Dog
ev: '6'
file_basename: War Dog Hypokrite
file_dpath: Monsters/War Dogs/Statblocks
free_strike: 3
intuition: 0
item_id: war-dog-hypokrite
item_index: '35'
item_name: War Dog Hypokrite
level: 4
might: 1
presence: 2
reason: 0
roles:
- Horde Ambusher
scc:
- mcdm.monsters.v1:monster.war-dogs.statblock:war-dog-hypokrite
scdc:
- 1.1.1:2.51.1:35
size: 1M
source: mcdm.monsters.v1
speed: 8
stability: 0
stamina: '30'
type: monster/war-dogs/statblock
---

~~~ds-statblock
type: statblock
name: War Dog Hypokrite
level: 4
roles:
  - Horde Ambusher
ancestry:
  - Humanoid
  - Soulless
  - War Dog
ev: "6"
stamina: "30"
speed: 8
size: 1M
stability: 0
free_strike: 3
might: 1
agility: 3
reason: 0
intuition: 0
presence: 2
features:
  - type: feature
    feature_type: ability
    name: Needle-Knife
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: One creature or object
    effects:
      - roll: Power Roll + 3
        tier1: 6 damage
        tier2: 8 damage; A < 2 bleeding (save ends)
        tier3: 10 damage; A < 3 bleeding and weakened (save ends)
      - name: Effect
        effect: This ability deals an extra 6 damage if the hypokrite is hidden or
          disguised.
  - type: feature
    feature_type: ability
    name: Feign Death
    icon: ❗️
    cost: 2 Malice
    keywords:
      - Ranged
    usage: Triggered action
    distance: Ranged 20
    target: Special
    trigger: The hypokrite takes damage.
    effects:
      - name: Effect
        effect: The hypokrite detonates their loyalty collar to deal 2d6 damage to each
          adjacent enemy, but teleports to an unoccupied space adjacent to an
          ally within distance and remains alive.
  - type: feature
    feature_type: trait
    name: Face in the Crowd
    icon: ⭐️
    effects:
      - effect: The hypokrite is invisible while adjacent to any ally who isn't hidden,
          and they can attempt to hide even while observed. Whenever they use
          the Hide maneuver, the hypokrite can disguise themself as another
          creature within line of effect.
  - type: feature
    feature_type: trait
    name: Loyalty Collar
    icon: ⭐️
    effects:
      - effect: When the hypokrite is reduced to 0 Stamina, their loyalty collar
          explodes, dealing 2d6 damage to each adjacent enemy and object.
~~~