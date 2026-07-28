---
agility: 2
ancestry:
- Giant
- Stone Giant
ev: 10 for four minions
file_basename: Sand Stone Giant
file_dpath: Monsters/Giants/Statblocks
free_strike: 3
intuition: 3
item_id: sand-stone-giant
item_index: 08
item_name: Sand Stone Giant
level: 8
might: 4
presence: 0
reason: 0
roles:
- Minion Controller
scc:
- mcdm.monsters.v1:monster.giants.statblock:sand-stone-giant
scdc:
- 1.1.1:2.23.1:08
size: '4'
source: mcdm.monsters.v1
speed: 7
stability: 10
stamina: '14'
type: monster/giants/statblock
---

~~~ds-statblock
type: statblock
name: Sand Stone Giant
level: 8
roles:
  - Minion Controller
ancestry:
  - Giant
  - Stone Giant
ev: 10 for four minions
stamina: "14"
speed: 7
movement: Burrow
size: "4"
stability: 10
free_strike: 3
with_captain: +6 bonus to Stamina
might: 4
agility: 2
reason: 0
intuition: 3
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Buried in Sand
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Magic
      - Melee
      - Strike
    usage: Main action
    distance: Melee 3
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 4
        tier1: 3 damage; slide 2
        tier2: 6 damage; slide 3; A < 3 restrained (save ends)
        tier3: 8 damage; slide 4; A < 4 restrained (save ends)
  - type: feature
    feature_type: trait
    name: Stonebreaker Flesh
    icon: ⭐️
    effects:
      - effect: Whenever an enemy obtains a tier 1 outcome on a melee ability used
          against the sand stone giant, they take a bane on that ability until
          the end of the encounter.
  - type: feature
    feature_type: trait
    name: Stone Steps
    icon: ⭐️
    effects:
      - effect: The sand stone giant ignores difficult terrain.
  - type: feature
    feature_type: trait
    name: Stone Swim
    icon: ⭐️
    effects:
      - effect: The sand stone giant can burrow through stone, but can't drag other
          creatures underground when they do so.
~~~