---
title: CreatureName
obsidianUIMode: preview
noteType: pf2eMonster
cssClasses: pf2e
aliases: 
tags:
  - pf2e/creature/type/beast
  - pf2eMonster
  - pf2e/creature/level/3
statblock: inline
name: CreatureName
level: 
license: OGL
icon: 
---

```statblock
columns: 2
forcecolumns: true
layout: Basic Pathfinder 2e Layout
token: [[modules/pf2e-tokens-bestiaries/portraits/humanoid/hybrid/centaur.webp| ]]
source: "Homebrew"
name: "Name"
level: "Creature Level"

alignment: ""
size: ""
trait_01: [[beast]]
modifier: 
perception:
  - name: "Perception"
    desc: "+9; Darkvision"
languages: "Common, Elven, Fey"
skills:
  - name: "Skills"
    desc: "Athletics: +11, Diplomacy: +6, Intimidation: +6, Nature: +7, Survival: +7"
abilityMods: [4, 2, 1, 0, 2, 1]
speed: 40 feet
sourcebook: "_Pathfinder Bestiary_"
ac: 20
armorclass:
  - name: AC
    desc: "20 22 with shield raised; __Fort__ +8, __Ref__ +9, __Will__ +9"
hp: 40
health:
  - name: ""
  - name: HP
    desc: "40"
abilities_top:
  - name: ""
  - name: "Items"
    desc: "[[Equipment/Longsword|Longsword]], 3x [[Equipment/Spear|Spear]], [[Equipment/Steel Shield|Steel Shield]], [[Equipment/Breastplate|Breastplate]]"
abilities_mid:
  - name: ""
  - name: "[[Bestiary Ability Glossary/Shield Block|Shield Block]]"
    desc: "`pf2:r`  **Trigger** The monster has its shield raised and takes damage from a physical attack.\n* * *\n\n**Effect** The monster snaps its shield into place to deflect a blow. The shield prevents the monster from taking an amount of damage up to the shield's Hardness. The monster and the shield each take any remaining damage, possibly breaking or destroying the shield."

attacks:
  - name: ""

  - name: "**Melee** `pf2:1` Hoof"
    desc: "+9 (agile)\n__Damage__  1d10 + 4 bludgeoning"

  - name: "**Melee** `pf2:1` Longsword"
    desc: "+11 (versatile p)\n__Damage__  1d8 + 4 slashing"

  - name: "**Melee** `pf2:1` Spear"
    desc: "+11 ()\n__Damage__  1d6 + 4 piercing"

  - name: "**Ranged** `pf2:1` Spear"
    desc: "+9 (thrown 20 ft.)\n__Damage__  1d6 + 4 piercing"

  - name: "[[Bestiary Ability Glossary/Trample|Trample]]"
    desc: "`pf2:3`  Medium or smaller, hoof, `DC 18 Reflex check` save\n* * *\n\nThe monster Strides up to double its Speed and can move through the spaces of creatures of the listed size, Trampling each creature whose space it enters. The monster can attempt to Trample the same creature only once in a single use of Trample. The monster deals the damage of the listed Strike, but trampled creatures can attempt a basic Reflex save at the listed DC (no damage on a critical success, half damage on a success, double damage on a critical failure)."
 
```

```encounter-table
name: Centaur
creatures:
  - 1: Centaur
```




