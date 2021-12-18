---
title: "Fate Explorer"
description: "Eine Hilfsapp für Pen & Paper Abende mit dem Schwarzen Auge"
draft: false
discontinued: false
image : "images/projects/fateexplorer.webp"
bg_image: "images/feature-bg.jpg"
category: [ "R", "Shiny" ]
information:
  - label : "Aufgaben"
    info : "Design, Entwicklung"
  - label : "Tools"
    info : "Inkscape, R-Studio, Krita"
  - label : "Projektstatus"
    info : "Fortschreitend"
  - label : "Fertigkeiten"
    info : "R / Shiny; HTML / CSS; DSA&nbsp;5"
  - label : "Kunde"
    info : "Das-Schwarze-Auge Spieler"
---

## DSA Fate Explorer

An interface to roll the dice based on the ["dark eye" rule system](https://ulisses-regelwiki.de/index.php/home.html) (version 5) based on [R shiny](https://shiny.rstudio.com/).


### Features

* Eigenschaftswürfe
* Fertigkeitswürfe einschließlich Zaubern und Wundern
* Kampfwürfe
  * *NEU* in Version 2 FateExplorer kann die Umgebungsfaktoren in Kampfsituationen berücksichtigen, also Entfernungen, Bewegung, oder Sichtbarkeit.
  * *NEU* in Version 2: Initiativewürfe
* Import [Optolith Characterbögen](https://optolith.app/en/)
  * *NEU* in Version 2: FateExplorer kann eigene Waffen importieren.
* Anzeige der Erfolgswahrscheinlichkeiten
* Zweisprachig (Englisch und Deutsch - kann aktuell über das Skript angepasst werden)


### Screenshots

![Bild von den Fertigkeitswürfe](/images/projects/fe_screenshot_skill.jpg)

![Bild von den Kampfwürfen](/images/projects/fe_screenshot_combat.jpg)



### Einschränkungen im gegenwärtigen Stand

* Nutzer müssen die Modifikatoren selbst berechnen und setzen. Sonderfertigkeiten, Zustände, etc. werden noch nicht berücksichtigt.
* DIe Sprache lässt sich nur übers Skript ändern.
    * FE kennt leider nicht alle Regeln im Kampf, z.B. eine 19 wäre bei einer improvisierten ein Patzer. Der FE kennt solche Ausnahmeregeln nicht.
* FE kennt keine Regeln, die spezifisch für einzelne Waffen sind.

<br/>
<a href="https://github.com/SigurdJanson/Fate-Explorer">Zu finden auf Github</a>

