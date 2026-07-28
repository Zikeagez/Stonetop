~~~ds-statblock
type: statblock
name: Principle of the Swamp
level: .
roles:
  - Minion Brute
ancestry:
  - Elemental (Green, Water, Rot)
ev: 5 essence for three minions
speed: 4
size: 2
stamina: 5|5|5
movement: Swim
weaknesses: 
immunities: 
  - Corruption R
  - poison R
stability: R
free_strike: 4
might: 3
agility: -2
reason: 0
intuition: 2
presence: -2
features:
  - type: feature
    feature_type: ability
    name: ⭐ Encroaching Strike
    icon: ⭐
    effects:
      - name: Encroaching Strike
        effect: The principle's melee free strikes have a distance of R and incflict `M < STRONG` grabbed. The principle can have an unlimited number of creatures or objects grabbed. A creature grabbed by this strike has their normal speed, but can't move farther away from the principle.
  - type: feature
    feature_type: trait
    cost: 1 Essence
    name: ⭐ Sludgefoot
    icon: ⭐️
    effects:
      - effect: When the principle is reduced to 0 Stamina, the area within 1 square of the principle becomes difficult terrain for enemies until the end of the encounter. An enemy that ends their turn in the affected area is pulled 4 toward the center of the area.

~~~

