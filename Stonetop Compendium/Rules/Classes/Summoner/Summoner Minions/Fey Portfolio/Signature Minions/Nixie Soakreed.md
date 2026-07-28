~~~ds-statblock
type: statblock
name: Nixie Soakreed
level: .
roles:
  - Signature Minion Controller
ancestry:
  - Fey
ev: 1 essence per minion summoned
speed: 5
size: 1T
stamina: 1
weaknesses:
movement: Swim
stability: 0
free_strike: 1
might: -2
agility: -1
reason: 0
intuition: 2
presence: 1
features:
  - type: feature
    feature_type: ability
    name: ⭐ Water Weird
    icon: ⭐
    effects:
      - name: 
        effect: Once per turn during their move action, each nixie under your control can teleport to a body of water within 5. The soakreed can't teleport into water created by their own soaking bog.
  - type: feature
    feature_type: trait
    name: ⭐ Soaking Bog
    icon: ⭐️
    effects:
      - effect: The area within 1 square of the soakreed is filled with swampy water. An enemy that starts their turn in the area is `A < WEAK` slowed (EoT). The potency increasees by 1 for each additional soaking bog the target occupies (maxium +2).
  - type: feature
    feature_type: trait
    name: ⭐ Miniscule
    icon: ⭐
    effects:
      - effect: The soakreed has cover while occupying a larger creature's space.


~~~

