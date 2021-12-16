---
title: "CSV Importer"
description: "CSV Import für Shiny Apps"
discontinued: false
draft: false
image : "images/projects/csv-import.webp"
bg_image: "images/feature-bg.jpg"
category: [ "R", "Shiny" ]
information:
  - label : "Aufgaben"
    info : "Konzept, Design, Entwicklung"
  - label : "Tools"
    info : "R-Studio, Inkscape"
  - label : "Projektstatus"
    info : "alpha"
  - label : "Fertigkeiten"
    info : "R / Shiny; HTML / CSS"
  - label : "Kunde"
    info : "Shiny App Entwickler"
---


Dieses [`R`](https://www.r-project.org/) Package beinhaltet ein [Shiny](https://shiny.rstudio.com/) Modul mit den Funktionen, die man braucht, um CSV Dateien zu importieren. Shiny Apps müssen kein eigenes UI dafür bereits stellen und können einfach auf dieses Modul zurückgreifen. Nutzer sind flexibel und können Import-Einstellungen anüassen:

* Das Spaltentrennzeichen
* Numerische Daten
  * Tausendertrennzeichen
  * Dezimaltrennzeichen
* Datums- und Zeitformat

Die aufrufende App hat die Möglichkeit eigene Defaults zu übergeben. Außerdem, kann sie detailliert spezifizieren, welche Spalten erwartet werden einschließlich deren Name und Format.

<br/>
<a href="https://github.com/SigurdJanson/shinyCSVImpoMod">Zu finden auf Github</a>
