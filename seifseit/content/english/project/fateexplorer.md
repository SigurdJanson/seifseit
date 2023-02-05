---
title: "Fate Explorer"
description: "A \"dark eye\" pen & paper support app"
draft: false
discontinued: false
image : "images/projects/fateexplorer.webp"
bg_image: "images/feature-bg.webp"
category: [ "Blazor / C#" ]
information:
  - label : "What I do"
    info : "Concept, Design, Implementation"
  - label : "Tools used"
    info : "Visual Studio; Inkscape, Krita; Git"
  - label : "Status"
    info : "Iterating"
  - label : "Skills"
    info : "C# / Blazor; HTML5 / CSS3; DSA&nbsp;5"
  - label : "Target Group"
    info : "The Dark Eye Community"
---

## DSA Fate Explorer

An app to roll the dice based on the ["dark eye" rule system](https://ulisses-regelwiki.de/index.php/home.html) (version 5). The Fate Explorer makes it easier to handle the rules and helps you to focus on your gameplay, your character and your story.


### Features

* Ability rolls
* Skill rolls incl. routine checks for mundane, magical or blessed skills
* Combat rolls
  * Attack and parry, dodge, initiative
  * Left and right hand; two-handed
* Energy management with life, astral energy and karma points.
* Calendar with holidays (i.e. fixed holidays) and phases of Mada.
* The **bazaar** with hundreds of items and a merchant to haggle the prize
* Bilingual (English and German)
* Import [Optolith character sheets](https://optolith.app/en/)
  * Including user-defined weapons.


### Screenshots

{{< figure src="/images/projects/fe_screenshot_ability_en.webp" title="Ability rolls" alt="Image of the main character page" width="46%" link="/images/projects/fe_screenshot_ability_en.webp" target="_blank">}}

{{< figure src="/images/projects/fe_screenshot_combat_en.webp" title="Combat rolls" alt="BImage of the combat roll tab" width="46%" link="/images/projects/fe_screenshot_combat_en.webp" target="_blank">}}



### Limitations at Current State of Development

* Users set the modifiers manually in the UI of the app and roll the dice. The character sheet import supports only limited special abilities and no states or conditions, etc. 
* FE is still ignorant of some very special rules; e.g. rolling a 19 with an improvised weapon is actually a botch but FE is not aware of that.
* FE does not know rules that are specific for a weapon.

<br/>
<a href="https://github.com/SigurdJanson/FateExplorer">Project page on Github</a>

