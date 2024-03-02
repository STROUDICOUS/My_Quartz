---
share: "true"
---



> [!comment]
>  This is a comment


> [!empty]
> This quote should be hidden

>[!yellowwarning] 
>Yellow warning

> [!yellowwarning] [[Coercive Financial Ultimatum|Coercive Financial Ultimatum]]
> tes


>[!objectif]
>Test


- Custom callouts are defined by CSS
- The css can be partially duplicated in Obsidian AND in GitHub Quartz [Custom callouts](https://github.com/STROUDICOUS/My_Quartz/blob/v4/quartz/styles/custom/callouts.scss)

- 1. Use admonition plugin to create new callout. Don' go too light or dark on the colour.
![[Custom Callouts and Email Inline Comments.png|Custom Callouts and Email Inline Comments.png]]
- 2. Go to Appearance>CSS Snippets.
 ![[Custom Callouts and Email Inline Comments-1.png|Custom Callouts and Email Inline Comments-1.png]]
- 3. Copy the CSS
- 4. Go to [GitHub/Custom callouts](https://github.com/STROUDICOUS/My_Quartz/blob/v4/quartz/styles/custom/callouts.scss)
- 5. Pastein this template
```js
    &[data-callout="yellowwarning"] { //replace from first part from admonition
    --color: rgb(var(--callout-color));//LEAVE
    --border: rgb(var(--callout-color));//LEAVE
    --bg: rgba(var(--callout-color), 0.3);//LEAVE
    --callout-color: 167, 164, 88;//Copy from Admonition CSS
    --callout-icon: url('data:image/svg+xml; utf8, ****** '); //Replace***** with <svg>*/<svg> from Admonition CSS
  }
```
- 6. Paste in the code from the Admonition CSS and match the syntax as in the // comments above, noting the folliwing:
	- remove `.callout`
	- Put in the `&` So `&[data-callout="yellowwarning"]`
	- CopyPaste the `<svg>*/<svg>` From the Admonition CSS
	- CopyPaste the colour `--callout-color: 255, 252, 163;`
