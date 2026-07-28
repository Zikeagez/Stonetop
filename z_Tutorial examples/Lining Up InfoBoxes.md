/* Custom CSS for Three-Column Layout in Admonition Block */
.admonition-statblock .callout-content {
    font-size: 16px !important;
    overflow-x: visible;
    column-count: 3;
    column-gap: 20px;
/*   padding: 25px; */
    padding: var(--callout-content-padding);
    background-color: var(--callout-content-background);
}

.admonition-statblock .callout-title {
    justify-content: center;
}

/* Force a break at the first h2, after the stats and before traits or actions */
.admonition-statblock .callout-content h2:nth-of-type(2n) {
    break-before: column; /* This creates a break before the first h2 */
}

/* Additional styling for other elements if needed */
.admonition-statblock ul, .admonition-statblock ol {
    padding-left: 10px;
}

.admonition-statblock table {
    width: 85%;
    page-break-inside: avoid; /* Avoid breaking tables across columns */
}

.admonition-statblock table th, .admonition-statblock table td {
        font-size: 14px;
}

/* Hide content when the callout is collapsed */
.admonition-statblock.is-collapsed .callout-content {
    display: none;
}



> [!columns|3 no-t]
> >[!info] Recent Notes 
> >First Content 
>
>> [!info] Session Notes 
>> Second Content 
>
>>[!info] Calendar 
>> Third Content



>[!columns|3 no-t]
>>[!InfoBox]
>># `=this.file.name`
>>![[BrynshanderImage.jpg]]
>>[[BrynshanderImage.jpg|Pop Out]] 
>>##### Geography
>>Type | Stat |
>>---|---|
>>Type | `=this.type`|
>>Size |`=this.size`|
>>Region |`=this.region`|
>>##### Politics
>>Type | Stat |
>>---|---|
>>GovtType | `=this.politics`|
>>Ruler |`=this.leader`|
>>Defense |`=this.defense`|
>>##### Organizations 
>>Type | Stat |
>>---|---|
>>Guilds & Groups |`=this.guildsgroups`|
>>##### Society
>>Type | Stat |
>>---|---|
>>Population |`=this.population`|
>>Races |`=this.commonraces`|
>>Temples |`=this.religion`|
>>##### Commerce
>>Type | Stat |
>>---|---|
>>Exports | `=this.exports`|
>>Imports |`=this.imports`|
>
>>[!InfoBox]
>># `=this.file.name`
>>![[BrynshanderImage.jpg]]
>>[[BrynshanderImage.jpg|Pop Out]] 
>>##### Geography
>>Type | Stat |
>>---|---|
>>Type | `=this.type`|
>>Size |`=this.size`|
>>Region |`=this.region`|
>>##### Politics
>>Type | Stat |
>>---|---|
>>GovtType | `=this.politics`|
>>Ruler |`=this.leader`|
>>Defense |`=this.defense`|
>>##### Organizations 
>>Type | Stat |
>>---|---|
>>Guilds & Groups |`=this.guildsgroups`|
>>##### Society
>>Type | Stat |
>>---|---|
>>Population |`=this.population`|
>>Races |`=this.commonraces`|
>>Temples |`=this.religion`|
>>##### Commerce
>>Type | Stat |
>>---|---|
>>Exports | `=this.exports`|
>>Imports |`=this.imports`|