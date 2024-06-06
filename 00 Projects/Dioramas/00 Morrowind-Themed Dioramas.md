---
dg-metatags:
  description: Morrowind-Themed Dioramas by MassiveJuice
  og:image: https://i.imgur.com/LmCg5HX.png
dg-publish: true
tags:
  - MOC
  - Dioramas
dg-pinned: true
title: Morrowind-Themed Dioramas
aliases:
  - Morrowind-Themed Dioramas
---

## About

Morrowind-themed Dioramas I have created. My goal in future is to create a diorama each year as a first-place prize for the Morrowind Modjam.

> [!cards|1 dataview] 
> ```dataview 
> TABLE WITHOUT ID 
> 	"![|sban cover hmicro](" + image + ")" as Image, 
> 	"**"+ link(file.link, title) + "**" AS "Column Name", 
> created AS "Modified"
> FROM "00 Projects/Dioramas" AND -"00 Projects/Dioramas/00 Morrowind-Themed Dioramas"
> SORT created desc
> ```