---
type: playbook
---

*Hoping for peace isn't enough. Trouble always comes knocking. And that's why we need you: to run the drills, to man the towers, to take charge when things get bad. To be cold enough to send your neighbors to a sure death in order to keep Stonetop safe. That's the job, Marshal. You up for it?*

# Background (Choose 1)
▢![[Scion]]
▢![[Penitent]]
▢![[Luminary]]

# Instinct (Choose 1)
![[Marshal Instincts]]

# Appearance
![[Marshal Appearance]]

# Place of origin and name
![[Marshal Place or Origin and Name]]
# Stats
Assign these scores +2, +1, +1, +0, +0, -1. When a debility is marked, you roll with disadvantage.
![[Image - Marshal Stats.webp]]
# Special Possessions
(Pick 2)

▢ **Chiurgeon's tools:** catgut, straps, bandages, tubes, poultice, willow bark, ◇ bonesaws, etc.
▢ **Distillery**skins of fine whistky (○○ uses, grants advantage to Persuade), copper tubes, malt, ◇◇ firkins, stills, barrels, etc.
▢ **Engineer's tools:** rulers, tapes, rods, plumb-bobs, ◇tripods, ◇ block & tackles, wheelbarrow, etc.
▢ **Personal Symbol** (a flag, crest, marking, etc.): when you ***display or reveal it in a dramatic fashion,*** your crew holds +1 Loyalty (max 3).
▢ **Scribe's tools:** parchment, ink, pigments, vials, quills, ◇ a notebook, etc.
▢ **Weapons of war:** choose up to 3 (now or later):
    ▢ ◇ **Sword,** iron (*close*, +1 damage)
	▢ ◇◇ **Long spear, fine steel,** iron (*reach,* 2 piercing)
	▢ ◇ **Battleaxe,** iron (*close, messy* )
	▢ ◇ **Composite bow** (*far*, +1 damage,  x piercing, ○ low ammo, ○ all out)
▢ .................................................................................... (discuss with GM)
# Moves
You start with Crew, Logistics, any moves from our Background, and 1 move of your choice.
```base
views:
  - type: table
    name: Table
    filters:
      and:
        - file.inFolder("Stonetop Compendium/Rules/Playbooks/The Marshal/Moves")
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



# War Stories
![[War Stories]]

# Introductions
![[Marshal Introductions]]