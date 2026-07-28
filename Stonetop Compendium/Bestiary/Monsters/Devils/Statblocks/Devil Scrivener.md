---
agility: 3
ancestry:
- Devil
- Infernal
ev: 7 for four minions
file_basename: Devil Scrivener
file_dpath: Monsters/Devils/Statblocks
free_strike: 3
intuition: 1
item_id: devil-scrivener
item_index: '01'
item_name: Devil Scrivener
level: 5
might: 0
presence: 2
reason: 1
roles:
- Minion Harrier
scc:
- mcdm.monsters.v1:monster.devils.statblock:devil-scrivener
scdc:
- 1.1.1:2.39.1:01
size: 1M
source: mcdm.monsters.v1
speed: 6
stability: 0
stamina: '9'
type: monster/devils/statblock
---

~~~ds-statblock
type: statblock
name: Devil Scrivener
level: 5
roles:
  - Minion Harrier
ancestry:
  - Devil
  - Infernal
ev: 7 for four minions
stamina: "9"
immunities:
  - Fire 5
speed: 6
movement: Fly
size: 1M
stability: 0
free_strike: 3
with_captain: +3 bonus to speed
might: 0
agility: 3
reason: 1
intuition: 1
presence: 2
features:
  - type: feature
    feature_type: ability
    name: Litigation
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Charge
      - Magic
      - Melee
      - Strike
    usage: Main action
    distance: Melee 1
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 3
        tier1: 3 corruption damage
        tier2: 5 corruption damage; slowed (EoT)
        tier3: 6 corruption damage; slowed (EoT)
      - name: Effect
        effect: The scrivener can shift 1 square.
  - type: feature
    feature_type: trait
    name: True Name
    icon: ⭐️
    effects:
      - effect: If a creature within 10 squares speaks the scrivener's true name, the
          scrivener loses their fire immunity and any nondamaging effects of
          their signature ability until the end of the encounter.
~~~