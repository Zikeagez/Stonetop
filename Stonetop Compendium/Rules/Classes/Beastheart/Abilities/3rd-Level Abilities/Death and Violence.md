```ds-feature
type: feature
feature_type: ability
name: Death and Violence
cost: 7 Ferocity
flavor: You leap from your foe's corpse.
keywords:
  - Beastheart
  - Magic
  - Ranged
usage: Triggered
distance: 📐 Ranged 10
target: 🎯 One creature
effects:
  - name: Trigger
    effect: Your companion uses an ability that reduces the target to 0 Stamina.

  - roll: Power Roll + Might
    tier1: If `P < WEAK` frightened (save ends)
    tier2: 4 psychic damage; `P < AVERAGE` frightened (save ends)
    tier3: 8 psychic damage; `P < STRONG` frightened (save ends)
```

