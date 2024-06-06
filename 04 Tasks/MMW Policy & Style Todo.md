---
tags:
  - todo
  - MMW-Policy
  - MMW-Style
---
For later editing purposes, it could helpful to label those areas that you consider subjective as you have suggested. A useful way to mark these would be what Wikipedia calls ['inline-cleanup tags'](https://en.wikipedia.org/wiki/Template:Inline_cleanup_tags). If a sentence or a section is subjective and/or based on your opinion, add an empty wikilink `[[opinion]]` to the end.

You can format this as superscript like so `<sup>\[[[opinion]]\]</sup>` by placing `<sup> </sup>` HTML tags around it. To make the single square brackets render, place a backslash before them like `\[  \]`. Just tested this in Quartz and it works.

We can later create a page for `[[opinion]]` like the wikipedia page [Template:Opinion](https://en.wikipedia.org/wiki/Template:Opinion) and then those empty wikilinks you've added will link there.

**Example sentence with an inline cleanup tag**
```
This is my opinion <sup>\[[[opinion]]\]</sup>.
```
Note that you need to have a space before the last word and the first `<sup>`

--- 

Update: you can also make the citation italicised by adding a pair of underscores: `<sup>\[_[[opinion]]_\]</sup>`