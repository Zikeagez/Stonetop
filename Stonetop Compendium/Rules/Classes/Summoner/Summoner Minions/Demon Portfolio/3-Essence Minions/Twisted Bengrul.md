~~~ds-statblock
type: statblock
name: Twisted Bengrul
level: .
roles:
  - Minion Hexer
ancestry:
  - Abyssal
  - Demon
ev: 3 essence for two minions
speed: 5
size: 1L
stamina: 5|5
movement: 
weaknesses: 
  - Holy 1
stability: 1
free_strike: 4
might: 2
agility: 1
reason: -1
intuition: -1
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Free Strike Damage Type - Psychic
  - type: feature
    feature_type: ability
    name: 🏹 Mind Twist 2d10 + `R`
    icon: 🏹
    usage: Main action
    keywords:
      - Magic
      - Ranged
      - Strike
    distance: Ranged 5
    target: 🎯 One creature or object per minion
    effects:
      - roll: Power Roll + Reason
        tier1: 4 damage; `P < WEAK` twisted (save ends)
        tier2: 6 dmaage; `P < AVERAGE` twisted (save ends)
        tier3: 8 damage; `P < STRONG` twisted (save ends)
        effect: A twisted target can't take advantage of edges or search for hidden creatures until the condition ends.
  - type: feature
    feature_type: trait
    name: ⭐ Soulsight
    icon: ⭐️
    effects:
      - effect: Each creature adjacent to the ensnarer can't be hidden from them.


~~~


