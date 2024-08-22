---
title: Extracting TES3 Cells by Region in JSON with JQ
aliases:
  - JQuery Command to Extract Cells by Region
  - Extracting TES3 Cells by Region in JSON with JQ
tags:
  - Groundcover
  - JSON
  - JQuery
  - Tes3conv
state: completed
cssclasses: 
Image: 
dg-publish: true
dg-metatags:
  description: ""
  og:image: https://i.imgur.com/LmCg5HX.png
---
By using a VS-Code plugin like [vscode-jq](https://marketplace.visualstudio.com/items?itemName=dandric.vscode-jq) in combination with a JSON-formatted TES3 plugin from [Tes3conv](https://github.com/Greatness7/tes3conv), data can be extracted and dumped to a new plugin.

## About

This is an alternative to [Tes3cmd]() `dump`, suggested by **Greatness7**, while I was running into issues trying to get it to dump cells by region. I could get it to dump cells with the default name "Ascadian Isles Region" (populated when an exterior cell has a region but is not explicitly named), but not explicitly named cells like `Pelagiad` which belonged to the aforementioned region.

Running the below JQ command extracts the cells by region from a JSON-formatted TES3 plugin:

```jq
[.[] | select(.type == "Header" or .region == "Ascadian Isles Region")]
```

Note: The region name can be substituted, and `"Header"` does not need to be included.