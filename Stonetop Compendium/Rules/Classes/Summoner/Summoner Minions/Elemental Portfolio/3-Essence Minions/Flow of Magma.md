~~~ds-statblock
type: statblock
name: Flow of Magma
level: .
roles:
  - Minion Harrier
ancestry:
  - Fire
  - Earth
ev: 3 essence for two minions
speed: 5
size: 1L
stamina: 6|6
movement: Climb
immunities:
  - Fire R
stability: 2
free_strike: 4
might: 2
agility: -2
reason: 0
intuition: 0
presence: 1
features:
  - type: feature
    feature_type: ability
    name: Free Strike Damage Type - Fire
  - type: feature
    feature_type: ability
    name: 🗡️ Molten Strike 2d10 + `R`
    icon: 🗡️
    usage: Main action
    keywords:
      - Magic
      - Melee
      - Strike
    distance: Melee 2
    target: 🎯 One creature or object per minion
    effects:
      - roll: Power Roll + Reason
        tier1: 4 fire damage; shift 3
        tier2: 6 fire damage; shift 4
        tier3: 8 fire damage; shift 5
        effect: Each square that the flow shifts into becomes wreathed in flames until th estart of the flow's next turn. An enemy that enters an affected square takes 2 damage.
  - type: feature
    feature_type: trait
    name: ⭐ Eruption
    icon: ⭐️
    effects:
      - effect: When the flow is reduced to 0 Stamina, they launch lava into an area equal to 1 + their size within 5 squares. The affected area becomes difficult terain for enemies until the end of the encounter. An enemy that enters an affected square or starts their turn takes `A < AVERAGE` 4 fire damage.


~~~


