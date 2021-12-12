---
title: "Die Kreuzkorrelationsfunction in R"
date: 2020-03-18
author: Jan Seifert
image : "images/blog/crosscorrelation.webp"
bg_image: "images/writing-bg.webp"
categories: ["Statistik"]
tags: ["R"]
languages: ["English"]
description: "Was nicht im Handbuch steht..."
draft: false
type: "writing"
information:
  - label : "Zielgruppe"
    info : "Data Scientists"

mediumlink: /the-r-cross-correlation-function-f5f426006425?source=friends_link&sk=60e3a85df26d2eebd0c47ab84c3407c0
abstract: ""
---

R is großartig! Du nimmst einfach zwei Vektoren, rein in die Funktion und fertig ... R ist die Pest. In einem kleinen Projekt brauchte die ccf-Funktion. Aber ich hatte große Schwierigkeiten die Ergebnisse zu verstehen. Es gibt da ein paar wichtige Dinge über die Kreuzkorrelationsfunktion von R, die schlicht nicht im Handbuch dokumentiert sind. Das Handbuch zu lesen hat mir kaum geholfen. Ich musste mit der Funktion experimentieren und das alles aufschreiben. Was in diesem Manuskript steht war etwa ein ganzer Tag Arbeit. Aber nur, weil ich es auf die harte Tour lernen musste, heißt nicht, dass Du das auch tun musst.

Die Funktion `ccf(x, y)` erwartet zwei Vektoren, um die Korrelation zwischen `x[t+k]` und `y[t]` zu bestimmen. Das bedeutet, sie wird natürlich nicht einfach die Vektoren korrelieren. Sie wird die Korrelation rechnen, nachdem sie die Vektoren in ihrer relativen Position zueinander um `k` Elemente verschoben hat. Außerdem wird typischerweise nicht nur mit einem Wert `k` gerechnet ...

