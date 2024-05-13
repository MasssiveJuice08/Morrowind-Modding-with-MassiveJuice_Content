---
tags:
  - Obsidian
  - MMW-Dev/CSS
---
Source: https://discord.com/channels/686053708261228577/702656734631821413/1126511749517017108

```css
/* Remove Title */
.callout[data-callout="infobox-person"] .callout-title {
  display: none;
}

/* Backgground */
.callout[data-callout="infobox-person"] {
  background: var(--bg1);
  border-radius: 12px;
  width: 260px;
  margin-left: 20px;
  padding: 0px;
  float: right;
}

/* Spacing */
.callout[data-callout="infobox-person"] p {
  margin-block-start: 0px;
  margin-block-end: 0px;
}

/* Title with background */
.callout[data-callout="infobox-person"] h1 {
  margin: 4px 0px 4px 2px;
  font-size: 24px;
  text-align: center;
  border-radius: 4px;
  background-color: rgba(255, 255, 255, 0.1);
  padding: 4px;
}

.callout[data-callout="infobox-person"] h2 {
  margin: 4px 0px 4px 2px;
  font-size: 20px;
  text-align: center;
  border-radius: 4px;
  background-color: rgba(255, 255, 255, 0.1);
  padding: 4px;
}

/* Table */
.callout[data-callout="infobox-person"] table {
  margin: 0px !important;
  width: 100%;
  font-size: 16px;
}

.callout[data-callout="infobox-person"] th {
  border: none !important;
}

.callout[data-callout="infobox-person"] td {
  border: none !important;
  padding-left: 12px; 
  padding-right: 0px;
  vertical-align: top;
}
```