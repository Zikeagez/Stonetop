```ds-feature
type: feature
feature_type: ability
name: Jaws of Death
cost: 7 Ferocity
flavor: Your bloody-forehead smash drives your companion into a frenzy.
keywords:
  - Beastheart
  - Melee
  - Magic
  - Ranged
usage: Main Action
distance: 📐 Melee 1 or Ranged 5
target: 🎯 One creature
effects:
  - roll: Power Roll + Intuition
    tier1: 7 + I damage; `P < WEAK` weakened (save ends)
    tier2: 10 + I damage; `P < AVERAGE` weakened (save ends)
    tier3: 19 + I damage; `P < STRONG` weakened (save ends)

  - name: Effect
    effect: Whenever a target more than 3 squares away from you fails the saving throw while weakened this way, you can pull the target up to a number of squares equal to your Intuition score as a free triggered action.
```

