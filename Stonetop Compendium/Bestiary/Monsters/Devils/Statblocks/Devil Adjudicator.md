---
agility: 1
ancestry:
- Devil
- Infernal
ev: '32'
file_basename: Devil Adjudicator
file_dpath: Monsters/Devils/Statblocks
free_strike: 7
intuition: 1
item_id: devil-adjudicator
item_index: '02'
item_name: Devil Adjudicator
level: 6
might: 0
presence: 3
reason: 2
roles:
- Elite Controller
scc:
- mcdm.monsters.v1:monster.devils.statblock:devil-adjudicator
scdc:
- 1.1.1:2.39.1:02
size: 1M
source: mcdm.monsters.v1
speed: 6
stability: 1
stamina: '140'
type: monster/devils/statblock
---

~~~ds-statblock
type: statblock
name: Devil Adjudicator
level: 6
roles:
  - Elite Controller
ancestry:
  - Devil
  - Infernal
ev: "32"
stamina: "140"
immunities:
  - Fire 5
speed: 6
movement: Fly
size: 1M
stability: 1
free_strike: 7
might: 0
agility: 1
reason: 2
intuition: 1
presence: 3
features:
  - type: feature
    feature_type: ability
    name: Infernal Injunction
    icon: 🏹
    ability_type: Signature Ability
    keywords:
      - Magic
      - Ranged
      - Strike
    usage: Main action
    distance: Ranged 10
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 3
        tier1: 10 fire damage; I < 1 frightened (save ends)
        tier2: 15 fire damage; I < 1 frightened (save ends)
        tier3: 18 fire damage; I < 1 frightened (save ends)
      - name: Effect
        effect: The adjudicator can slide a target frightened by this ability up to 2
          squares.
  - type: feature
    feature_type: ability
    name: Adjudicator's Interdiction
    icon: 🏹
    keywords:
      - Magic
      - Ranged
    usage: Main action
    distance: Ranged 10
    target: One creature
    effects:
      - name: Effect
        effect: The target makes a Presence test.
        tier1: The target is slowed, takes a bane on power rolls, and can't regain
          Stamina (save ends).
        tier2: The target is slowed and takes a bane on power rolls (save ends).
        tier3: Slowed (save ends)
  - type: feature
    feature_type: ability
    name: Quid Pro Quo
    icon: 🏹
    keywords:
      - Magic
      - Ranged
    usage: Maneuver
    distance: Ranged 10
    target: One ally or frightened creature
    effects:
      - name: Effect
        effect: The adjudicator and the target teleport to switch places.
  - type: feature
    feature_type: ability
    name: Devilish Charm
    icon: ❗️
    cost: 2 Malice
    keywords:
      - Magic
      - Ranged
    usage: Triggered action
    distance: Ranged 5
    target: The triggering creature
    trigger: A creature targets the adjudicator with a strike.
    effects:
      - name: Effect
        effect: The target makes a Presence test.
        tier1: The adjudicator chooses a new target for the strike.
        tier2: The adjudicator halves the triggering damage.
        tier3: The target takes a bane on the strike.
  - type: feature
    feature_type: trait
    name: Vexatious Litigation
    icon: ⭐️
    effects:
      - effect: Any creature within 10 squares of the adjudicator who has P < 3 takes a
          −2 penalty to saving throws.
  - type: feature
    feature_type: trait
    name: True Name
    icon: ⭐️
    effects:
      - effect: If a creature within 10 squares speaks the adjudicator's true name, the
          adjudicator loses their damage immunities, any nondamaging effects of
          their signature ability, and their Devilish Charm ability until the
          end of the encounter.
~~~