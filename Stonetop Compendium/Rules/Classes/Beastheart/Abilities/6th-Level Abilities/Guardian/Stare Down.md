```ds-feature
type: feature
feature_type: ability
name: Stare Down
cost: 9 Ferocity
flavor: Your companion locks eyes with an enemy, imposing theirw ill upon the enemy and daring them to move a muscle.
keywords:
  - Companion
  - Magic
  - Ranged
usage: Maneuver
distance: 📐 Ranged 5
target: 🎯 One creature
effects:
  - name: Effect
    effect: The first time the target uses a move action, main action, maneuver, or triggered action before the start of your next turn, your companion makes the following power roll before the target acts. If the target hasn't acted before the start of your next turn, they are frightened of your companion (save ends).
  - roll: Power Roll + Intuition
    tier1: 9 + I psychic damage; `I < WEAK` weakened (save ends)
    tier2: 13 + I psychic damage; `I < AVERAGE` weakened (save ends)
    tier3: 18 + I psychic damage; `I < STRONG` weakened (save ends)

```

