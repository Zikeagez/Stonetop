---
type: playbook
---

*Look at us. Huddling behind our walls, hearing evil in every passing noise. Cowards, all. All, but you. You fear not the unknown. You plunge into it, searching. Grasping at what has been lost. What will you find, o Seeker? Signs of a bright new age? Or signs of our doom?

# Background (Choose 1)
▢![[Patriot]]
▢![[Antiquarian]]
▢![[Witch Hunter]]

# Instinct (Choose 1)
![[Seeker Instinct]]

# Appearance
![[Seeker Appearance]]

# Place of origin and name
![[Seeker Place of Origin and Name]]
# Stats
Assign these scores +2, +1, +1, +0, +0, -1. When a debility is marked, you roll with disadvantage.
![[Image - Seeker Stats.webp]]
# Special Possessions
(Pick 2)

🗹 **Scribe's tools:** parchment, ink, pigments, vials, quills, ◇ a notebook, etc.
▢ **Books & Scrolls** (○○○○○ uses):expend a use to consult your collection and turn a [[Know Things]] roll you just made into a 10+.
▢ **Distillery**skins of fine whisky (○○ uses, grants advantage to Persuade), copper tubes, malt, ◇◇ firkins, stills, barrels, etc.
▢ **Engineer's tools:** rulers, tapes, rods, plumb-bobs, ◇tripods, ◇ block & tackles, wheelbarrow, etc.
▢ **Laboratory:** chemics, reagents, vials, measures, ◇ scales, ◇ decanters, etc. Every season, produce d4-2 uses of ◇ naphtha (*thrown, area, dangerous,* ignores armor).
▢ **Scribe's tools:** parchment, ink, pigments, vials, quills, ◇ a notebook, etc.
▢ **Paraphernalia:** crystals, incense, talismans, blood, bone, horn, eye of newt, ◇ braziers, ◇◇ a cauldron, etc.
▢ **Trade contacts:** small amounts of salt, glass, silk, spice, medicinal herbs, pigments, ivory, etc.
▢ .................................................................................... (discuss with GM)
# Moves
You start with Well Versed, Work With What You've Got, plus 1 from your Background.
```base
views:
  - type: table
    name: Table
    filters:
      and:
        - file.inFolder("Stonetop Compendium/Rules/Character Creation/Playbooks/The Seeker/Moves")
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



# Collection
![[Collection]]

# Introductions
![[Seeker Introductions]]