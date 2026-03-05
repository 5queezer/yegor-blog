---
title: "Object Thinking Meetup #7: Nikolay Kudasov / Algebraische Datentypen"
date: 2022-09-21T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
  - "oop"
  - "ai"
cover:
  image: "https://img.youtube.com/vi/ERIDMfy4rCg/maxresdefault.jpg"
  alt: "Object Thinking Meetup #7: Nikolay Kudasov / Algebraische Datentypen"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=ERIDMfy4rCg](https://www.youtube.com/watch?v=ERIDMfy4rCg)

## Zusammenfassung
In diesem Meetup erörtert Nikolay Kudasov die mathematischen Grundlagen und die praktische Relevanz von algebraischen Datentypen (ADTs). Er erklärt, dass der Begriff „algebraisch“ daher rührt, dass Typen durch Operationen wie Addition (Summentypen) und Multiplikation (Produkttypen) gebildet werden. Während Produkttypen – wie Klassen oder Structs – in der objektorientierten Programmierung (OOP) allgegenwärtig sind, wurden Summentypen (wie enums in Rust oder sealed classes in Kotlin) in Sprachen wie Java lange vernachlässigt.

Der zentrale Vorteil von ADTs liegt laut Kudasov darin, „illegale Zustände undarstellbar zu machen“. Durch den Einsatz von Summentypen können Entwickler Geschäftsregeln so in das Typsystem integrieren, dass ungültige Datenkonstellationen (z. B. ein Objekt, das gleichzeitig ein Ergebnis und eine Fehlermeldung enthält) technisch unmöglich werden. Kudasov kontrastiert dies mit dem klassischen OOP-Ansatz der Vererbung und zeigt auf, dass ADTs eine klare, erschöpfende Fallunterscheidung ermöglichen. Zudem wird das „Expression Problem“ thematisiert: Während die OOP die Erweiterung um neue Datentypen erleichtert, bieten ADTs Vorteile, wenn häufig neue Funktionen auf einer festen Menge von Datentypen hinzugefügt werden müssen. Der Vortrag plädiert für eine präzisere Modellierung der Domäne, um die Fehleranfälligkeit zu senken und die Wartbarkeit zu erhöhen.

## Kernaussagen
- „Ein gutes Typsystem sollte so entworfen sein, dass illegale Zustände gar nicht erst repräsentiert werden können.“
- „Produkttypen sind ein 'UND', Summentypen ein 'ODER'. Viele Fehler entstehen, weil wir 'UND' verwenden, wo logisch ein 'ODER' hingehört.“
- „Algebraische Datentypen ermöglichen es uns, die Domänenlogik direkt in die Struktur der Daten zu gießen, sodass der Compiler unsere Geschäftsregeln prüft.“
- „Das 'Expression Problem' zeigt uns, dass es kein perfektes System gibt – ADTs und OOP haben jeweils unterschiedliche Stärken bei der Erweiterbarkeit.“

## Relevanz: 5/5
Sehr hoch für Software-Architekten. Das Verständnis von ADTs ist entscheidend für modernes API-Design und robuste Systemarchitekturen.
