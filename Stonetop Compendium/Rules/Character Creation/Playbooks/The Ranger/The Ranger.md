---
type: playbook
---

*Your true home is out there. Away from the Old Roads, in the wild places, where you've faced storm and beast alike. But unknown forces are at work beyond the Ringwall, and you fear for your kith and kin. these are strange times. Guide them, ranger, and keep them safe when darkness falls.

# Background (Choose 1)
▢![[Mighty Hunter]]
▢![[Wide Wanderer]]
▢![[Beast-Bonded]]

# Instinct (Choose 1)
![[Ranger Instinct]]

# Appearance
![[Ranger Appearance]]

# Place of origin and name
![[Ranger Place of Origin and Name]]
# Stats
Assign these scores +2, +1, +1, +0, +0, -1. When a debility is marked, you roll with disadvantage.
![[Image - Ranger Stats.webp]]
# Special Possessions
(Pick 2)

🗹 ◇ **Composite bow** (*far*, +1 damage,  x piercing, ○ low ammo, ○ all out)
▢ **Distillery**skins of fine whistky (○○ uses, grants advantage to Persuade), copper tubes, malt, ◇◇ firkins, stills, barrels, etc.
▢ **Hideouts**(○○○ uses): expend a use to have a well-stocked, safe shelter nearby; GM can veto.
▢ **Husbandry tools:** brushes, muzzles, collars, feed, ◇ whips, ◇ bridles, etc. Gain advantage to Persuade domestic beasts (livestock, dogs, etc.).
▢ **Hounds,** 2-3 followers (*trackers, keen-nosed, fast*); HP 6; Damage d6 (*hand, grabby*) **Instinct** to give chase; Cost: training
▢ **Lay of the Land** (○○○ uses): expend a use to know where to find ....., without having to [[Know Things]]; GM can veto
▢ **Trapping gear:** snares, pelts, musk, bait, etc. When you ***[[Forage]],*** get +1 use of provisions.
▢ .................................................................................... (discuss with GM)
# Moves
You start with Home on the Range, any moves from your Background, plus 1 of your choice.
```base
views:
  - type: table
    name: Table
    filters:
      and:
        - file.inFolder("Stonetop Compendium/Rules/Playbooks/The Ranger/Moves")
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
![[Something Wicked This Way Comes]]

# Introductions
![[Ranger Introductions]]