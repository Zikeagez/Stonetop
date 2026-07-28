~~~ds-statblock
type: statblock
name: The Boil
level: .
roles:
  - Hazard Support
ancestry:
  - Fixture
ev: .
stamina: 20 + your level
size: 2
stability: 0
free_strike: 0
might: 0
agility: 0
reason: 0
intuition: 0
presence: 0
features:
  - type: feature
    feature_type: ability
    name: ⭐ Hunter Thrush
    icon: ⭐
    effects:
      - name: 
        effect: Each enemy that starts their turn within 3 squares of the boil is `I < AVERAGE` taunted (EoT) by the boil, or `I < WEAK` taunted (EoT) by the boil and can't move further from it.
  - type: feature
    feature_type: trait
    name: ⭐ Oh, It Pops
    icon: ⭐️
    effects:
      - effect: When the boil is destroyed, each enemy within 3 squares of the boil takes acid damage equal to your level and is `A < STRONG` weakened (save ends).
  - type: feature
    feature_type: trait
    name: ⭐ Level 5 Fixture Advancement Feature - Soul Rancor
    icon: ⭐
    effects:
      - effect: You gain a surge the first time in a round that your demon minions deal 3 or more damage to a creature while you have line of effect to the boil. You can choose to give the surge to an ally who also has line of effect to the boil.
  - type: feature
    feature_type: trait
    name: ⭐ Level 9 Fixture Advancement Feature - Size Increase
    icon: ⭐
    effects:
      - effect: The boil is now size 3
  - type: feature
    feature_type: trait
    name: ⭐ Level 9 Fixture Advancement Feature - Fester Field
    icon: ⭐
    effects:
      - effect: Each non-abyssal enemy that starts their turn within 3 squares of the boil takes 5 corruption damage.
~~~

