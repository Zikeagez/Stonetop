~~~ds-statblock
type: statblock
name: Dragon's Portent
level: .
roles:
  - Champion
ancestry:
  - Dragon
  - Elemental
ev: 9 essence for one champion
speed: 6
size: 2
stamina: Your maximum Stamina
movement: Fly
weaknesses:
immunities:
  - Affinity 5
stability: 2
free_strike: 9
might: 2
agility: 2
reason: 5
intuition: 5
presence: 2
features:
  - type: feature
    feature_type: ability
    name: Free Strike Damage Type - Affinity
  - type: feature
    feature_type: trait
    name: ⭐ Affinity
    icon: ⭐️
    effects:
      - effect: The Portent selects an affinity for one of the following damage types when they are summoned - acid, cold, corruption, fire, lightning, or poison. This type determines the Portent's affinity immunity and the damage type of theri abilities.
  - type: feature
    feature_type: ability
    name: 🗡️ Elemental Tail Swing 2d10 + 5 - Signature Ability
    icon: 🗡️
    usage: Main action
    keywords:
      - Charge
      - Melee
      - Strike
      - Weapon
    distance: 📐 Melee 2
    target: 🎯 Two creature or objects
    effects:
      - roll: Power Roll + Reason
        tier1: 9 affinity damage; push 2
        tier2: 12 affinity damage; push 4
        tier3: 14 affinity damage; push 6
        effect: A target pulled adjacent to the Aspect is grabbed.
  - type: feature
    feature_type: trait
    name: ⭐ Sealing Strike
    icon: ⭐️
    effects:
      - effect: The Portent's free strikes inflict `M < STRONG` slowed (save ends). While slowed this way, the target takes 1d6 affinity damage at the start of each of their turns.
  - type: feature
    feature_type: trait
    name: ⭐ Champion's Ire
    icon: ⭐️
    effects:
      - effect: If the Apsect only targets one creature or object with a strike, they deal additional damage to the target equal to your Reason.
  - type: feature
    feature_type: ability
    name: ⭐ Searing Wyrmscale
    icon: ⭐️
    effects:
      - effect: Whenever an adjacent creature deals damage to the Portent, they take 4 affinity damage.
  - type: feature
    feature_type: trait
    name: ⭐ Dragon Heart
    icon: ⭐️
    effects:
      - effect: Once per turn, the Portent can take 10 damage to allow you or an ally within your Summoner's Range to gain 1 heroic resource. This damage can't be reduced in any way.
  - type: feature
    feature_type: trait
    name: ⭐ Level 10 Champion Advancement Feature - Size Increase
    icon: ⭐️
    effects:
      - effect: The Aspect is now size 3.
  - type: feature
    feature_type: trait
    name: 🏁 Level 10 Champion Advancement Feature - A Breath Felt in a Hurricane
    icon: ⭐️
    keywords:
      - Area
      - Magic
      - Ranged
    usage: Champion Action
    distance: 📐 4 cube within 10
    target: 🎯 Each enemy and object in the area
    cost: 1 Eidos
    effects:
      - effect: 9 affinity damage. The damage ignores immunity. The affected area becomes difficult terrain. An enemy has affinity weakness 5 whiel occupying an affected square.
~~~


