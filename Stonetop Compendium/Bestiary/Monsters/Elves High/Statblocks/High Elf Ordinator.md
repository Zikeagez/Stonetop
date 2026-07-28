---
agility: 2
ancestry:
- Fey
- High Elf
- Humanoid
ev: '20'
file_basename: High Elf Ordinator
file_dpath: Monsters/Elves High/Statblocks
free_strike: 5
intuition: 2
item_id: high-elf-ordinator
item_index: '07'
item_name: High Elf Ordinator
level: 3
might: 0
presence: 3
reason: 3
roles:
- Leader
scc:
- mcdm.monsters.v1:monster.elves-high.statblock:high-elf-ordinator
scdc:
- 1.1.1:2.14.1:07
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '120'
type: monster/elves-high/statblock
---

~~~ds-statblock
type: statblock
name: High Elf Ordinator
level: 3
roles:
  - Leader
ancestry:
  - Fey
  - High Elf
  - Humanoid
ev: "20"
stamina: "120"
speed: 5
movement: Fly
size: 1M
stability: 0
free_strike: 5
might: 0
agility: 2
reason: 3
intuition: 2
presence: 3
features:
  - type: feature
    feature_type: ability
    name: Lightning Rod
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
      - roll: Power Roll + 3
        tier1: 9 lightning damage; R < 1 dazed (save ends)
        tier2: 14 lightning damage; R < 2 dazed (save ends)
        tier3: 17 lightning damage; R < 3 dazed (save ends)
      - name: Effect
        effect: Until the start of the ordinator's next turn, each ally high elf in the
          encounter gains an edge on ability rolls against the target.
  - type: feature
    feature_type: ability
    name: Elemental Uproar
    icon: ❇️
    keywords:
      - Area
      - Magic
    usage: Maneuver
    distance: 10 burst
    target: Each elemental ally in the area
    effects:
      - name: Effect
        effect: Each target can move up to their speed or make a free strike. Elemental
          mote targets can, instead, use their Spark of Life trait.
  - type: feature
    feature_type: ability
    name: Summon Elemental
    icon: 🏹
    cost: 2 Malice
    keywords:
      - Ranged
    usage: Maneuver
    distance: Ranged 10
    target: Special
    effects:
      - name: Effect
        effect: The ordinator summons four elemental motes or four soot crows into
          unoccupied space within distance.
      - cost: 3 Malice
        effect: The ordinator instead summons one ceramic horse or one winded
          brambleguard into an unoccupied space within distance.
  - type: feature
    feature_type: ability
    name: Enough!
    icon: ❗️
    keywords:
      - Ranged
    usage: Triggered action
    distance: Ranged 10
    target: The triggering enemy
    trigger: An enemy within distance uses an ability against the ordinator or any
      ally within distance.
    effects:
      - name: Effect
        effect: The ordinator uses Lightning Rod against the target after the ability is
          resolved.
  - type: feature
    feature_type: trait
    name: Otherworldly Blessing
    icon: ⭐️
    effects:
      - effect: At the start of each of their turns, the ordinator can choose one or
          more effects on them that can be ended by a saving throw. The effects
          instead end at the end of the ordinator's turn.
  - type: feature
    feature_type: ability
    name: Fountains Roar, Now Free From the Earth
    icon: ☠️
    ability_type: Villain Action 1
    keywords:
      - Area
      - Magic
    usage: "-"
    distance: 10 burst
    target: Each ally in the area
    effects:
      - name: Effect
        effect: Each target glows briefly, and can end one effect on themself then move
          up to their speed.
  - type: feature
    feature_type: ability
    name: And the Sun Forsook Her Children
    icon: ☠️
    ability_type: Villain Action 2
    keywords:
      - Area
      - Magic
      - Ranged
    usage: "-"
    distance: 5 cube within 10
    target: Each enemy in the area
    effects:
      - name: Effect
        effect: Each target makes a **Presence test**.
        tier1: 12 corruption damage; pull 5 toward the center of the cube
        tier2: 9 corruption damage; pull 3 toward the center of the cube
        tier3: Pull 1 toward the center of the cube
      - name: Effect
        effect: The area turns dark and distorted, and is difficult terrain for enemies.
  - type: feature
    feature_type: ability
    name: But We Will Change Her Mind
    icon: ☠️
    ability_type: Villain Action 3
    keywords:
      - Area
      - Magic
    usage: "-"
    distance: 10 burst
    target: Self and each ally in the area
    effects:
      - name: Effect
        effect: Each target's free strike now has the Magic keyword and can target two
          creatures or objects. Additionally, each target glows with magic.
~~~