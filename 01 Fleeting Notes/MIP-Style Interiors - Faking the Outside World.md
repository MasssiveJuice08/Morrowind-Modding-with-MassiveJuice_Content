---
state: in-progress
tags:
  - Secret-of-Vilmuhn
  - Far-From-the-Marsh
dg-metatags:
  description: ""
  og:image: https://i.imgur.com/LmCg5HX.png
dg-publish:
---

## About

In [[Secret of Vilmuhn - Home|Secret of Vilmuhn]] and [[Far From the Marsh - Home|Far From the Marsh]] I make use of fake exteriors, giving the illusion that the outside world is visible from an interior cell.

The approach is inspired by and similar to GrumblingVomit's [Morrowind Interiors Project](https://www.nexusmods.com/morrowind/mods/52237) (AKA 'MIP'), which is no surprise considering we work together on Vilmuhn. Where my approach differs however is that I do not set the interior cell to `Behave Like Exterior`. Treating the cell like an exterior removes the ability to change the cell's ambient light settings, which otherwise allow you to create moody, theatrical lighting for your interiors.

This is not without its drawbacks.

### Creating a Fake Exterior

The approach is roughly the same as MIP's - see the [Morrowind Modding Wiki](https://morrowind-modding.github.io/Guides/Interiors/Morrowind-Interiors-Project) guide - with a few differences:

- I use Greatness7's [Export Sphere](https://www.nexusmods.com/morrowind/mods/52245?tab=files) tool to create a single `.nif` of an exterior.
- Instead of letting the player fully see outside, I use OAAB Lighthole meshes to create blinding light, where only glimpses of the outside world are visible.

This approach is not perfect. The downside of using the cell's ambient light settings is that there is no sky - only an empty void.

[[Fake Skyboxes for Morrowind]]