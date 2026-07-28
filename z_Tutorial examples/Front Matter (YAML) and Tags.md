---
NoteType: Junk
key: value
key2: value2
key3:
  - one
  - two
  - three
key4:
  - four
  - five
  - six
aliases:
  - NoteName1
  - NoteName2
  - Fred
  - Bob
  - Goblin
  - Goblins
tags:
  - Tag4
  - Tag5
---

#Tag1 
#Tag2

Front MAtter is a vital and important element of Obsidian 
#Tag3

#LeetVideo




[[Front Matter (YAML) and Tags|Goblins]]
[[Front Matter (YAML) and Tags|Bob]]
[[Front Matter (YAML) and Tags|Fred]]
## Dataview Usage
`=this.key2`

```dataview
list from #Tag1
where NoteType = "Junk"
```



```dataview
table key, key2, key3, key4
from #Tag3
```