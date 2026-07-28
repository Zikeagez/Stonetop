---
agility: 2
ancestry:
- Humanoid
- Kobold
ev: 3 for four minions
file_basename: Kobold Veles
file_dpath: Monsters/Kobolds/Statblocks
free_strike: 1
intuition: 0
item_id: kobold-veles
item_index: '07'
item_name: Kobold Veles
level: 1
might: 0
presence: 0
reason: 0
roles:
- Minion Harrier
scc:
- mcdm.monsters.v1:monster.kobolds.statblock:kobold-veles
scdc:
- 1.1.1:2.10.1:07
size: 1S
source: mcdm.monsters.v1
speed: 6
stability: 0
stamina: '4'
type: monster/kobolds/statblock
---

~~~ds-statblock
type: statblock
name: Kobold Veles
level: 1
roles:
  - Minion Harrier
ancestry:
  - Humanoid
  - Kobold
ev: 3 for four minions
stamina: "4"
speed: 6
size: 1S
stability: 0
free_strike: 1
with_captain: +1 bonus to speed
might: 0
agility: 2
reason: 0
intuition: 0
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Pilium
    icon: ⚔️
    ability_type: Signature Ability
    keywords:
      - Melee
      - Ranged
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1 or Ranged 5
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 2
        tier1: 1 damage
        tier2: 2 damage
        tier3: 3 damage
      - name: Effect
        effect: Until the start of the veles's next turn, the target can't make
          opportunity attacks against any kobold.
  - type: feature
    feature_type: trait
    name: Shield? Shield!
    icon: ⭐️
    effects:
      - effect: While adjacent to an ally who also has this trait, the veles has
          stability 1, has cover, and grants cover to allies.
~~~