---
title: "Fate Explorer"
description: "A \"dark eye\" pen & paper support app"
draft: false
discontinued: false
image : "images/projects/fateexplorer.webp"
bg_image: "images/feature-bg.jpg"
category: [ "R", "Shiny" ]
information:
  - label : "What I do"
    info : "Concept, Design, Implementation"
  - label : "Tools used"
    info : "Inkscape, R-Studio, Krita"
  - label : "Status"
    info : "Iterating"
  - label : "Skills"
    info : "R / Shiny; HTML / CSS; DSA&nbsp;5"
  - label : "Client"
    info : "The Dark Eye Community"
---

## DSA Fate Explorer

An interface to roll the dice based on the ["dark eye" rule system](https://ulisses-regelwiki.de/index.php/home.html) (version 5) based on [R shiny](https://shiny.rstudio.com/).


### Features

* Ability rolls
* Skill rolls incl. routine checks for mundane, magical or blessed skills
* Combat rolls
  * *NEW* in version 2 FateExplorer can consider the combat situation like weapons range, movement, or visibility.
  * *NEW* in version 2: initiative rolls
* Import [Optolith character sheets](https://optolith.app/en/)
  * *NEW* in version 2: FateExplorer can import user-defined weapons.
* Display of probabilities for different results
* Bilingual (English and German - can be changed in the code of the script)


### Screenshots

![Image of the skill roll tab](/images/projects/fe_screenshot_skill.jpg)

![Image of the combat roll tab](/images/projects/fe_screenshot_combat.jpg)



### Limitations at Current State of Development

* Users set the modifiers manually in the UI of the app and roll the dice. The character sheet import does not support special abilities, states, conditions, etc. 
* Language can only be changed in the source code of the script.
* FE is still ignorant of some very pecial rules for weapons; e.g. rolling a 19 with an improvised weapon is actually a botch but FE is not aware of that.
* FE does not know rules that are specific for a weapon.

<br/>
<a href="https://github.com/SigurdJanson/Fate-Explorer">Find on Github</a>

