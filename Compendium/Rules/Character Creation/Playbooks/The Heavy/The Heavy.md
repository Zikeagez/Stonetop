---
type: playbook
---
*These are good people. Hard-working, honest. They look out for each other. But sometimes, looking out for each other ain't enough. Sometimes, good people need someone to stick up for them. Someone who's not afraid to get a little bloody. To get heavy. Yeah, someone like you.*

# Background (Choose 1)
▢![[Sheriff]]
▢![[Blood-Soaked Past]]
▢![[Storm-Marked]]

# Instinct (Choose 1)
![[Heavy Instincts]]

# Appearance
![[Heavy Appearance]]

# Place of origin and name
![[Heavy Place of Origin and Name]]
# Stats
Assign these scores +2, +1, +1, +0, +0, -1. When a debility is marked, you roll with disadvantage.
![[Image - Stats The Heavy.webp]]
# Special Possessions
(Pick 2)
▢ **Distillery:** skins of fine whisky(○○ uses, grants advantage to Persuade), copper tubes, malt, ◇◇ firkins, stills, barrels, etc. 
▢ **Chirurgeon's tools:** catgut, straps, bandages, tubes, poultices, willow bark, ◇ bonesaws, etc.
▢ **Husbandry tools:** brushes, muzzles, collars, feed, ◇ whips, ◇ bridles, etc. Gain advantage to Persuade domestic beasts (livestock, dogs, etc.).
▢ **Smithy** (or access to it): iron goods, ingots, thick gloves, ◇ tongs, ◇ bellows, an anvil, etc.
▢ **Stoneworker's tools:** chisels, drills, ◇ prybars, ◇ spikes, ◇ block & tackles, wheelbarrow, etc.
▢ **Weapons of war:** choose up to 3 (now or later):
    ▢ ◇ **Sword,** iron (*close*, +1 damage)
	▢ ◇ **Battleaxe,** iron (*close, messy*)
	▢ ◇ **Warhammer,** iron (*close,* 2 piercing)
	▢ ◇ **Mace or flail,** iron (*close, forceful*)
	▢ ◇ **Crossbow** (*far*, +1 damage, *reload,* x piercing, ○ low ammo, ○ all out)

▢ .................................................................................... (discuss with GM)
# Moves
You start with Dangerous, Hard to Kill, and either Armored OR Uncanny Reflexes.
```base
views:
  - type: table
    name: Table
    filters:
      and:
        - file.inFolder("Stonetop Compendium/Rules/Playbooks/The Heavy/Moves")
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



# A History of Violence
![[A History of Violence]]


# Introductions
![[Heavy Introduction]]