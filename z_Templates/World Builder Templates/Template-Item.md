---
tags:
  - Category/Galaxy
obsidianUIMode: preview
MyContainer:
image: "Template_Galaxy_Placeholder.png"
---
<%*
const hasTitle = !tp.file.title.startsWith("NewGalaxy");
let title;
if (!hasTitle) {
    title = await tp.system.prompt("Enter Galaxy Name");
    await tp.file.rename(title);
} else {
    title = tp.file.title;
}
_%>

> [!NOTE] Parent:

> [!column|no-i no-t]
>> [!info|no-title] Map
>> ![[Template_Galaxy_Placeholder.png]]
>
>> [!note|no-title] Town Name
>> ~~~meta-bind
>> INPUT[select(
>> option(1, ℹ️General Info),
>> option(2, 🌐Galaxy Details),
>> option(3, 📝GM Notes),
>> class(tabbed)
>> )]
>> ~~~
>>>[!tabbed-box-maxh]
>>> >[!div-m|no-title]
>>> > ![[#General Info|no-h clean]]
>>>
>>> >[!div-m|no-title]
>>> > ![[#Planet Details|no-h clean]]
>>>
>>> > [!div-m|no-title]
>>> > ![[#GM Notes|no-h clean]]
>>> 

> [!NOTE|no-title]
> ~~~meta-bind
> INPUT[select(
> option(1, 🗺️Star Systems),
> class(tabbed)
> )]
> ~~~
> >[!tabbed-box]
> > >[!div-m|no-title]
> > > ![[#Star Systems|no-h clean]]
> >

---
# General Info

This is the planet description. 

# Planet Details

**Dominant Races:**  

# GM Notes

Make notes of what you need to track in the region here. 

# Star Systems

`BUTTON[button_starsystem]` **Continents**  Large continuous landmasses that contain regions.

```base
properties:
  file.name:
    displayName: Star Systems Name
  note.MyCategory:
    displayName: Type of Star System
views:
  - type: cards
    name: Star Systems - Cards
    filters:
      and:
        - file.folder == "1. World/Star Systems"
        - list(MyContainer).contains(this)
    order:
      - file.name
    image: note.image
  - type: table
    name: Star Systems - Table
    filters:
      and:
        - file.folder == "1. World/Star Systems"
        - list(MyContainer).contains(this)
    order:
      - file.name
    sort:
      - property: file.name
        direction: DESC
    columnSize:
      file.name: 182

```

