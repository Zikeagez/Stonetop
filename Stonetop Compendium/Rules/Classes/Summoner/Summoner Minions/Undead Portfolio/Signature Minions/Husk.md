~~~ds-statblock
type: statblock
name: Husk
level: .
roles:
  - Signature Minion Defender
ancestry:
  - Undead
ev: 1 essence per minion summoned
speed: 5
size: 1M
stamina: 3
weaknesses:
immunities:
  - Damage 2, corruption R, poison R
movement:
stability: 0
free_strike: 1
might: 2
agility: 0
reason: -1
intuition: -1
presence: -1
features:
  - type: feature
    feature_type: ability
    name: Free Strike Damage Type - Sonic
  - type: feature
    feature_type: ability
    name: ⭐ Rotting Strike
    icon: ⭐
    effects:
      - name: 
        effect: The husk's melee free strikes inflict `M < WEAK` slowed (EoT). The potency increases by 1 for each additional husk adjacent to the target (maximum +2).
~~~

