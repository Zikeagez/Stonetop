```statblock
name: string
size: string
type: string
subtype: string
alignment: string
ac: number
hp: number
hit_dice: string
speed: string
stats: [number, number, number, number, number, number]
saves:
  - <ability-score>: number
skillsaves:
  - <skill-name>: number
damage_vulnerabilities: string
damage_resistances: string
damage_immunities: string
condition_immunities: string
senses: string
languages: string
cr: number
spells:
  - <description>
  - <spell level>: <spell-list>
traits:
  - name: Example Name
    desc: This is an example description
actions:
  - name: Example Action
    desc: "Example description: +7 to hit, reach 5ft. one target. Hit 7 (1d6 + 4) piercing damage"
legendary_actions:
  - name: Example Reaction
    desc: "Example Description"
bonus_actions:
  - name: <trait-name>
    desc: <trait-description>
  - ...
reactions:
  - name: Example Reaction
    desc: "Example description"
```

