~~~ds-statblock
type: statblock
name: Avatar of Death
level: .
roles:
  - Champion
ancestry:
  - Undead
ev: 9 essence for one champion
speed: 6
size: 2
stamina: Your maximum Stamina
movement: Fly
weaknesses:
immunities:
  - Corruption 5
  - Poison 5
stability: 3
free_strike: 9
might: 5
agility: 2
reason: 5
intuition: 2
presence: 2
features:
  - type: feature
    feature_type: ability
    name: Free Strike Damage Type - Holy
  - type: feature
    feature_type: ability
    name: 🏹 Culling Scythe 2d10 + 5 - Signature Ability
    icon: 🏹
    usage: Main action
    keywords:
      - Melee
      - Strike
      - Weapon
    distance: 📐 Melee 2
    target: 🎯 Two creature or objects
    effects:
      - roll: Power Roll + 5
        tier1: 9 corruption damage; `M < WEAK` bleeding (save ends)
        tier2: 12 corruption damage; `M < AVERAGE` bleeding (save ends)
        tier3: 14 corruption damage; `M < STRONG` bleeding (save ends)
        effect: If the target is a creature that isn't a leader or a solo and they are still bleeding at the end of the encounter, they instantly die.
  - type: feature
    feature_type: trait
    name: ⭐ Revelation Strike
    icon: ⭐️
    effects:
      - effect: The Avatar's melee free strikes `P < WEAK` instantly reduce a winded non-leader or solo creature to 0 Stamina, including targets winded by the strike.
  - type: feature
    feature_type: trait
    name: ⭐ Champion's Ire
    icon: ⭐️
    effects:
      - effect: If the Apsect only targets one creature or object with a strike, they deal additional damage to the target equal to your Reason.
  - type: feature
    feature_type: ability
    name: ⭐ Dust and Rot
    icon: ⭐️
    distance: 📐 1 burst
    target: 🎯 Each enemy in the burst
    trigger: The Avatar takes damage
    effects:
      - effect: Roll `M < AVERAGE` weakened (EoT).
  - type: feature
    feature_type: trait
    name: ⭐ Drifting Spirit
    icon: ⭐️
    effects:
      - effect: The Avatar is unaffected by difficult terrain and damage from forced movement.
  - type: feature
    feature_type: trait
    name: ⭐ Level 10 Champion Advancement Feature - Size Increase
    icon: ⭐️
    effects:
      - effect: The Aspect is now size 3.
  - type: feature
    feature_type: trait
    name: 🏁 Level 10 Champion Advancement Feature - Gravemaker
    icon: ⭐️
    usage: Champion Action
    keywords:
      - Area
      - Magic
      - Ranged
    distance: 📐 5 x 3 line within 1
    target: 🎯 Each enemy and object in the line
    cost: 1 Eidos
    effects:
      - effect: 9 holy damage. Each target is vertically pulled a number of squares equal to their size straight down, ignoring stability. If the target would be force moved into the ground, they are buried beneath the ground instead.
~~~


