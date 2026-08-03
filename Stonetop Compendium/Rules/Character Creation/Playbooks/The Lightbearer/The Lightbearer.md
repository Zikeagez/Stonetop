---
type: playbook
---

*Imagine yourself and your kin in a cave lit by a single torch, entranced by shadow puppet stories. Imagine realizing there is a grater truth, and stepping out of the cave into the Light of day. Would you not bring that Light back into the darkness, to set your people free?*

# Background (Choose 1)
▢![[Auspicious Birth]]
▢![[Itinerant Mystic]]
▢![[Soul on Fire]]

# Instinct (Choose 1)
![[Lightbearer Instincts]]

# Appearance
![[Lightbearer Appearance]]

# Place of origin and name
![[Lightbearer Place of Origin and Name]]
# Stats
Assign these scores +2, +1, +1, +0, +0, -1. When a debility is marked, you roll with disadvantage.
![[Image - Lightbearer Stats.webp]]
# Special Possessions
(Pick 2)

▢ **Apiary:** beeswax, candles (*close, area,* lasts ~1hr) honey, ◇ bee smokers, ◇ hats & veils, etc. 
▢ **Books & Scrolls** (○○○○○ uses):expend a use to consult your collection and turn a [[Know Things]] roll you just made into a 10+.
▢ **Chandlery:** beeswax, candles (*close, area,* lasts ~1hr), wicks, scented herbs, soap, lye, ash, etc.
▢ **Disillery:** skins of fine whisky (○○ uses, grants advantage to Persuade), copper tubes, malt, ◇◇ firkins, stills, barrels, etc. 
▢ **Glassworks:** vials, charms, lenses, sand, marbles, bellows, crucible, ◇ lanterns (○○○○○ hours, *close, area*), etc.
▢ **Holy relicts** (○○○ uses): if you have one in inventory when you Invoke the Sun God, you can mark a use in lieu of choosing a consequence.
▢ **Luthier's Tools:** chisels, files, catgut, various woods, stains, ◇ a lute, ◇ a fiddle, etc.
▢ .................................................................................... (discuss with GM)
# Moves
You start with Consecrated Flame and Invoke the Sun God, plus 1 more of your choice.
```base
views:
  - type: table
    name: Table
    filters:
      and:
        - file.inFolder("Stonetop Compendium/Rules/Playbooks/The Lightbearer/Moves")
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



# Praise The Day
![[Praise The Day]]

# Introductions
![[Lightbearer Introductions]]