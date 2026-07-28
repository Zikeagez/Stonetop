```ds-feature
type: feature
feature_type: ability
name: Rip Them Apart!
cost: 9 Ferocity
flavor: Harnessing your companion's strenght, you send your foe flying.
keywords:
  - Beastheart
  - Melee
  - Strike
  - Weapon
usage: Main Action
distance: 📐 Melee 1
target: 🎯 One creature
effects:
  - roll: Power Roll + Might
    tier1: 11 + M damage; `M < WEAK` bleeding (save ends)
    tier2: 17 + M damage; `M < AVERAGE` bleeding (save ends)
    tier3: 22 + M damage; `M < STRONG` bleeding (save ends)

  - name: Effect
    effect: If the target is grabbbed by your partner, the target takes extra damage equal to your Might score plus your partner's Might score. If the target is reduced to 0 Stamina by this ability, each enemy within 2 squares who has `P < AVERAGE` is frightened (save ends).
```

