~~~ds-statblock
type: statblock
name: Faded Blightling
level: .
roles:
  - Minion Support
ancestry:
  - Abyssal
  - Demon
ev: 7 essence for two minions
speed: 5
size: 1L
stamina: 17|17
movement: Fly
weaknesses:
  - Holy 1
stability: 0
free_strike: 7
might: 0
agility: 0
reason: -1
intuition: 4
presence: 3
features:
  - type: feature
    feature_type: ability
    name: Free Strike Damage Type - Corruption
  - type: feature
    feature_type: ability
    name: 🏹 Blighted Strike 2d10 + R - Signature Ability
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
        tier1: 7 corruption damage; `P < WEAK` bleeding (EoT)
        tier2: 11 corruption damage; `P < AVERAGE` bleeding (EoT)
        tier3: 16 corruption damage; `P < STRONG` bleeding (EoT)
        effect: Instead of taking damage, you or an ally targeted by this ability impose a double bane on the next strike that targets them.
  - type: feature
    feature_type: trait
    name: ⭐ Wilted Wings
    icon: ⭐️
    effects:
      - effect: The blightling must land on the ground at the end of their turn or fall prone.
  - type: feature
    feature_type: trait
    name: ⭐ Soulsight
    icon: ⭐️
    effects:
      - effect: Each creature adjacent to the blightling can't be hidden from them.

~~~


