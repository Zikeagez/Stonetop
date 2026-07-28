```ds-feature
type: feature
feature_type: ability
name: Omnomnom
cost: 5 Ferocity
flavor: What do you have in your mouth? No! Bad boy!
keywords:
  - Companion
  - Melee
  - Strike
  - Weapon
usage: Main action
distance: 📐 Melee 1
target: 🎯 One creature
effects:
  - name: Special
    effect: This ability targets only creatures who are grabbed and are your companion's size or smaller.
  - roll: Power Roll + Might
    tier1: 6 + M damage; `M < WEAK` the target is swallowed 
    tier2: 10 + M damage; `M < AVERAGE` the target is swallowed 
    tier3: 14 + M damage; `M < STRONG` the target is swallowed

  - name: Effect
    effect: A swallowed creature shares your companion's space, is grabbed and restrained, and has line of effect only to your companion. Nothing has line of effect to the swallowed creature.

  - name:
    effect: Once per round at the start of your turn, the swallowed creature takes acid damage equal to 1 + your companion's Might score. If the swallowed creature escapes the grab, your companion immediately regurgitates the creature, who lands prone in an unoccupied square adjacent to your companion. Your companion can also regurgitate a swallowed creature as a free maneuver. Your companion can have only one creature swallowed at a time.
```

