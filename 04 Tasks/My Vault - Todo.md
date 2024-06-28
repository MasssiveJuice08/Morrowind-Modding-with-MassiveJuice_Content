---
tags:
  - todo
state:
---
## Tasks

- [x] Add a true/false property to indicate if a note is completed or 'processed' or not
	- [x] consider extending this to Omnivore template, using `{{state}}` values of if article is 'reading' or 'completed'
- [x] add template for blog post notes incorporating things from [daily note style](https://dannb.org/blog/2022/obsidian-daily-note-template/#fn:1).
	- [x] Add 'previous/next' links to top of template, perhaps incorporating a [Dataview query](https://forum.obsidian.md/t/dataviewjs-snippet-showcase/17847/21)
- [ ] Customise Omnivore article template further
	- [ ] Remove duplicate title 
	- [ ] add `{{description}}`: make it more obvious this is someone else's content I have annotated
- [ ] Onnivore - do colored highlights work now?
- [ ] Article on using CS with MO2

## Inbox

```dataview
TABLE without ID file.link as "Note Title", file.mday as "Last Modified"
FROM "01 Fleeting Notes" OR "02 Reference Notes"
WHERE state = "inbox"
SORT file.name asc
```

## In-Progress Notes

```dataview
TABLE without ID file.link as "Note Title", file.mday as "Last Modified"
FROM "01 Fleeting Notes"
WHERE state = "in-progress"
SORT file.name asc
```

## Omnivore In-Progress 'Reading'

```dataview
TABLE without ID file.link as "Note Title", file.mday as "Last Modified"
FROM "02 Reference Notes"
WHERE state = "reading"
SORT file.name asc
```