---
type: playbook
---

*Look here at this little town, this candleflame in the darkness. Its very existence is an act of courage and faith. And Aratis has charged you to keep it: to settle its disputes; to chronicle its tales; to defend it from darkness and ruin. Take up your hammer, Judge. Your town needs you.*

# Background (Choose 1)
▢![[Legacy]]
▢![[Missionary]]
▢![[Prophet]]

# Instinct (Choose 1)
![[Judge Instinct]]

# Appearance
![[Judge Appearance]]

# Place of origin and name
![[Judge Place of Origin and Name]]
# Stats
Assign these scores +2, +1, +1, +0, +0, -1. When a debility is marked, you roll with disadvantage.
![[Image - Judge Stats.webp]]
# Special Possessions
(Pick 2)
☑ **Your symbol of authority** (pick 1:)
	▢ ◇◇ **Black iron maul,** utterly immune to all magic (*close, forceful, awkward,* +1 damage)
	▢ ◇◇ **Makerglass shield,** etched with Aratis's symbol (*indestructible,* +1 armor, +1 Readiness on a [[Defend]] 7+)
	▢ ◇ **Helm** set with a dark ice "jewel." Grants advantage to resist mind-affecting magic.
---

☑ **Scribe's tools:** parchment, ink, pigments, vials, quills, ◇ a notebook, etc.
▢ **Aviary:** thick gloves, bird hoods, tethers, seed, ◇ messenger birds, ◇ birdcages, etc.
▢ **Carpenter's tools:** chisels, files, nails, pitch, ◇ prybars, ◇ saws, ◇◇ firkins, barrels, etc.
▢ **Engineer's tools:** rulers, tapes, rods, plumb-bobs, ◇ tripods, ◇ block & tackles, wheelbarrow, etc.
▢ **Smithy** (or access to it): iron goods, ingots, thick gloves, ◇ tongs, ◇ bellows, an anvil, etc.
▢ .................................................................................... (discuss with GM)
# Moves
You start with Censure, Chronicler of Stonetop, plus 2 more of your choice.
```base
views:
  - type: table
    name: Table
    filters:
      and:
        - file.inFolder("Stonetop Compendium/Rules/Playbooks/The Judge/Moves")
    order:
      - mark
      - file.name
      - requires
    sort:
      - property: file.name
        direction: ASC
      - property: requires
        direction: DESC

```



# The Chronicle
[[The Chronicle]]

# The Lawkeeper
[[The Lawkeeper]]

# Introductions
![[Heavy Introduction]]