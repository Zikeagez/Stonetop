---
agility: 2
ancestry:
- Animal
ev: '12'
file_basename: Predator A
file_dpath: Monsters/Animals/Statblocks
free_strike: 5
intuition: 1
item_id: predator-a
item_index: '05'
item_name: Predator A
level: 1
might: 1
presence: 1
reason: -2
roles:
- Elite Brute
scc:
- mcdm.monsters.v1:monster.animals.statblock:predator-a
scdc:
- 1.1.1:2.34.1:05
size: '2'
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '80'
type: monster/animals/statblock
---

~~~ds-statblock
type: statblock
name: Predator A
level: 1
roles:
  - Elite Brute
ancestry:
  - Animal
ev: "12"
stamina: "80"
speed: 5
size: "2"
stability: 0
free_strike: 5
might: 1
agility: 2
reason: -2
intuition: 1
presence: 1
features:
  - type: feature
    feature_type: ability
    name: Natural Weapon
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 2
        tier1: 7 damage
        tier2: 10 damage; M < 1 prone
        tier3: 13 damage; M < 1 prone
  - type: feature
    feature_type: ability
    name: Ready to Strike
    icon: 👤
    keywords:
      - "-"
    usage: Maneuver
    distance: Self
    target: Self
    effects:
      - name: Effect
        effect: The predator assesses their environment or lets loose a threatening roar
          and gains an edge on their next strike.
  - type: feature
    feature_type: ability
    name: Quick Strike
    icon: ❗️
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Triggered action
    distance: Melee 1
    target: The triggering creature or object
    trigger: A creature or object comes within distance.
    effects:
      - name: Effect
        effect: The predator makes a free strike against the target. If the predator was
          hidden from the target, the strike deals an extra 3 damage.
  - type: feature
    feature_type: trait
    name: Nature's Spirit
    icon: ⭐️
    effects:
      - effect: While outdoors or in a natural environment, the predator can negate a
          bane on their abilities or turn a double bane into a bane.
~~~