---
tags:
  - Category/Quest
MyContainer: []
MyCategory:
image: "Template_Quest_Placeholder.png"
obsidianUIMode: preview
questObtained:
questStatus: Not Started
questGiver:
questLocationObtained:
questSessionObtained:
questNotes:
questLootAvail:
questLookEarned:
NoteIcon: quest
---
<%*

// 1) Prompt for Quest name
const poiName = await tp.system.prompt("Enter Quest Name", tp.file.title);
if (!poiName) return;
await tp.file.rename(poiName);

// 2) Gather region notes
const regionFiles = tp.app.vault.getMarkdownFiles()
  .filter(f => f.path.startsWith("1. World/Regions/"));

const placeholderLabel = "🌀 No Region Selected";
const placeholderPath = "__placeholder__";

// 3) Prompt to choose a container region
const regionChoices = [placeholderLabel, ...regionFiles.map(f => f.basename)];
const regionValues  = [placeholderPath, ...regionFiles.map(f => f.path)];
const chosenPath    = await tp.system.suggester(regionChoices, regionValues, true);
if (!chosenPath) return;

// 4) Build wiki-link or fallback
let regionLink = null;
if (chosenPath !== placeholderPath) {
  const regionAlias = chosenPath.split("/").pop().replace(/\.md$/, "");
  regionLink = `[[${chosenPath}|${regionAlias}]]`;
}

// 5) Write into frontmatter
setTimeout(() => {
  const file = tp.file.find_tfile(tp.file.path(true));
  if (!file) return;
  app.fileManager.processFrontMatter(file, fm => {
    fm["MyContainer"] = regionLink ?? "None";
  });
}, 100);

%>

> [!NOTE] Parent Region: `INPUT[inlineListSuggester(optionQuery(#Category/Hub),optionQuery(#Category/Region),optionQuery(#Category/Place),optionQuery(#Category/PointofInterest)):MyContainer]`
%% DISPLAYS NOTES THAT MATCH THE TAGS ABOVE %% 

> [!column|no-i no-t]
>> [!info|no-title] Map
>> ![[Template_Quest_Placeholder.png]]
>
>> [!note|no-title] Town Name
>> ~~~meta-bind
>> INPUT[select(
>> option(1, 🏆Quest Info),
>> option(2, 🕵️‍♀️Quest Details),
>> option(3, 📝GM Notes),
>> class(tabbed)
>> )]
>> ~~~
>>>[!tabbed-box-maxh]
>>> >[!div-m|no-title]
>>> > ![[#Quest Info|no-h clean]]
>>>
>>> >[!div-m|no-title]
>>> > ![[#Quest Details|no-h clean]]
>>>
>>> > [!div-m|no-title]
>>> > ![[#GM Notes|no-h clean]]
>>> 


> [!NOTE|no-title] 
> ~~~meta-bind
> INPUT[select(
> option(1, 🏡Backstory),
> option(2, 🍎Planning),
> option(3, 🙎‍♂️People),
> class(tabbed)
> )]
> ~~~
>>[!tabbed-box|div-m]
>>>[!div-m|no-title]
>>> ![[#Backstory|no-h clean]]
>>
>>> [!div-m|no-title]
>>> ![[#Planning|no-h clean]]
>>
>>> [!div-m|no-title]
>>> ![[#People|no-h clean]]



---
# Quest Info

Provide a summary of the quest here. 

- [ ] Obtain the quest
- [ ] Embark on an epic journey
- [ ] Complete the quest
- [ ] Roll in epic loot

# Quest Details


Date Obtained: `INPUT[datePicker:questObtained]` 
Status: `INPUT[inlineSelect(option(Not Started), option(In Progress), option(Complete)):questStatus]` 
Quest Giver: `INPUT[suggester(optionQuery(#Category/People)):questGiver]` 
Quest Location: `INPUT[suggester(optionQuery(#Category/Hub)):questLocationObtained]` 
Session Obtained: `INPUT[suggester(optionQuery(#Category/Journal)):questSessionObtained]` 
Available Loot: `INPUT[suggester(optionQuery(#item)):questLootAvail]` 
Acquired Loot: `INPUT[suggester(optionQuery(#item)):questLookEarned]` 

# GM Notes

Make notes of what you need to track in the region here. 

# Backstory

Describe the backstory of the quest here. Why is it important for the party to complete?

# Planning

Plan your quest out here. 

# People

`BUTTON[button_person]` The following people are associated with this quest.

```base
properties:
  file.name:
    displayName: People Name(s)
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
        - list(Connected_Quests).contains(this)
        - char_status == "Alive"
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
        - list(Connected_Quests).contains(this)
        - char_status == "Alive"
    order:
      - file.name
    sort:
      - property: file.name
        direction: DESC
    columnSize:
      file.name: 182

```


