```base
properties:
  file.name:
    displayName: List of People in Place
views:
  - type: cards
    name: People - Cards
    filters:
      and:
        - file.folder == "2. World/People"
        - list(MyContainer).contains(this)
        - char_status.contains("Alive")
    order:
      - file.name
    image: note.image
  - type: table
    name: People - Table
    filters:
      and:
        - file.folder == "2. World/People"
        - list(MyContainer).contains(this)
        - char_status.contains("Alive")
    order:
      - file.name
    sort:
      - property: file.name
        direction: DESC
    columnSize:
      file.name: 182

```