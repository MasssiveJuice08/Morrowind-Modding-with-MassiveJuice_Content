---
title: MGE-XE Groundcover Research by OpenMW
aliases:
  - MGE-XE Groundcover Research by OpenMW
  - MGE-XE Groundcover
tags:
  - Groundcover
state: inbox
cssclasses: 
Image: 
dg-publish: 
dg-metatags:
  description: "A forum discussion by OpenMW devs documenting how MGE-XE handles groundcover. Ironically, this is the best source for documenting MGE-XE groundcover."
  og:image: https://i.imgur.com/LmCg5HX.png
---
[Original Post](https://forum.openmw.org/viewtopic.php?p=53197#p53197)

> "I looked at [MGE XE sources](https://github.com/Hrnchamd/MGE-XE) and did some research about how grass generation works in MGE.  
>   
> 1. MGE considers all meshes from Meshes/Grass folder as a grass and add all objects which use them to distant land cache during distant land generation.  
> 2. Grass density parameter shows probability for every grass instance from ESP to be included to distant land cache (yes, just a simple random).  
> 3. During game start, MGE loads all grass instances from cache to QuadTree.  
> The world in MGE has 4 quad trees: for near objects, far objects, very far objects and grass.  
> 4. Cull visitor cuts all grass instances on large distance.  
> 5. MGE selects meshes which are in camera frustrum.  
> 6. Then MGE uses [instancing](http://3dcgtutorials.blogspot.ru/2013/08/instancing-with-openscenegraph.html) to render grass.  
> Basically, MGE takes transforms from every grass instance with selected mesh, packs them all in a single array and calls the DrawIndexedPrimitive DirectX function (OpenGL has the glDrawElementsInstanced function which do a similar thing) for batching rendering.  
> Each transform is a 4x3 float matrix (in MGE - 48 bytes).  
> 7. Grass animation works as a shader which takes in account a wind speed and direction.  
> 8. MGE has a cap - only 8192 grass instances can be rendered in one time (the MaxGrassElements variable).  
>   
> Can we use a similar approach in OpenMW, or it is a too hackish or slow for us?"
> 
> \-  **[akortunov](https://forum.openmw.org/memberlist.php?mode=viewprofile&u=3643)** 2018-03-22

