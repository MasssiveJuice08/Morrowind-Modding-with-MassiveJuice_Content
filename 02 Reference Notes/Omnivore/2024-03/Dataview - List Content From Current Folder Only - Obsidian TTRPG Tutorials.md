---
id: 5ccd5a29-fff9-4902-9b99-613a4c9f371d
title: Dataview - List Content From Current Folder Only - Obsidian TTRPG Tutorials
author: unknown
tags:
  - Dataview
  - MMW-Policy/Structure
date_saved: 2024-03-20 22:18:24
site_name: obsidianttrpgtutorials.com
original_url: https://obsidianttrpgtutorials.com/Obsidian+TTRPG+Tutorials/Plugin+Tutorials/Dataview/Dataview+-+List+Content+From+Current+Folder+Only
---

## Dataview - List Content From Current Folder Only - Obsidian TTRPG Tutorials
#Omnivore

[Read on Omnivore](https://omnivore.app/me/dataview-list-content-from-current-folder-only-obsidian-ttrpg-tu-18e5b279431)
[Read Original](https://obsidianttrpgtutorials.com/Obsidian+TTRPG+Tutorials/Plugin+Tutorials/Dataview/Dataview+-+List+Content+From+Current+Folder+Only)

### Highlights

> This might be handy for limiting your queries to only return results from the current folder. 
> 
> `WHERE contains(file.folder, this.file.folder)`
> 
> ### Example 
> 
> ```pgsql
> ```dataview  
> TABLE WITHOUT ID link(file.name) AS "NPC Name", Gender, Race, Age, Location, AssociatedGroup  
> FROM "2. Mechanics/Non-Player Characters"
> WHERE contains(file.folder, this.file.folder)
> SORT file.mtime DESC
> LIMIT 10
> ```
> ``` [⤴️](https://omnivore.app/me/dataview-list-content-from-current-folder-only-obsidian-ttrpg-tu-18e5b279431#15532688-e905-4f78-a595-c964a49c553b)  ^15532688

