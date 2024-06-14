---
state: in-progress
tags:
  - MW-May-Modathon-2024
  - MOC
  - Far-From-the-Marsh
cssclasses: 
dg-publish: true
dg-metatags:
  description: Far From the Marsh a Morrowind mod by MassiveJuice
  og:image: https://i.imgur.com/LmCg5HX.png
aliases:
  - Far From the Marsh
---
## Far From the Marsh

A mod for Week One of the 2024 Morrowind Modathon theme, **'Mysticism and Prophecy'**

![[MJ_FFTM_v0-5_img_01.png|banner]]

> [!quote|mark color-green] **~ Jeelish-Tar** <br>18th of Rain's Hand, 3E 427
> "Honored marshbrother, 
> 
> This land is cold to us, but we find solace here. Sheogorad is a harsh place. It has taught us much. We trace paths whispered by wise ones. This next day, I delve into currents as deep as Hist roots. If swept away, know I walked where our swamps touch the sky. Guard our marsh-kin, as the Hist watches over us. 
> 
> Walk well, wet and dry."

---

> [!infobox|n-th] 
> # Far From the Marsh
> ![[May-Modathon-2024_Week-One-Banner.png]]
> ###### Requirements
> | Mod Name | Notes |
> | ---- | ---- |
> | [OAAB_Data](https://www.nexusmods.com/morrowind/mods/49042) | Required |
> | [Tamriel_Data](https://www.nexusmods.com/morrowind/mods/44537) | Required |
> 
> ##### Hosted on
> | Name | Notes |
> | ---- | ---- |
> | [NexusMods](https://www.nexusmods.com/morrowind/mods/54612) | Initial release |
> | [GitHub](https://github.com/MasssiveJuice08/Far-From-The-Marsh) | WIP builds |
> 
> ##### Status
> 
> > [!success|title-center] In active development

### Description:

A Mages Guild member studying hidden patterns of Mysticism and prophecy has gone missing. Explore their cave retreat in Sheogorad for clues about their ultimate fate. A quest outline and initial dialogue has been written, but not yet implemented; this will be added in a future update. In the meantime, you can expect a pretty cave with the mage's journal and some environmental story-telling.   
  
You can find their cave west of Dagon Fel. Follow the road west and then north to a river crossing – the cave entrance is on the left.

<br>
<br>
<br>

---

### Project Notes - Contents

> [!example|bg-gray c-orange]+ Project Notes
> 
> ```dataview
> TABLE without ID file.link as "Note Title", file.mday as "Last Modified"
> FROM #MW-May-Modathon-2024 AND -#Omnivore AND -#MOC
> SORT file.name asc
> ```

> [!example|bg-gray c-orange]+ Reference Notes
> 
> ```dataview
> TABLE without ID file.link as "Note Title", file.mday as "Last Modified"
> FROM #MW-May-Modathon-2024 AND #Omnivore
> SORT file.name asc
> ```

### To-Do

**Quest**:
- [ ] Jeelish-Tar's journal starts at Sun's Dawn month but talks of New Year; change month to Morning Star.
- [ ] Finish quest dialogue and add journal entries
- [ ] Add dialogue for Andre Maul and Dagon Folk NPCs
- [ ] Script travel to Andre Maul's Island

**World**
- [ ] Finish Jeelish-Tar's cave
- [ ] Find reference images of vanilla and TR Mages Guild interiors for ideas on cluttering
- [ ] Find Reference images of cave-dwelling rogue mages


### Creative Process - Quest Writing:

I experimented with using ChatGPT to develop the questline for this mod. In my personal life I have worked a lot on [Devised Theatre](https://en.wikipedia.org/wiki/Devised_theatre), and it's the type of creative process I am most familiar with, as opposed to scriptwriting. I have found ChatGPT to be a surprisingly capable tool for simulating the devising process: I fill the role of director and [dramaturg](https://en.wikipedia.org/wiki/Dramaturge), while ChatGPT is the devisor. I offer creative prompts and direction, and undertake research on lore and Morrowind's writing style. Once all the initial writing has been completed by ChatGPT, my intention is to then act as the story editor, tweaking and refining the material. 

I found this process to be a useful way of distilling my thoughts. I have ADHD, so I tend to jump from one idea/topic to another very quickly where my interests lead me (hence why I have started four separate modding projects over the course of a year and have technically finished... none?). If I'm taking decent notes along the way, I end up with a vast pile of resources and creative ideas to draw from - the difficulty then lies in tying all those together, which can feel like a monumental task (especially when just starting out). It's quite easy to be endlessly stuck in the research phase of a project and never venture into the next step of actually creating content. With ChatGPT, I have been able to feed it all my scattered, dense notes, and it immediately provides me with clear, instantaneous output.

Working with ChatGPT as a creative 'partner' makes for a very frictionless creative relationship: 
- no waiting impatiently for a response 
- immediate output 
- (humbly) responsive to creative feedback

Friction is not always a bad thing in creative processes though; conflict and restrictions can be great stimuli for creativity. With that in mind, what ChatGPT lacks as a creative tool that a human does not is:
- It can take creative feedback, but it won't give it back (unprompted, that is) - if you give it a creative prompt for a terrible script idea, _it'll do it anyway_, for better or worse.
- It won't fight for _'its'_[^1] own ideas and argue that theirs should be used over your own ideas 

Given the AI's limitations, seeking critical feedback from other modders will remain an important step in the creative process. That being said, ChatGPT has proved to be an invaluable tool in the initial developmental stage.

### Brainstorming the Concept

Week one theme - **'Mysticism and Prophecy'**

![[MW May Modathon 2024 Week 1 - Brainstorming#^b8a259]]

### Pitching the Concept to ChatGPT

![[MW May Modathon 2024 Week 1 - Plot Outline#^47b3b1]]

### Plot Outline

![[MW May Modathon 2024 Week 1 - Plot Outline#^b118af]]

### Journal Entries

![[MW May Modathon 2024 Week 1 - Jeelish-Tar's Journal#^f97303]]

---

[^1]: I say 'its' ideas because authorship and plagiarism with AI language models is a contentious subject. Despite how thorough my creative prompts and feedback are, what ChatGPT outputs might still be a facsimile of someone else's work. Therefore, the final stage of heavily editing ChatGPT's work _without_ its input is a vital step to ensure that the final product is not unwitting plagiarism