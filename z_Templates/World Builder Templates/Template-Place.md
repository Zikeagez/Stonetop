---
tags:
  - Category/Place
MyContainer: "[[z_Templates/World Builder Templates/Template-Hub.md|Template-Hub]]"
MyCategory: Commerce
obsidianUIMode: preview
image: "Template_Place_Placeholder.png"
---

<%*

// 1) Prompt for Place name
const title = await tp.system.prompt("Enter Place Name", tp.file.title);
if (!title) return;
await tp.file.rename(title);

// 2) Gather all container notes from 1. World/Hubs
const containerFiles = tp.app.vault.getMarkdownFiles()
  .filter(f => f.path.startsWith("1. World/Hubs/"));

const placeholderLabel = "🌀 No Hub Selected";
const placeholderPath = "__placeholder__";

// 3) Build suggester options
const containerChoices = [placeholderLabel, ...containerFiles.map(f => f.basename)];
const containerValues  = [placeholderPath, ...containerFiles.map(f => f.path)];
const chosenPath       = await tp.system.suggester(containerChoices, containerValues, true);
if (!chosenPath) return;

// 4) Build wiki-link or fallback
let wikiLink = null;
if (chosenPath !== placeholderPath) {
  const alias = chosenPath.split("/").pop().replace(/\.md$/, "");
  wikiLink = `[[${chosenPath}|${alias}]]`;
}

// 5) Pick a category from your list
const categoryOptions = [
  "Commerce",
  "Agriculture",
  "Military",
  "Philosophy",
  "Industrial",
  "Nesting",
  "Government"
];
const chosenCat = await tp.system.suggester(categoryOptions, categoryOptions, true);
if (!chosenCat) return;

// 6) Write to frontmatter
setTimeout(() => {
  const file = tp.file.find_tfile(tp.file.path(true));
  if (!file) return;
  app.fileManager.processFrontMatter(file, fm => {
    fm["MyContainer"] = wikiLink ?? "None";
    fm["MyCategory"]  = chosenCat;
  });
}, 100);

%>

> [!NOTE] Parent Hub: `INPUT[suggester(optionQuery(#Category/Hub)):MyContainer]`

> [!column|no-title]
>> [!note|no-title]
>> ![[#Image|no-h clean]]
>
>> [!note|no-title] Place Name
>> ~~~meta-bind
>> INPUT[select(
>> option(1, ℹ️General Info),
>> option(2, 🏃‍♂️‍➡️NPCs),
>> option(3, 📝GM Notes),
>> class(tabbed)
>> )]
>> ~~~
>>>[!tabbed-box-maxh]
>>> >[!div-m|no-title]
>>> > ![[#General|no-h clean]]
>>>
>>> >[!div-m|no-title]
>>> > ![[#NPCs|no-h clean]]
>>>
>>> > [!div-m|no-title]
>>> > ![[#GM Notes|no-h clean]]
>>> 

> [!NOTE|no-title]
> ~~~meta-bind
> INPUT[select(
> option(1, 🛒Selling),
> option(2, 🪙Buying),
> option(3, 🛠️Services),
> option(4, 🤐Rumours),
> class(tabbed)
> )]
> ~~~
> >[!tabbed-box]
> > >[!div-m|no-title]
> > > ![[#Selling|no-h clean]]
> >
> > > [!div-m|no-title]
> > > ![[#Buying|no-h clean]]
> > 
> > > [!div-m|no-title]
> > > ![[#Services|no-h clean]]
> > 
> > > [!div-m|no-title]
> > > ![[#Rumours|no-h clean]]

---

# General

Select Settlement: `INPUT[suggester(optionQuery(#Category/Hub)):MyContainer]`
%% DISPLAYS NOTES THAT MATCH THE TAGS ABOVE %% 

Select Category: `INPUT[template-place-category][:MyCategory]`
%% MODIFY OPTIONS IN SETTINGS > COMMUNITY PLUGINS > META-BIND > EDIT TEMPLATES > template-place-category %%

This is the places description. 

# NPCs

`BUTTON[button_person]` The following people are associated with this place.

```base
properties:
  file.name:
    displayName: Star Systems Name
  note.MyCategory:
    displayName: Type of Star System
  note.char_race:
    displayName: Race
  note.char_gender:
    displayName: Gender
  note.char_age:
    displayName: Age
views:
  - type: cards
    name: Star Systems - Cards
    filters:
      and:
        - file.folder == "1. World/People"
        - list(MyContainer).contains(this)
        - char_status.contains("Alive")
    order:
      - file.name
      - char_age
      - char_gender
      - char_race
    image: note.image
  - type: table
    name: Star Systems - Table
    filters:
      and:
        - file.folder == "1. World/People"
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

# GM Notes

Make notes of what you need to track in the town here. 


# Selling

The following items are available for purchase. 

```dataviewjs
// This dataviewjs code grabs a random item(s) from the folder below. You can remove this if that's not useful. It's an example of what's possible. 
// 1. grab all pages in the folder
let pages = dv.pages('"2. Mechanics/CLI/items"').values;

// 2. shuffle
for (let i = pages.length - 1; i > 0; i--) {
  const j = Math.floor(Math.random() * (i + 1));
  [pages[i], pages[j]] = [pages[j], pages[i]];
}

// 3. take the first X where (0, X) should be the number of items to return
let pick = pages.slice(0, 1);

// 4. render table of clickable links + Gender
dv.table(
  ["Random Item", "cost", "weight"],
  pick.map(p => [
    dv.fileLink(p.file.path),        // clickable note link
    p.cost ?? "—",                  // frontmatter field (falls back to “—” if missing)
    p.weight ?? "—"                  // frontmatter field (falls back to “—” if missing)
  ])
);
```

# Buying

List of things this merchant will purchase. 

| Item   | Cost | Weight |
| ------ | ---- | ------ |
| Item 1 | 1gp  | L      |
| Item 2 | 1cp  | -      |

# Services

Services offered. 

| Item   | Cost | Weight |
| ------ | ---- | ------ |
| Service 1 | 1gp  | L      |
| Service 2 | 1cp  | -      |

# Rumours

Anything the party might over hear?

# Image
![[Template_Place_Placeholder.png|500]]

