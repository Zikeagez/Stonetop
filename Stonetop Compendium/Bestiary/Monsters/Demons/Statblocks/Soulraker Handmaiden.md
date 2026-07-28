---
agility: 0
ancestry:
- Abyssal
- Demon
- Soulraker
ev: '10'
file_basename: Soulraker Handmaiden
file_dpath: Monsters/Demons/Statblocks
free_strike: 4
intuition: 2
item_id: soulraker-handmaiden
item_index: '17'
item_name: Soulraker Handmaiden
level: 8
might: 3
presence: 4
reason: 2
roles:
- Horde Ambusher
scc:
- mcdm.monsters.v1:monster.demons.statblock:soulraker-handmaiden
scdc:
- 1.1.1:2.35.1:17
size: 1M
source: mcdm.monsters.v1
speed: 0
stability: 0
stamina: '50'
type: monster/demons/statblock
---

~~~ds-statblock
type: statblock
name: Soulraker Handmaiden
level: 8
roles:
  - Horde Ambusher
ancestry:
  - Abyssal
  - Demon
  - Soulraker
ev: "10"
stamina: "50"
weaknesses:
  - Holy 5
speed: 0
size: 1M
stability: 0
free_strike: 4
might: 3
agility: 0
reason: 2
intuition: 2
presence: 4
features:
  - type: feature
    feature_type: trait
    name: Implanted Parasite
    icon: ⭐️
    effects:
      - effect: >-
          A host creature implanted by a soulraker hivequeen's Stinging
          Ovipositor has no physical or mental signs of the handmaiden gestating
          inside the host's body.


          After 1d3 + 1 weeks of gestation, the handmaiden fully forms inside
          the host. The handmaiden always moves with and occupies the same space
          as the host and can't be separated from them. While totally within the
          creature, the handmaiden doesn't have line of effect to the host or
          targets outside the host and vice versa. As a maneuver, the handmaiden
          can emerge from the host as a horrifying tower of flesh and bone that
          remains attached to the host's insides. While emerged, the handmaiden
          can use a move action to make the host move up to their speed and has
          access to the host's signature abilities, using the host's modifiers
          for any power rolls. The handmaiden has the same Stability as the
          host. If the handmaiden or host is force moved, the other moves with
          them. While emerged, the handmaiden can be targeted independently of
          the host. The handmaiden can retreat totally within the host's body as
          a maneuver. If the handmaiden dies, their remains separate from the
          host.

          The Find a Cure downtime project in Draw Steel: Heroes can be used to
          find a cure that removes a handmaiden from a host. The cure kills the
          handmaiden when consumed.
  - type: feature
    feature_type: ability
    name: Emergent Horrors
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 2
    target: One creature or object
    effects:
      - roll: Power Roll + 4
        tier1: 8 corruption damage
        tier2: 11 corruption damage
        tier3: 13 corruption damage; M < 4 frightened (save ends)
      - name: Effect
        effect: If the handmaiden was totally within their host's body at the start of
          this turn, the ability deals an extra 8 damage.
  - type: feature
    feature_type: trait
    name: Lethe
    icon: ⭐️
    effects:
      - effect: While the handmaiden is winded, they gain an edge on strikes, and any
          strike made against them gains an edge.
~~~