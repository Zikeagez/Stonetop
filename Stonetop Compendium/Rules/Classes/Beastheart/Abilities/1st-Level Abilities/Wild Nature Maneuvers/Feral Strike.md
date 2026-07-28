```ds-feature
type: feature
feature_type: ability
name: Feral Strike
flavor: "\"Your companion lunges into the fray, attacking wildly with teeth, claws, or other weapons.\""
keywords:
  - Area
  - Companion
  - Melee
  - Strike
  - Weapon
usage: Main action
distance: 📐 1 burst
target: Each creature in the area
effects:
  - name: Effect
    effect: Your companion moves up to a number of squares equal to their Intuition score straight toward the closest enemy they are aware of, avoiding damaging terrain and ending the movement when they are adjacent to that enemy. Your companion then makes the following power roll.
  - roll: Power Roll + Might
    tier1: 1 + M damage
    tier2: 3 + M damage
    tier3: 4 + M damage
  - name: Effect
    effect: >-
      This ability gains the following benefit based on your wild nature.
      
   
      - **Guardian:** Each enemy target is taunted by your companion until the start of your next turn.

      - **Prowler:** Each enemy target is weakened until the start of your next turn.

      - **Punisher:** Your companion slides each target up to a number of squares equal to their Might score.

      - **Spark:** This strike deals cold, fire, lightning, or sonic damage. You gain 1 surge.
```

