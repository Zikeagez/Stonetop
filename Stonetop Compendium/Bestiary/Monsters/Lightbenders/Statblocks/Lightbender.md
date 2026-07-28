---
agility: 1
ancestry:
- Beast
- Lightbender
ev: '20'
file_basename: Lightbender
file_dpath: Monsters/Lightbenders/Statblocks
free_strike: 6
intuition: 1
item_id: lightbender
item_index: '01'
item_name: Lightbender
level: 3
might: 2
presence: -1
reason: -3
roles:
- Elite Ambusher
scc:
- mcdm.monsters.v1:monster.lightbenders.statblock:lightbender
scdc:
- 1.1.1:2.25.1:01
size: '2'
source: mcdm.monsters.v1
speed: 10
stability: 1
stamina: '100'
type: monster/lightbenders/statblock
---

~~~ds-statblock
type: statblock
name: Lightbender
level: 3
roles:
  - Elite Ambusher
ancestry:
  - Beast
  - Lightbender
ev: "20"
stamina: "100"
speed: 10
size: "2"
stability: 1
free_strike: 6
might: 2
agility: 1
reason: -3
intuition: 1
presence: -1
features:
  - type: feature
    feature_type: ability
    name: Flash Swipe
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 2
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        tier1: 9 damage
        tier2: 14 damage
        tier3: 18 damage
      - name: Effect
        effect: If this ability gains an edge or has a double edge, it deals an extra 4
          damage.
  - type: feature
    feature_type: ability
    name: Piercing Tails
    icon: 🗡
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 2
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        tier1: 8 damage
        tier2: 12 damage; M < 1 bleeding (save ends)
        tier3: 15 damage; M < 2 bleeding (save ends)
      - name: Effect
        effect: While bleeding this way, the target takes a bane on tests to search for
          the lightbender while they are hidden.
  - type: feature
    feature_type: ability
    name: Hypnotic Mane
    icon: ❇️
    cost: 5 Malice
    keywords:
      - Area
      - Magic
    usage: Maneuver
    distance: 3 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 2
        tier1: I < 0 dazed (save ends)
        tier2: I < 1 dazed (save ends)
        tier3: I < 2 dazed (save ends)
      - name: Effect
        effect: While dazed this way, a target has speed 0. If a target takes damage, or
          if someone else uses a main action to shake the target out of their
          stupor, the dazed condition ends.
  - type: feature
    feature_type: ability
    name: Stalker's Afterimage
    icon: ❗️
    keywords:
      - Magic
    usage: Triggered action
    distance: Self
    target: Self
    trigger: The lightbender takes damage from a strike.
    effects:
      - name: Effect
        effect: The lightbender halves the damage, ignores any nondamaging effects
          associated with it, and can teleport up to 5 squares. If they teleport
          into concealment or cover, the lightbender can immediately attempt to
          hide as a free maneuver.
  - type: feature
    feature_type: trait
    name: Avoidance
    icon: ⭐️
    effects:
      - effect: Any effect on the lightbender that would be ended by a saving throw
          instead ends automatically at the end of their next turn.
~~~