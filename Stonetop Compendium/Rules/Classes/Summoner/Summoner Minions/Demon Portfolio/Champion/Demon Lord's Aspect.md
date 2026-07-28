~~~ds-statblock
type: statblock
name: Demon Lord's Aspect
level: .
roles:
  - Champion
ancestry:
  - Abyssal
  - Demon
ev: 9 essence for one champion
speed: 5
size: 2
stamina: Your maximum Stamina
movement: Teleport
immunities: 
  - Corruption 5
weaknesses:
stability: 2
free_strike: 9
might: 2
agility: 5
reason: 5
intuition: 2
presence: 2
features:
  - type: feature
    feature_type: ability
    name: Free Strike Damage Type - Corruption
  - type: feature
    feature_type: ability
    name: 🗡️ Grasping Appendages 2d10 + 5 - Signature Ability
    icon: 🗡️
    usage: Main action
    keywords:
      - Magic
      - Strike
      - Weapon
    distance: 📐 Melee 5
    target: 🎯 Two creature or objects
    effects:
      - roll: Power Roll + 5
        tier1: 9 corruption damage; pull 2
        tier2: 12 corruption damage; pull 4
        tier3: 14 corruption damage; pull 5
        effect: A target pulled adjacent to the Aspect is grabbed.
  - type: feature
    feature_type: trait
    name: ⭐ Warping Strike
    icon: ⭐️
    effects:
      - effect: The Apsect's free strikes teleport the target 5 squares.
  - type: feature
    feature_type: trait
    name: ⭐ Champion's Ire
    icon: ⭐️
    effects:
      - effect: If the Apsect only targets one creature or object with a strike, they deal additional damage to the target equal to your Reason.
  - type: feature
    feature_type: ability
    usage: Free triggered action
    distance: 📐 Self
    target: 🎯 Self
    trigger: The Aspect takes damage from an enemy.
    name: ⭐ I Like Your Taste
    icon: ⭐️
    effects:
      - effect: The Apsect has a double edge on their next power roll. They can choose to give this benefit to an ally within your Summoner's Range instead.
  - type: feature
    feature_type: trait
    name: ⭐ Frenzy
    icon: ⭐️
    effects:
      - effect: When the Apsect is reduced to 0 Stamina, they make a free strike against each adjacent enemy before dying.
  - type: feature
    feature_type: trait
    name: ⭐ Level 10 Champion Advancement Feature - Size Increase
    icon: ⭐️
    effects:
      - effect: The Aspect is now size 3.
  - type: feature
    feature_type: trait
    name: 🔅 Level 10 Champion Advancement Feature - Reality Flense
    icon: ⭐️
    usage: Champion Action
    distance: 📐 20 burst
    target: 🎯 Self and each non-minion ally in the Area
    cost: 1 Eidos
    effects:
      - effect: Each target teleports up to their speed and makes a free strike. If a target has a Save Ends condition, they can inflict the condition onto a creature with their strike and end the condition on themself.
~~~


