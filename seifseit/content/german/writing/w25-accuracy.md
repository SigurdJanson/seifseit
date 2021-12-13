---
title: 'Die Genauigkeit selbst programmierter R Funktionen'
date: '2020-01-14'
author: Jan Seifert
image: images/blog/accuracy.webp
bg_image: images/writing-bg.webp
categories:
  - Software Tests
tags:
  - 'R'
languages:
  - English
description: 'Eine Geschichte über undichte Stellen, Verschleiß, und Abtrift'
draft: false
type: writing
information:
  - label : "Zielgruppe"
    info : "Data scientists"

mediumlink: /accuracy-of-self-made-r-functions-8b3ff097f915?source=friends_link&sk=ba40877a80b410235c0c5011bcd9a85b
abstract: ""
---

Kürzlich habe ich ein paar eigene statistische Funktionen in R getestet. Ich hatte dafür nur wenige Testfälle zur Verfügung und kam daher auf die Idee, die inverse Funktion zum Testen einzusetzen, um meine Tests zu verbessern. In R gibt es viele solcher Funktionen, die auch invers funktionieren. Das bedeutet, dass  `f'(x)` rückgängig macht, was auch immer `f(x)` erzeugt hat. Also, in der Theorie: `f'(f(x)) == x`. In der Praxis kann es natürlich immer passieren, dass beide Funktionen Fehler haben, die sich gegenseitig aufheben. Ein Test kann daher nicht allein auf einer inversen Operation aufbauen. Aber ich dachte, dass es eine gute Ergänung zu den routinemäßigen Unit Tests wäre, weil sich eine Funktion damit sehr umfassend testen lässt, was sonst sehr aufwändig wäre ...

