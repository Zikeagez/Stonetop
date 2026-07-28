~~~ds-statblock
type: statblock
name: Pixie Belladonix
level: .
roles:
  - Minion Artillery
ancestry:
  - Fey
ev: 7 essence for two minions
speed: 6
size: 1T
stamina: 16|16
movement: Fly, hover
weaknesses:
immunities:
  - Poison R
stability: 0
free_strike: 8
might: -2
agility: 2
reason: 4
intuition: 0
presence: 4
features:
  - type: feature
    feature_type: ability
    name: Free Strike Damage Type - Poison
  - type: feature
    feature_type: ability
    name: 🏹 A Thorn, Woe to the Pricked 2d10 + R - Signature Ability
    icon: 🏹
    usage: Main action
    keywords:
      - Magic
      - Ranged
      - Strike
    distance: Ranged 15
    target: 🎯 One creature or object per minion
    effects:
      - roll: Power Roll + Reason
        tier1: 8 poison damage; `I < WEAK` restrained (save ends)
        tier2: 12 poison damage; `I < AVERAGE` restrained (save ends)
        tier3: 17 poison damage; `I < STRONG` restrained (save ends)
        effect: A target restrained by this ability is trapped in a poison-fueled haze and considers each creature within 1 square of them to be an enemy until the condition ends.
  - type: feature
    feature_type: trait
    name: ⭐ Miniscule
    icon: ⭐️
    effects:
      - effect: The belladonix has cover while occupying a larger creature's space.

~~~


