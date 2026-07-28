---
file_basename: Wild Rumpus
file_dpath: Perks/Exploration Perks
item_id: wild-rumpus
item_index: "06"
item_name: Wild Rumpus
scc:
  - mcdm.heroes.v1:perk.exploration:ive-got-you
scdc:
  - 1.1.1:18.3:06
source: mcdm.heroes.v1
type: perk/exploration
description: You have the Wild Rumpus ability
---

This perk can be taken only by beastheart characters.

You have the following ability.

```ds-feature
type: feature
feature_type: ability
name: Wild Rumpus
flavor: The ability to glide like a condor or race like a wolf is intoxicating - but beware the temptation to run yourself to death.
keywords:
  - Beastheart
  - Magic
usage: Maneuver
distance: 📐 Self
target: 🎯 Self
effects:
  - name: Effect
    effect: For one minute or until you or your companion takes damage, you and your companion gain each other's movement types in addition to your own. You and your companion both use your speed or your companion's speed, whichever is higher. Each additional time you use this ability after the first, you take damage equal to your level until you finish a respite or gain 1 or more Victories. This damage can't be reduced in any way and doesn't end the ability's effect.
```