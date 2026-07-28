---
ancestryTrait: Yes
name: Vengeance Mark
ancestry: Revenant
type: Purchased
cost: 2 Points
description: As a maneuver, you place a magic sigil on a creature within 10 squares. When you place a sigil, you decide where it appears on the creature's body, and whether the sigil is visible to only you or to all creatures.
---
As a maneuver, you place a magic sigil on a creature within 10 squares. When you place a sigil, you decide where it appears on the creature's body, and whether the sigil is visible to only you or to all creatures.

You always know the direction to the exact location of a creature who bears one of your sigils and is on the same world. You can have a number of active sigils equal to your level, and can remove a sigil from a creature at will (no action required). If you already have the maximum number of sigils activated and you place a new one, your oldest sigil disappears with no other effect.

Additionally, you have the following signature ability. Signature abilities can be used at will.

```ds-feature
type: trait
feature_type: ability
name: Detonate Sigil
cost: 
flavor: _A magic sigil you placed on a creature explodes with energy._
keywords:
  - Magic
  - Ranged
  - Strike
usage: Main action
distance: Ranged 10
target: One creature bearing your sigil
effects:
  - roll: Power Roll + Reason, Inuition, or Presence 
    tier1: 3 + R, I, or P damage; slide 1
    tier2: 5 + R, I, or P damage; slide 2
    tier3: 7 + R, I, or P damage; slide 3
  - name: Effect
    effect: The sigil disappears from the creature.
```


