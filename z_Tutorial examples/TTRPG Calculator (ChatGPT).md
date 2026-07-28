---
JumpInputStrength: 20
---

# Jump Calculator

**Character Strength:**`INPUT[number:JumpInputStrength]`

Long Jump with running start: `VIEW[{JumpInputStrength}]`
Long Jump from standing: `VIEW[{JumpInputStrength}/2]`
High Jump with running start: `VIEW[(({JumpInputStrength}-10)/2)+3]`
High jump from standing: `VIEW[round((({JumpInputStrength}-10)/2)+3)/2]`




```dataviewjs
// input field and button
dv.el("bold", "Input Strength: ")
const inputField = dv.el('input', "input field")
const btn = dv.el('button', "Calculate Jump Distances")

// template out the 4 results to remove 
dv.paragraph("Long jump with running start: - feet")
dv.paragraph("Long jump from standing: - feet")
dv.paragraph("High jump with running start: - feet")
dv.paragraph("High jump from standing: - feet")

// on-click event
btn.addEventListener('click', (event) => {
    event.preventDefault()

    // remove the last 4 results (or defaults)
    this.container.lastChild.remove()
    this.container.lastChild.remove()
    this.container.lastChild.remove()
    this.container.lastChild.remove()

    // calculate and format
    let strength = parseInt(inputField.value);
    let strMod = Math.floor((strength - 10) / 2);

    //display results 
    dv.paragraph("Long jump with running start: " + strength + " feet")
    dv.paragraph("Long jump from standing: " + (strength / 2) + " feet")
    dv.paragraph("High jump with running start: " + (strMod+3) + " feet")
    dv.paragraph("High jump from standing: " + ((strMod+3) / 2) + " feet")
});
```


## Heading
```dataviewjs
// Input field and button
dv.el("bold", "Input 4th Edition DC: ");
const inputField = dv.el('input', "input field");
const btn = dv.el('button', "Calculate 5th Edition DC");

// Template out the result to remove
dv.paragraph("5th Edition DC: -");

// On-click event
btn.addEventListener('click', (event) => {
    event.preventDefault();

    // Remove the last result (or default)
    this.container.lastChild.remove();

    // Calculate and format
    let fourthEditionDC = parseInt(inputField.value);

    // Convert to 5th Edition DC
    let levelOfMonster = fourthEditionDC / 2;
    
    // Use LevelOfMonster against the 5th edition proficiency bonus table to determine Proficiency Bonus (for example, assuming a simple linear relationship)
    // Replace this with your own logic based on your proficiency bonus table
    let proficiencyBonus = Math.ceil(levelOfMonster / 4);

    // Calculate 5th Edition DC
    let fifthEditionDC = levelOfMonster + proficiencyBonus;

    // Display result
    dv.paragraph("5th Edition DC: " + fifthEditionDC);
});
```

## 4e to 5e DC Convertor
```dataviewjs
// Input field and button
dv.el("bold", "Input 4th Edition DC: ");
const inputField = dv.el('input', "input field");
const btn = dv.el('button', "Calculate 5th Edition DC");

// Template out the result to remove
dv.paragraph("5th Edition DC: -");

// Proficiency bonus table
const proficiencyBonusTable = {
    1: 2,
    2: 2,
    3: 2,
    4: 2,
    5: 3,
    6: 3,
    7: 3,
    8: 3,
    9: 4,
    10: 4,
    11: 4,
    12: 4,
    13: 5,
    14: 5,
    15: 5,
    16: 5,
    17: 6,
    18: 6,
    19: 6,
    20: 6
};

// On-click event
btn.addEventListener('click', (event) => {
    event.preventDefault();

    // Remove the last result (or default)
    this.container.lastChild.remove();

    // Calculate and format
    let fourthEditionDC = parseInt(inputField.value);

    // Convert to 5th Edition DC
    let levelOfMonster = Math.floor(fourthEditionDC / 2);
    
    // Use LevelOfMonster against the 5th edition proficiency bonus table to determine Proficiency Bonus
    let proficiencyBonus = proficiencyBonusTable[levelOfMonster];

    // Calculate 5th Edition DC
    let fifthEditionDC = levelOfMonster + proficiencyBonus;

    // Display result (rounded down)
    dv.paragraph("5th Edition DC: " + Math.floor(fifthEditionDC));
});
```

## DC Calculator in 5e

```dataviewjs
// Input fields and button
dv.el("bold", "Enter Character Level: ");
const characterLevelInput = dv.el('input', { type: 'number', placeholder: 'Character Level' });

dv.el("bold", "Enter Difficulty Level (Very Easy, Easy, Medium, Hard, Very Hard, Nearly Impossible): ");
const difficultyInput = dv.el('input', { type: 'text', placeholder: 'Difficulty Level' });

const btn = dv.el('button', "Calculate DC");

// Template out the result to remove
dv.paragraph("Recommended DC: -");

// On-click event
btn.addEventListener('click', (event) => {
    event.preventDefault();

    // Remove the last result (or default)
    this.container.lastChild.remove();

    // Get input values
    let characterLevel = parseInt(characterLevelInput.value);
    let difficultyLevel = difficultyInput.value.toLowerCase(); // Convert to lowercase for case-insensitivity

    // Calculate DC based on specified difficulty level and character level
    let recommendedDC;

    switch (difficultyLevel) {
        case 'very easy':
            recommendedDC = characterLevel <= 3 ? 5 + characterLevel - 1 : 5 + 1 + Math.floor((characterLevel - 4) / 3);
            break;
        case 'easy':
            recommendedDC = characterLevel <= 3 ? 10 + characterLevel - 1 : 10 + 1 + Math.floor((characterLevel - 4) / 3);
            break;
        case 'medium':
            recommendedDC = characterLevel <= 3 ? 15 + characterLevel - 1 : 15 + 1 + Math.floor((characterLevel - 4) / 3);
            break;
        case 'hard':
            recommendedDC = characterLevel <= 3 ? 20 + characterLevel - 1 : 20 + 1 + Math.floor((characterLevel - 4) / 3);
            break;
        case 'very hard':
            recommendedDC = characterLevel <= 3 ? 25 + characterLevel - 1 : 25 + 1 + Math.floor((characterLevel - 4) / 3);
            break;
        case 'nearly impossible':
            recommendedDC = characterLevel <= 3 ? 30 + characterLevel - 1 : 30 + 1 + Math.floor((characterLevel - 4) / 3);
            break;
        default:
            // Default to medium difficulty if an invalid difficulty level is entered
            recommendedDC = characterLevel <= 3 ? 15 + characterLevel - 1 : 15 + 1 + Math.floor((characterLevel - 4) / 3);
            break;
    }

    // Display result
    dv.paragraph("Recommended DC: " + recommendedDC);
});
```