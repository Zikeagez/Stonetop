---
agility: 1
ancestry:
- Giant
- Ogre
ev: 9 for four minions
file_basename: Ogre Blue Blood
file_dpath: Monsters/Ogres/Statblocks
free_strike: 4
intuition: 0
item_id: ogre-blue-blood
item_index: '03'
item_name: Ogre Blue Blood
level: 7
might: 4
presence: 2
reason: -1
roles:
- Minion Brute
scc:
- mcdm.monsters.v1:monster.ogres.statblock:ogre-blue-blood
scdc:
- 1.1.1:2.4.1:03
size: '2'
source: mcdm.monsters.v1
speed: 5
stability: 4
stamina: '13'
type: monster/ogres/statblock
---

~~~ds-statblock
type: statblock
name: Ogre Blue Blood
level: 7
roles:
  - Minion Brute
ancestry:
  - Giant
  - Ogre
ev: 9 for four minions
stamina: "13"
speed: 5
size: "2"
stability: 4
free_strike: 4
with_captain: Gain an edge on strikes
might: 4
agility: 1
reason: -1
intuition: 0
presence: 2
features:
  - type: feature
    feature_type: ability
    name: Crush Underfoot
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 2
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 4
        tier1: 4 damage
        tier2: 7 damage; M < 3 prone
        tier3: 8 damage; prone
      - name: Effect
        effect: A target who is already prone takes an extra 4 damage.
  - type: feature
    feature_type: trait
    name: In My Stead
    icon: ⭐️
    effects:
      - effect: Whenever the blue blood would make a free strike, an ally within 5
          squares can make a free strike instead.
  - type: feature
    feature_type: trait
    name: Royal Anger
    icon: ⭐️
    effects:
      - effect: The blue blood has damage immunity 2 while their squad has three or
          fewer minions in it.
~~~