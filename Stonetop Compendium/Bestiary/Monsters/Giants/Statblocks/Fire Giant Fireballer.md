---
agility: 2
ancestry:
- Fire Giant
- Giant
ev: 11 for four minions
file_basename: Fire Giant Fireballer
file_dpath: Monsters/Giants/Statblocks
free_strike: 3
intuition: 2
item_id: fire-giant-fireballer
item_index: '03'
item_name: Fire Giant Fireballer
level: 9
might: 4
presence: 1
reason: 0
roles:
- Minion Harrier
scc:
- mcdm.monsters.v1:monster.giants.statblock:fire-giant-fireballer
scdc:
- 1.1.1:2.23.1:03
size: '4'
source: mcdm.monsters.v1
speed: 7
stability: 5
stamina: '13'
type: monster/giants/statblock
---

~~~ds-statblock
type: statblock
name: Fire Giant Fireballer
level: 9
roles:
  - Minion Harrier
ancestry:
  - Fire Giant
  - Giant
ev: 11 for four minions
stamina: "13"
immunities:
  - Fire 9
speed: 7
size: "4"
stability: 5
free_strike: 3
with_captain: +3 bonus to speed
might: 4
agility: 2
reason: 0
intuition: 2
presence: 1
features:
  - type: feature
    feature_type: ability
    name: Blazing Leap
    icon: ❇️
    ability_type: Signature Ability
    keywords:
      - Area
      - Weapon
    usage: Main action
    distance: 1 burst
    target: Each enemy and object in the area
    effects:
      - roll: Power Roll + 4
        tier1: 2 fire damage
        tier2: 5 fire damage; push 1
        tier3: 6 fire damage; push 2
      - name: Effect
        effect: The fireballer can jump up to 4 squares before using this ability.
  - type: feature
    feature_type: trait
    name: Searing Skin
    icon: ⭐️
    effects:
      - effect: Whenever an adjacent enemy grabs the fireballer or uses a melee ability
          against them, that enemy takes 5 fire damage.
~~~