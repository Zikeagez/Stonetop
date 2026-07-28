---
agility: 2
ancestry:
- Giant
- Ogre
ev: 9 for four minions
file_basename: Ogre Tantrum
file_dpath: Monsters/Ogres/Statblocks
free_strike: 4
intuition: 0
item_id: ogre-tantrum
item_index: '02'
item_name: Ogre Tantrum
level: 7
might: 4
presence: -1
reason: -1
roles:
- Minion Artillery
scc:
- mcdm.monsters.v1:monster.ogres.statblock:ogre-tantrum
scdc:
- 1.1.1:2.4.1:02
size: '2'
source: mcdm.monsters.v1
speed: 5
stability: 2
stamina: '10'
type: monster/ogres/statblock
---

~~~ds-statblock
type: statblock
name: Ogre Tantrum
level: 7
roles:
  - Minion Artillery
ancestry:
  - Giant
  - Ogre
ev: 9 for four minions
stamina: "10"
speed: 5
size: "2"
stability: 2
free_strike: 4
with_captain: +5 bonus to ranged distance
might: 4
agility: 2
reason: -1
intuition: 0
presence: -1
features:
  - type: feature
    feature_type: ability
    name: Throw Fit
    icon: 🏹
    ability_type: Signature Ability
    keywords:
      - Ranged
      - Strike
      - Weapon
    usage: Main action
    distance: Ranged 8
    target: One creature or object per minion
    effects:
      - name: Effect
        effect: The tantrum unearths a rock or a hunk of terrain and tosses it. If a
          size 1L, 1M, or 1S creature or object adjacent to the tantrum has A <
          3 the tantrum can grab them to use as the projectile for this ability.
      - effect: A creature or object used as a projectile is vertically pushed 8 (or 13
          with a captain), ignoring stability.
        roll: Power Roll + 4
        tier1: 4 damage
        tier2: 7 damage; push 2
        tier3: 8 damage; push 4
  - type: feature
    feature_type: trait
    name: Excessive Anger
    icon: ⭐️
    effects:
      - effect: The tantrum has damage immunity 3 and speed 8 while their squad has two
          or fewer minions in it.
~~~