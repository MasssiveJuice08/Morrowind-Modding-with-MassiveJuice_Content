---
state: completed
dg-publish: true
dg-metatags:
 description: "Workarounds for importing bugged Omnivore articles to Obsidian"
 og:image: https://i.imgur.com/LmCg5HX.png
---

## About

[![Omnivore.app Logo|right wsmall](https://i.imgur.com/0YszZiM.png)](https://omnivore.app/)

Some articles saved in [[Omnivore - Saving Articles for Citations in Obsidian|Omnivore]] do not render correctly in Obsidian. For example, the article [[Abbreviations - Web Accessibility Guidance project - NZ Government]] contains `<abbr>` HTML tags surrounded by `<code> </code>` tags so that it does not render the abbreviation, but Omnivore is not translating this to Markdown style \``code`\` surrounded by backticks. This causes the article highlights to render incorrectly in reading mode on Obsidian, and to break the associated web page on [my digital garden](https://morrowind-modding-with-massivejuice.vercel.app/).

As an alternative, I have added the `#omnivore-bug` label to problematic articles and in Omnivore's Obsidian plugin have added the filter `-label:omnivore-bug` so that those articles are not synced to Obsidian. Instead, I place the articles in this folder so I can still reference these sources within my digital garden.

### Can't you just edit the article in Obsidian?

No, syncing from Omnivore to Obsidian is one-way. If I make changes to the Markdown file of a synced article in Obsidian, those changes are not updated within Omnivore. Furthermore, when using the `Omnivore: Resync all articles` command in Obsidian, any manual changes made to the markdown file are reverted by Omnivore. 

Moving the problematic articles to a new folder and filtering them out of the sync with the `omnivore-bug` label allows me to safely make manual edits to the Markdown files.

### What then?

The recurring issue I have found is with HTML content within `<code> </code>` tags on websites not being placed within \``backticks`\` when synced to Obsidian. I can manually make the adjustments myself to place them within backticks.

### It's not all Omnivore's fault

As well as articles and documents, i also save forum comments and posts, such as a [[Benefit to using Acronym and Abbreviation HTML Tags - Stack Overflow|useful answer in a StackOverflow discussion]]. Code written in these is not guaranteed to be fenced with `<code>` tags, as the comment author may not need to worry about the comment system trying to render the HTML (depending on the forum).

These may also need to be manually entered.

## Omnivore Manual Entry articles:

```dataview
TABLE without ID file.link as "Note Title", file.mday as "Last Modified"
FROM #omnivore-bug
SORT file.name asc
```