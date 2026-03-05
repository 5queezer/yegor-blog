---
title: "SQM 3/24: Kognitive Komplexität von G. Ann Campbell [Crashkurs Softwarequalität]"
date: 2023-10-03T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/oRUux3w4rsc/maxresdefault.jpg"
  alt: "SQM 3/24: Kognitive Komplexität von G. Ann Campbell [Crashkurs Softwarequalität]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=oRUux3w4rsc](https://www.youtube.com/watch?v=oRUux3w4rsc)

## Zusammenfassung
In diesem Vortrag aus seiner Reihe über Software-Qualitätsmetriken beleuchtet Yegor Bugayenko die Schwächen der klassischen zyklomatischen Komplexität (CC) und stellt die kognitive Komplexität (CoCo) als modernere, menschenzentrierte Alternative vor. Die zentrale These ist, dass CC zwar ein hervorragendes mathematisches Modell zur Bestimmung der Testbarkeit ist, jedoch versagt, wenn es darum geht, wie schwierig es für einen Programmierer ist, die Logik des Codes zu erfassen.

Bugayenko erläutert die drei von G. Ann Campbell entwickelten Grundregeln der kognitiven Komplexität. Erstens: „Syntactic Sugar“ wird ignoriert. Moderne Sprachmerkmale, die den Code kompakter machen, erhöhen die Komplexität nicht, da sie das Verständnis oft erleichtern. Zweitens: Jede Unterbrechung des linearen Kontrollflusses (wie `if`, `while` oder `catch`) führt zu einem Punktabzug. Drittens – und das ist der entscheidende Unterschied – gibt es einen „Verschachtelungs-Aufschlag“. Während CC verschachtelte Strukturen linear zählt, gewichtet CoCo sie basierend auf ihrer Tiefe. Ein `if` innerhalb mehrerer Schleifen belastet das Arbeitsgedächtnis deutlich stärker als eine sequentielle Abfrage.

Der Vortrag geht zudem auf die wissenschaftliche Validierung ein. Bugayenko beschreibt Experimente mit EEG-Headsets, die zeigen, dass tiefe Verschachtelungen die Gehirnaktivität messbar steigern. Abschließend wird die „soziale Code-Analyse“ thematisiert: Metriken sollten idealerweise mit der Fehlerhäufigkeit und dem Wartungsaufwand korrelieren, um als Steuerungsinstrument für Teams nützlich zu sein. Ziel ist es, Code zu schreiben, der flach, linear und somit leichter wartbar ist.

## Kernaussagen
- „Die zyklomatische Komplexität misst den Testaufwand, die kognitive Komplexität den Verständnisaufwand.“
- „Verschachtelung ist der Hauptfeind der Lesbarkeit; jede Ebene verlangt vom Entwickler, mehr Kontext gleichzeitig im Kopf zu behalten.“
- „Metriken müssen biologisch validiert werden – durch EEG-Messungen lässt sich nachweisen, dass komplexe Logik das Gehirn tatsächlich stärker belastet.“
- „Eine gute Metrik ist ein Vorhersageinstrument für das Teammanagement, um potenzielle Fehlerquellen frühzeitig zu identifizieren.“

## Relevanz: 5/5
Äußerst relevant für Software-Architekten, da sie eine objektive Grundlage bietet, um die Wartbarkeit von Code in großen Teams zu bewerten und zu verbessern.
