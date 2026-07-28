---
agility: 2
ancestry:
- Goblin
- Hobgoblin
- Humanoid
- Infernal
ev: '16'
file_basename: Hobgoblin Redglare
file_dpath: Monsters/Hobgoblins/Statblocks
free_strike: 6
intuition: 3
item_id: hobgoblin-redglare
item_index: 09
item_name: Hobgoblin Redglare
level: 6
might: 0
presence: 3
reason: 2
roles:
- Platoon Hexer
scc:
- mcdm.monsters.v1:monster.hobgoblins.statblock:hobgoblin-redglare
scdc:
- 1.1.1:2.22.1:09
size: 1L
source: mcdm.monsters.v1
speed: 5
stability: 4
stamina: '70'
type: monster/hobgoblins/statblock
---

~~~ds-statblock
type: statblock
name: Hobgoblin Redglare
level: 6
roles:
  - Platoon Hexer
ancestry:
  - Goblin
  - Hobgoblin
  - Humanoid
  - Infernal
ev: "16"
stamina: "70"
immunities:
  - Fire 6
speed: 5
movement: Teleport
size: 1L
stability: 4
free_strike: 6
might: 0
agility: 2
reason: 2
intuition: 3
presence: 3
features:
  - type: feature
    feature_type: ability
    name: Eye Flash
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
        tier1: 9 corruption damage; P < 1 slowed (save ends)
        tier2: 14 corruption damage; P < 2 restrained (save ends)
        tier3: 17 corruption damage; P < 3 restrained (save ends)
  - type: feature
    feature_type: ability
    name: Glare of the Old Judgments
    icon: 🏹
    cost: 5 Malice
    keywords:
      - Magic
      - Ranged
      - Strike
    usage: Main action
    distance: Ranged 10
    target: One creature
    effects:
      - roll: Power Roll + 3
        tier1: 10 corruption damage
        tier2: 10 corruption damage, or if the target has P < 2 they are judged
        tier3: The target is judged.
      - name: Effect
        effect: Until the end of the encounter, a judged target takes 10 corruption
          damage at the start of each of their turns, and regains 5 Stamina each
          time they use an ability or other effect that allows another creature
          to spend a Recovery.
  - type: feature
    feature_type: trait
    name: Infernal Ichor
    icon: ⭐️
    effects:
      - effect: When the redglare is reduced to 0 Stamina, they spray burning blood.
          Each creature adjacent to the redglare takes 3 fire damage.
~~~