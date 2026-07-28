~~~ds-statblock
type: statblock
name: Celestial Attendant
level: .
roles:
  - Champion
ancestry:
  - Fey
ev: 9 essence for one champion
speed: 7
size: 2
stamina: Your maximum Stamina
movement: Fly, Hover
weaknesses:
immunities:
  - Damage 2
stability: 0
free_strike: 9
might: 2
agility: 2
reason: 5
intuition: 2
presence: 5
features:
  - type: feature
    feature_type: ability
    name: Free Strike Damage Type - Poison
  - type: feature
    feature_type: ability
    name: 🏹 Pixie Swarm 2d10 + 5 - Signature Ability
    icon: 🏹
    usage: Main action
    keywords:
      - Magic
      - Ranged
      - Strike
    distance: 📐 Ranged 10
    target: 🎯 Two creature or objects
    effects:
      - roll: Power Roll + 5
        tier1: 9 affinity damage; slide 3
        tier2: 12 affinity damage; slide 5
        tier3: 14 affinity damage; slide 6
        effect: An ally targeted by this ability can, instead, spend a Recovery and shift the slide amount.
  - type: feature
    feature_type: trait
    name: ⭐ Neurotoxic Strike
    icon: ⭐️
    effects:
      - effect: A creature that takes damage from the ATtendant's free strike is `I < AVERAGE` unable to establish line of effect beyond 3 squares (EoT).
  - type: feature
    feature_type: trait
    name: ⭐ Champion's Ire
    icon: ⭐️
    effects:
      - effect: If the Apsect only targets one creature or object with a strike, they deal additional damage to the target equal to your Reason.
  - type: feature
    feature_type: ability
    name: ⭐ Celestial Bell
    icon: ⭐️
    distance: Self
    target: 🎯 Self
    trigger: The Attendant takes damage from an enemy.
    effects:
      - effect: The Attendant rings a bell, and you summon a signature minion into an unoccupied space adjacent to the Attendant.
  - type: feature
    feature_type: trait
    name: ⭐ Pixie Bouqet
    icon: ⭐️
    effects:
      - effect: The Attendant starts their turn with temporary Stamina equal to 2 x the number of fey minions within 1 square of them. This temporary Stamina lasts until the start of their next turn.
  - type: feature
    feature_type: trait
    name: ⭐ Level 10 Champion Advancement Feature - Size Increase
    icon: ⭐️
    effects:
      - effect: The Aspect is now size 3.
  - type: feature
    feature_type: trait
    name: ⭐ Level 10 Champion Advancement Feature - A Shower of Dust
    icon: ⭐️
    usage: Champion Action
    distance: 🔅 20 burst
    target: 🎯 Self and each noon-minion ally in the area
    cost: 1 Eidos
    effects:
      - effect: Each target gains 20 temporary Stamina and receives the benefits of one of your Flash Powder effects until the end of their next turn.
~~~


