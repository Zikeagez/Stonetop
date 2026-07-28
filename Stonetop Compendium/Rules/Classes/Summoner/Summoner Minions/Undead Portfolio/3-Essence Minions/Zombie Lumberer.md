~~~ds-statblock
type: statblock
name: Zombie Lumberer
level: .
roles:
  - Minion Defender
ancestry:
  - Undead
ev: 3 essence for two minions
speed: 5
size: 2
stamina: 8|8
movement:
weaknesses: 
immunities:
  - Corruption R, poison R
stability: R
free_strike: 1
might: 2
agility: -2
reason: 0
intuition: 0
presence: 1
features:
  - type: feature
    feature_type: ability
    name: ⭐ Zombie Clutch
    icon: ⭐
    effects:
      - name: 
        effect: The lumberer's melee free strikes inflict `M < AVERAGE` grabbed. A creature or object that starts their turn grabbed by the lumberer takes corruption damage equal to your Reason.
  - type: feature
    feature_type: trait
    name: ⭐ Death Grasp
    icon: ⭐️
    effects:
      - effect: When the lumberer is reduced to 0 Stamina, they can latch onto an adjacent enemy before being destroyed. The enemy is `M < STRONG` restrained (EoT)

~~~

