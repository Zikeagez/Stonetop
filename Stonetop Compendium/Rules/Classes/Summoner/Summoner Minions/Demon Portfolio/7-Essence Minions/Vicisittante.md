~~~ds-statblock
type: statblock
name: Vicisittante
level: .
roles:
  - Minion Harrier
ancestry:
  - Abyssal
  - Demon
ev: 7 essence for two minions
speed: 10
size: 2
stamina: 17|17
movement:
weaknesses:
  - Holy 1
stability: 0
free_strike: 7
might: 3
agility: 4
reason: 0
intuition: 0
presence: -1
features:
  - type: feature
    feature_type: ability
    name: Free Strike Damage Type - Psychic
  - type: feature
    feature_type: ability
    name: 🏹 Cerebral Flay 2d10 + R - Signature Ability
    icon: 🏹
    usage: Main action
    keywords:
      - Magic
      - Psionic
      - Strike
    distance: Melee 1
    target: 🎯 One creature or object per minion
    effects:
      - roll: Power Roll + Reason
        tier1: 7 psychic damage; `P < WEAK` weakened (save ends)
        tier2: 11 psychic damage; `P < AVERAGE` weakened (save ends)
        tier3: 16 psychic damage; `P < STRONG` weakened (save ends)
        effect: A target weakened by this ability is always considered flanked by the vicisittante regardless of position until the condition ends.
  - type: feature
    feature_type: trait
    name: ⭐ Soulsight
    icon: ⭐️
    effects:
      - effect: Each creature adjacent to the blightling can't be hidden from them.

~~~


