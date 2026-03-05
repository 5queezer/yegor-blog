---
title: "SQM 2/24: Zyklomatische Komplexität nach Thomas J. McCabe"
date: 2023-09-30T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/Cvv0Olx4Bpw/maxresdefault.jpg"
  alt: "SQM 2/24: Zyklomatische Komplexität nach Thomas J. McCabe"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=Cvv0Olx4Bpw](https://www.youtube.com/watch?v=Cvv0Olx4Bpw)

## Zusammenfassung
In dieser Sitzung analysiert Yegor Bugayenko das wegweisende Werk von Thomas J. McCabe aus dem Jahr 1976 über die zyklomatische Komplexität (CC). Er stellt Komplexität nicht als technisches Nebenprodukt dar, sondern als eine bewusste Entscheidung, die den Respekt eines Entwicklers gegenüber künftigen Wartungsingenieuren widerspiegelt. Mit der humorvoll bezeichneten „Augenschmerz-Metrik“ verdeutlicht er, dass Code, der schwer zu lesen ist, zwangsläufig riskant und teuer in der Wartung ist. Die technische Definition von CC basiert auf der Anzahl der linear unabhängigen Pfade durch den Kontrollflussgraph eines Programms, berechnet nach der Formel $V(G) = E - N + 2$.

Ein wesentlicher Teil des Vortrags widmet sich der Debatte über das Verhältnis zwischen CC und der Anzahl der Codezeilen (Lines of Code, LoC). Obwohl beide Metriken oft korrelieren, betont Bugayenko, dass die zyklomatische Komplexität die logische Dichte eines Moduls wesentlich präziser erfasst. Er weist darauf hin, dass eine hohe CC ein verlässlicher Indikator für eine hohe Fehlerdichte und erschwerte Testbarkeit ist. In Anlehnung an McCabe plädiert er für einen strikten Schwellenwert von 10: Funktionen, die diesen Wert überschreiten, sollten als „Code Smell“ betrachtet und refaktorisiert werden. Die wichtigste praktische Erkenntnis ist die Verbindung zum Testen: Der CC-Wert entspricht der Mindestanzahl an Testfällen für eine vollständige Zweigabdeckung. Abschließend stellt Bugayenko fest, dass wahre Ingenieurskunst darin besteht, komplexe Anforderungen durch einfachen, wartbaren Code zu lösen, unterstützt durch automatisierte Qualitätskontrollen in CI/CD-Pipelines.

## Kernaussagen
* „Komplexität ist eine Entscheidung, die der Programmierer trifft, keine unvermeidbare Folge der Anforderungen.“
* „Die zyklomatische Komplexität gibt an, wie viele Testfälle man mindestens benötigt, um alle Pfade abzudecken.“
* „Komplexer Code ist ein Zeichen mangelnden Respekts gegenüber denjenigen, die ihn später warten müssen.“
* „Die Formel $V(G) = E - N + 2$ ermöglicht es uns, Risiken in der Logik mathematisch greifbar zu machen.“

## Relevanz: 5/5
Die zyklomatische Komplexität ist ein Grundpfeiler moderner Software-Qualitätsmetriken und entscheidend für die Testplanung und Wartbarkeit.
