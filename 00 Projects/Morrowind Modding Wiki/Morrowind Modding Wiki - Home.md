---
state: in-progress
tags:
  - MMW
  - MOC
dg-publish: true
dg-pinned: true
dg-metatags:
  description: My personal notes on contributing to the Morrowind Modding Wiki
  og:image: https://i.imgur.com/LmCg5HX.png
aliases:
  - Morrowind Modding Wiki
---

![[MMW_Logo.png|hm-sm center]]

---

## About:

The [Morrowind Modding Wiki](https://morrowind-modding.github.io/) is a community project that aims to collect and centralise community knowledge on Morrowind modmaking. 

Content is authored in [Obsidian.md](https://obsidian.md/) and published online using [Quartz](https://quartz.jzhao.xyz/).

### Members:

- Greatness7 
- S3ctor
- MassiveJuice

### Contributors

- MelchiorDahrk
- GrumblingVomit
- Zackhasacat

## My own notes on the wiki:

During development I have been taking my own notes (helped greatly by [Omnivore.app](https://omnivore.app/). I have published these here to my site for easier sharing

### Fleeting Notes

Brief notes capturing an idea

```dataview
TABLE without ID file.link as "Note Title", file.mday as "Last Modified"
FROM "01 Fleeting Notes" AND (#MMW OR #MMW-Dev OR #MMW-Style OR #MMW-Policy) AND -#Omnivore AND -#MOC 
SORT file.name asc
```

### Omnivore Notes:

Highlights of articles and forum posts saved with Omnivore. Many but not all contain my own annotations.

```dataview
TABLE without ID file.link as "Note Title", file.mday as "Last Modified"
FROM #MMW OR #MMW-Dev OR #MMW-Style OR #MMW-Policy AND #Omnivore AND -#MOC
SORT file.name asc
```