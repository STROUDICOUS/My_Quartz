---
myCodeProperty: const page = dv.current();dv.table(["**To**", "**Cc**"], [[page.To, page.CC]]);
icon: FiCode
To:
  - "[[person1]]"
  - "[[Adrienne Jeffrey|Adrienne Jeffrey]]"
  - "[[Bob and Mary Smart]]"
CC:
  - "[[person3]]"
DateTime: 2005-05-05T05:05:00
share: "true"
---
```dataviewjs
const page = dv.current();
dv.table(["**To**", "**Cc**"], [[page.To, page.CC]]);

``` 

```dataviewjs
///////TRANSCLUDED EMAIL TO AND CC TABLE
const specificNotePage = dv.page("50 Queens Avenue/meta/Transcluded Email To and CC Table.md"), codeString = specificNotePage?.file.frontmatter.myCodeProperty;
codeString ? eval(codeString) : dv.paragraph("No code found in the frontmatter of the specified note."), error => dv.paragraph("Error executing dynamic code: " + error.toString());
```


| To                                   | Cc                          |    
| ------------------------------------ | --------------------------- | 
| [[Taghrid Choucair Vizoso\|Taghrid]] | [[Paul Stroud\|Paul]]       |  
|                                      | [[Hazem El Akhnawy\|Hazem]] |
```dataviewjs
// Initialize the Markdown table string with headers
let markdownTable = "| To | CC |\n| --- | --- |\n";

// Function to extract text from wikilink item
function extractText(item) {
    if (!item) return "NONE";
    // Match the pattern [[Link|Text]] or [[Link]]
    const match = item.match(/\[\[(?:[^\]\|]*\|)?([^\]]+)\]\]/);
    return match ? match[1] : item; // Return the text part if match is found
}

// Fetch "To" and "CC" from the current file's frontmatter
const { To, CC } = dv.current().file.frontmatter;

// Determine the maximum count of items in either "To" or "CC" for iteration
const maxCount = Math.max(To?.length || 0, CC?.length || 0);

// Populate the table rows based on the position in the arrays
for (let i = 0; i < maxCount; i++) {
    const toItem = To && i < To.length ? '[[' + extractText(To[i]) + ']]': "";
    const ccItem = CC && i < CC.length ? '[[' + extractText(CC[i]) + ']]': "";
    markdownTable += `| ${toItem} | ${ccItem} |\n`;
}

// Display the Markdown table as a paragraph
dv.paragraph(markdownTable);


```

![[Pasted image 20240226140003.png]]