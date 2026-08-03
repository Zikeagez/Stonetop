# Working with PDFs
PDF's can be dragged into your vault. They will default to the folder you have defined as your 'Attachments' folder. Alternatively, you drag them into specific folders or use your operating system to copy them into specific folders.

To link to a .pdf you can use similar syntax to an image or link. 

`[[PZ09500-18e - LTiBA]]`

If you would like to display a preview of the link within the note, use a ! at the Start

`![[PZ09500-18e - LTiBA]]`

To link to a psecific page this is the required syntax. 
Instead of trying to remember this; make a template!

`[[PZ09500-18e - LTiBA#page=5]]`

# Example

This will link to a pdf and skip to page 3. The ! tells Obsidian to display a preview in this note. Without the ! it will just display a link that you can hover/click.
![[Playbook - The Fox (1-up).pdf#page=3]]
[[Playbook - The Fox (1-up).pdf#page=3]]

# PDF Catalogue (Requires Dataview Plugin)

You can use DatabiewJS to query pdf's within your vault. This code will list all pdfs within your vault.

```dataviewjs
const pdfFiles = app.vault.getFiles().filter(file => file.extension === 'pdf')
dv.list(pdfFiles.map(file => dv.fileLink(file.path)))
```

# PDF Catalogue with Folder (Requires Dataview Plugin)

You can use DatabiewJS to query pdf's within your vault. This code will list all pdfs within a specific folder. In this example the 'z_Assets' folder is being referenced.

```dataviewjs
const pdfFiles = app.vault.getFiles().filter(file => file.extension === 'pdf' && file.path.includes('z_Assets'))
dv.list(pdfFiles.map(file => dv.fileLink(file.path)))
```