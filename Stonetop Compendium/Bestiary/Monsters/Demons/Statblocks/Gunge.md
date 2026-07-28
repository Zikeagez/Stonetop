---
agility: 2
ancestry:
- Abyssal
- Demon
ev: '6'
file_basename: Gunge
file_dpath: Monsters/Demons/Statblocks
free_strike: 2
intuition: 2
item_id: gunge
item_index: '19'
item_name: Gunge
level: 4
might: 3
presence: -1
reason: 1
roles:
- Horde Controller
scc:
- mcdm.monsters.v1:monster.demons.statblock:gunge
scdc:
- 1.1.1:2.35.1:19
size: '3'
source: mcdm.monsters.v1
speed: 6
stability: 0
stamina: '25'
type: monster/demons/statblock
---

~~~ds-statblock
type: statblock
name: Gunge
level: 4
roles:
  - Horde Controller
ancestry:
  - Abyssal
  - Demon
ev: "6"
stamina: "25"
weaknesses:
  - Holy 5
speed: 6
size: "3"
stability: 0
free_strike: 2
might: 3
agility: 2
reason: 1
intuition: 2
presence: -1
features:
  - type: feature
    feature_type: ability
    name: Bilious Expulsion
    icon: 🔳
    ability_type: Signature Ability
    keywords:
      - Area
      - Ranged
      - Weapon
    usage: Main action
    distance: 1 burst, or 3 cube within 5
    target: One creature or object in the area
    effects:
      - roll: Power Roll + 3
        tier1: 5 acid damage; M < 1 slowed (save ends)
        tier2: 7 acid damage; M < 2 slowed (save ends)
        tier3: 9 acid damage; M < 3 restrained (save ends)
      - name: Effect
        effect: The ground and any surfaces in the area pool with slime. The slime is
          difficult terrain for enemies, and any enemy is bleeding while in the
          area.
  - type: feature
    feature_type: ability
    name: Spew Slide
    icon: ❗️
    cost: 1 Malice
    keywords:
      - "-"
    usage: Free triggered action
    distance: Self
    target: Self
    trigger: The gunge takes damage from a melee strike.
    effects:
      - name: Effect
        effect: The gunge vomits with great force, letting them shift up to their speed
          and ignore any additional effects from the strike. The space the gunge
          occupied before the shift is covered in slime that is difficult
          terrain for enemies. Additionally, any enemy is bleeding while in the
          slime.
  - type: feature
    feature_type: trait
    name: Lethe
    icon: ⭐️
    effects:
      - effect: While the gunge is winded, they gain an edge on strikes, and any strike
          made against them gains an edge.
  - type: feature
    feature_type: trait
    name: Soulsight
    icon: ⭐️
    effects:
      - effect: Any creature within 2 squares of the gunge can't be hidden from them.
~~~