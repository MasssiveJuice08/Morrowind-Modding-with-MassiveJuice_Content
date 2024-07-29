---
state: completed
tags:
  - Quartz/UI
  - MMW-Dev/CSS
dg-publish: true
dg-metatags:
  description: Notes on the idea of adding a horizontal nav-bar at the top of the page in the Morrowind Modding Wiki
  og:image: https://i.imgur.com/LmCg5HX.png
---
## About

The Quartz site [Notkesto](https://notes.camargomau.com/) has added a horizontal navigation bar pinned to the top of the web page, with links to content categories. This structure could suit the [[Morrowind Modding Wiki - Home|Morrowind Modding Wiki]] well as a quick way to locate the top-level wiki categories (such as 'Guides', 'Modding Tools', 'Programmers Reference', 'Contributing' etc).

A mobile [[Hamburger Menu for Quartz]] could make this redundant, but the two could also complement each other.

## Implementation 

Notkesto adds the custom component [LinksHeader.tsx](https://github.com/camargomau/notkesto-site/blob/v4/quartz/components/LinksHeader.tsx) which controls the navbar. Style is determined with [quartz/components/styles/linksHeader.scss](https://github.com/camargomau/notkesto-site/blob/v4/quartz/components/styles/linksHeader.scss).
