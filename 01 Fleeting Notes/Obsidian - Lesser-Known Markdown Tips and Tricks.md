---
title: 
aliases: 
tags:
  - Obsidian
state: in-progress
cssclasses: 
Image: 
dg-publish: true
dg-metatags:
  description: "Exploring the more obscure features of Obsidian Markdown formatting"
  og:image: https://i.imgur.com/LmCg5HX.png
---
## About

Not all of Obsidian's capabilities are thoroughly documented in the [Obsidian Help Docs](https://help.obsidian.md/Home).

That's not to say that the docs are lacking – they are an excellent primer on using Obsidian. What is lacking is some of the more particular, obscure workarounds inherent to [Markdown](https://www.markdownguide.org/) and HTML content in Markdown. These are generally for very specific use-cases.

## Display a Link as an Image

> [!caption|wmed right]
> 
> [![An image as a clickable link|wm-m](https://i.imgur.com/bdAW9ne.png)](https://morrowind-modding-with-massivejuice.vercel.app/)
> 
> A link displayed as an image – clicking the link will take you to the homepage. 

Want to create a button or an image that links to a different note or an external web page?

We can do this by wrapping an embedded image inside the square brackets (`[ ]`) of a standard [Markdown link](https://www.markdownguide.org/basic-syntax/#links). Inside the square brackets we would insert the Markdown for either:

- an embedded [Internal Image](https://help.obsidian.md/Linking+notes+and+files/Embed+files#Embed+an+image+in+a+note), e.g:

```
![[Engelbart.jpg]]
```

- an [External Image](https://help.obsidian.md/Editing+and+formatting/Basic+formatting+syntax#External+images), e.g:

```
![Engelbart](https://history-computer.com/ModernComputer/Basis/images/Engelbart.jpg)
```

### External Link

Using an image to link to an external web page:

**Eternal image:**

```Markdown 
[![image alt text](url to image)](https://www.some-website.com)
```

**Internal image** embedded via `wikilink`:

```Markdown
[![[wikilink to image.png]]](https://www.some-website.com)
```

### Internal Link

Using an image to link to an internal page does not work using the standard `[[wikilink]]` syntax. 

Instead, it is formatted like a Markdown link, with the exception that instead of a URL in the `(brackets)`, you would put the page name surrounded by `< >`. So, `[[page title]]`  would instead be written as `(<page title>)`

Here is the full formatting:

**Eternal image:**

```Markdown 
[![image alt text](url to image)](<page name>)
```

**Internal image** embedded via `wikilink`:

```Markdown
[![[wikilink to image.png]]](<page name>)
```

---

## Wikipedia-Style 'Inline Cleanup Tags'

Using the HTML `<sup>` (superscript) tag, we can create a Wikipedia-style [Inline Cleanup Tag](https://en.wikipedia.org/wiki/Template:Inline_cleanup_tags).

You may have seen them before while trawling a wiki article – they look like this:

- Some consider the Tribunal to be false gods. <sup>\[_[according to whom?](https://en.m.wikipedia.org/wiki/Wikipedia:Manual_of_Style/Words_to_watch#Unsupported_attributions)_\]</sup>
- Wulfharth, along with Dagoth Ur, led the Nordic and Orc forces into Morrowind. <sup>\[_[original research?](https://en.m.wikipedia.org/wiki/Wikipedia:No_original_research)_\]</sup>
- Nerevar was betrayed and murdered by the Tribunal. <sup>\[_[citation needed](https://en.m.wikipedia.org/wiki/Wikipedia:Citation_needed)_\]</sup>

> [!note|clean embed no-t] %% embed [[Inline Cleanup Tags]] %%
> 
> ![[MMW Inline Cleanup Tags#HTML Superscript Tags|clean]]

## Tables - lists and linebreaks

- https://www.markdownguide.org/hacks/#line-breaks-within-table-cells
- https://www.markdownguide.org/hacks/#lists-within-table-cells

## Investigate Further:
- [Adding titles to links](https://www.markdownguide.org/basic-syntax/#adding-titles "Markdown Guide")
- [Reference Style Links][1]

---

## External Links 
- [1]: <https://www.markdownguide.org/basic-syntax/#reference-style-links> "Markdown Guide - Basic Syntax#Reference-Style-Links"