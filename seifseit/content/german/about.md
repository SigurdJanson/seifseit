---
title: "Über mich"
description: ""
bg_image: "images/globe-detailed_labelled.svg"
layout: "about"
draft: false
menu:
  main:
    name: "Über mich"
    weight: 2


################################## About #####################################
about:
  enable : true
  image : "images/Jan2013c.jpg"
  title : "Meine Geschichte"
  content : "<p>Ich war schon immer fasziniert von den Möglichkeiten der Technik und dennoch wollte ich mehr darüber wissen, was Menschen antreibt. Drei Themen haben mich am meisten gepackt: die biologische Basis des Geistes, die Methoden, um Erkenntnisse über Menschen zu gewinnen, und wie unsere Umwelt mit uns interagiert und umgekehrt.</p>
  <p>Auf der Universität bin ich früh mit der Hirnforschung in Berührung gekommen, mit elektrophysiologischer und bildgebender Forschung. Die Erkundung des menschlichen Geistes mit komplizierter technischer Ausrüstung ... ich bin blieb nach dem Diplom an der Uni für den Spaß an der Neugier.</p>
  <p>Davon habe ich mich mit dem Doktor der Naturwissenschaften in 2005 verabschiedet und bin in die User Experience gegangen. Andere Aufgabe, gleiches Leitmotiv: das Interesse an Menschen in Verbindung mit Technologien und das Bemühen, die Beziehung der beiden zueinander zu verbessern und Allen einen fairen Zugang zu neuen Technologien zu verschaffen. In den letzten {{< yearsinux >}} Jahren habe ich dutzende Kunden unterstützt. In einer wachsenden Gemeinschaft von Kollegen und Freunden machen wir Research, konzeptuelle Gestaltung und Prototyping.</p>
  <p>Die Interaktion von Menschen mit ihrer Umwelt natürlich auch eine wesentliches Thema in der User Experience. In den letzten Jahren bekam das noch ein ganz neues Gewicht. Es geht für mich heute nicht nur um Menschen und Technik. Die Menschen in ihrer Zusammenarbeit und den Organisationen rücken mehr ins Zentrum. Wie entwickeln sich Organisationen, wie schränken sie uns ein oder setzen Potential frei? Ich weiß nicht so recht, ob wir das jemals voll und ganz verstehen. Aber wir machen Fortschritte.</p>


### Interessensschwerpunkte

* **Organisationsdesign und -entwicklung** wobei ich dabei meine Wurzeln aus der Psychologie wiederentdecke und mich sehr mit Behavioural Design auseinandersetze. Veränderung beginnt mit den Menschen.

* Emotionale and soziale Aspekte der Mensch-Maschine-Interaktion

* **User & Customer Research** - quantitative and qualitative Analysen und die dafür erforderlichen [Operations (Research Ops)](https://researchops.community/).

* Die Auseinandersetzung mit **Design Leadership** wurde im Laufe der Jahre zunehmend wichtiger.
"

insight:
  enable: true
  title: "Eine kleine Erkenntnis auf meinem Weg ..."
  message: "Die wertvollste Ressource in Eurer Organisation? Es ist nicht Zeit. Auch nicht Geld. ... Es ist Aufmerksamkeit."


button:
  enable : false
  label : "Download Company Profile"
  link : "#"



funfacts:
# funfacts loop
- icon : "icon-flask-outline" #ionicon pack v2 : https://ionicons.com/v2/
  name : "Abgeschlossene Projekte"
  count : '{{< param "nprojects" >}}' #

# funfacts loop
- icon : "icon-trophy-outline" #ionicon pack v2 : https://ionicons.com/v2/
  name : "Zufriedene Kunden"
  count : '{{< param "nCustomers" >}}' #

# funfacts loop
- icon : "icon-wine-outline" #ionicon pack v2 : https://ionicons.com/v2/
  name : "Jahre Erfahrung"
  count : '{{< yearsinux >}}'

# funfacts loop
- icon : "icon-chatbubbles-outline" #ionicon pack v2 : https://ionicons.com/v2/
  name : "User Research Kontakte"
  count : '{{< param "nResearchContacts" >}}' # 



################################ feature #####################################
features:
  enable : true
  title : "Aktivitäten aus reiner Neugier"
  feature_item:
  # feature item loop
  - icon : "icon-code-working-outline" #ionicon pack v2 : https://ionicons.com/v2/
    name : "App Entwicklung"
    content : "Um die Arbeit mit Technologien besser zu verstehen halte ich mich auf Trab mit [R](https://www.r-project.org) und [.NET Blazor](https://dotnet.microsoft.com/apps/aspnet/web-apps/blazor)."

  # feature item loop
  - icon : "icon-bag-outline" #ionicon pack v2 : https://ionicons.com/v2/
    name : "eCommerce"
    content : "Verantwortlich für digitale Angelegenheiten und Design im kleinen Familienunternehmen [Ankes Keksgenuss](https://keksgenuss.de)."

  # feature item loop
  - icon : "icon-people-outline" #ionicon pack v2 : https://ionicons.com/v2/
    name : "User Experience"
    content : "Viele Jahre im [User Experience Design](https://www.uid.com) als Gestalter und Researcher, als Projekt- und Teamleiter und als Consultant für einen deutlicheren Produkterfolg."

  # feature item loop
  - icon : "icon-chatbubbles-outline" #ionicon pack v2 : https://ionicons.com/v2/
    name : "Vernetzt"
    content : "Immer auf der Suche nach Austausch in den Communities, dem [German UPA chapter](https://www.germanupa.de/), auf Konferenzen und Vorträgen."

  # feature item loop
  - icon : "icon-nutrition-outline" #ionicon pack v2 : https://ionicons.com/v2/
    name : "Kochen"
    content : "Kennt Ihr leckere Fälle von einfacher Crossover Küche, lasst es mich wissen."

  # feature item loop
  - icon : "icon-color-wand-outline" #ionicon pack v2 : https://ionicons.com/v2/
    name : "Geschichten"
    content : "Geschichten lesen, imaginieren, oder einfach darin eintauchen."


#################################### testimonial & mission vision #######################################
testimonial:
  enable : false
  # testimonial content comes from "data/*/homepage.yml" file

mission_vision:
  enable : true
  title: "Einsichten"
  tabs:
  # tab item loop
  - name : "Verstehen"
    content : "Tolle Produkte gestalten, die die Leute lieben ... ist keine einfache Sache und klappt meist nur, wenn wir auch vertraute Pfade verlassen. Während Freunde von mir die design-getriebene Organisation propagieren, oder auch agile und innovationsgetriebene, stelle ich lieber Fragen: 'Welches Problem wollen wir gerade lösen?'. Denn **ein Ziel ist nur ein Werkzeug**. Keine Lösung. Darum sollen wir nicht aufhören uns zu fragen, wo wir stehen und welcher Weg uns in eine lichtere Zukunft führen kann."

  # tab item loop
  - name : "Anpassen"
    content : "Der Gewinn aus nutzerzentriertem Arbeiten ist nicht immer der Gleiche. Der Ansatz ermöglicht es ganz verschiedene Ziele zu verfolgen. Mir gehts immer darum herauszufinden was funktioniert. Was ist das beste Ziel für uns? Was müssen wir für unsere UX tun, um sie möglichst effizient zu entwickeln? Wie können wir andere inspirieren und sie für nutzerzentriertes Arbeiten begeistern? Derartige Fragen bewegen mich in meinen Projekten. Hört nicht auf Fragen zu stellen."


  # tab item loop
  - name : "Vereinfachen"
    content : "Wachsendes agiles Arbeiten hat unsere Arbeitswelt bereits stark beeinflusst und viele Chancen eröffnet. Aber wir haben noch keine neue Balance gefunden. Der fortwährende Zyklus vin Inspektion, Anpassung und Lernen trägt das Risiko sich zu viel aufzuhalsen. Es ist absolut wichtig, dass wir neue Routinen entwickeln, die Veränderung als Teil der Routine realisieren. VIele Ideen klingen auf der strategischen Ebene plausibel und können in der Umsetzung doch viel zu kompliziert sein. Strebt nach Einfachheit und seid Euch bewusst, dass **Einfachheit im Detail liegt**."

  # tab item loop
  - name : "Aktivieren"
    content : "**Strategie muss von der Umsetzung her gedacht werden**. Alles von oben bis ganz nach unten durchzuplanen wäre schädliches Micromanagement. Stellt Informationen zur Verfügung, gebt Impulse, bringt Risiken zum Vorschein, helft, aber vor allem: findet Mittel, die es in der Umsetzung erlaubt möglichst schnell die Auswirkungen von Entscheidungen zu verstehen. Arbeitet an einem System, dass es Kollegen ermöglicht zu wachsen und selbst Ziele zu entwickeln, die in die Strategie der Organisation passen."


############################# call to action #################################
cta:
  enable : false
  # call to action content comes from "_index.md"
---

