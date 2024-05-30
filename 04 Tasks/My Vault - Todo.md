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

## In-Progress Notes

> [!cards|2 dataview] Fleeting Notes:
```dataview
TABLE without ID file.link as "Note Title", file.mday as "Last Modified"
FROM "01 Fleeting Notes"
WHERE state = "in-progress"
SORT file.name asc
```
