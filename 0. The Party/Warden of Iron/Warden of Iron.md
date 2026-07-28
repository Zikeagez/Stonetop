```base
properties:
  note.char_race:
    displayName: Race
  note.char_gender:
    displayName: Gender
  note.char_age:
    displayName: Age
  note.level:
    displayName: Level
  note.char_class:
    displayName: Class
views:
  - type: table
    name: Table
    filters:
      and:
        - file.folder == "0. The Party/Warden of Iron"
        - file.name != "Warden of Iron"
    order:
      - file.name
      - level
      - char_age
      - char_class
      - char_gender
      - char_race
    sort:
      - property: level
        direction: ASC

```