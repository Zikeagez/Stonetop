---
agility: 1
ancestry:
- Undead
- Vampire
ev: 9 for four minions
file_basename: Blood Starved Vampire
file_dpath: Monsters/Undead/Statblocks
free_strike: 3
intuition: 1
item_id: blood-starved-vampire
item_index: '01'
item_name: Blood-Starved Vampire
level: 7
might: 4
presence: -3
reason: -3
roles:
- Minion Harrier
scc:
- mcdm.monsters.v1:monster.undead.statblock:blood-starved-vampire
scdc:
- 1.1.1:2.8.1:01
size: 1M
source: mcdm.monsters.v1
speed: 6
stability: 0
stamina: '12'
type: monster/undead/statblock
---

~~~ds-statblock
type: statblock
name: Blood-Starved Vampire
level: 7
roles:
  - Minion Harrier
ancestry:
  - Undead
  - Vampire
ev: 9 for four minions
stamina: "12"
immunities:
  - Corruption 7
  - poison 7
speed: 6
movement: Climb
size: 1M
stability: 0
free_strike: 3
with_captain: +3 bonus to speed
might: 4
agility: 1
reason: -3
intuition: 1
presence: -3
features:
  - type: feature
    feature_type: ability
    name: Feeding Frenzy
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 4
        tier1: 3 damage
        tier2: 6 damage
        tier3: 7 damage; M < 4 bleeding (EoT)
      - name: Effect
        effect: If a target made bleeding this way is already bleeding, they are instead
          knocked prone and can't stand until the end of their next turn.
  - type: feature
    feature_type: trait
    name: Unslakable Bloodthirst
    icon: ⭐️
    effects:
      - effect: The blood-starved vampire has speed 10 while any creature within 10
          squares of them is bleeding. The vampire must use Feeding Frenzy
          against a bleeding creature on their turn if they are able to.
~~~