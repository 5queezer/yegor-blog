---
title: "Der Schmerz von OOP Lektion #2: Statische Methoden und Attribute"
date: 2023-06-19T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
  - "oop"
  - "ai"
cover:
  image: "https://img.youtube.com/vi/lELJSj9mWbI/maxresdefault.jpg"
  alt: "Der Schmerz von OOP Lektion #2: Statische Methoden und Attribute"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=lELJSj9mWbI](https://www.youtube.com/watch?v=lELJSj9mWbI)

## Zusammenfassung
In dieser Vorlesung übt Yegor Bugayenko eine scharfe Kritik an statischen Methoden und Attributen und bezeichnet sie als "Krebsgeschwür", das die objektorientierte Programmierung (OOP) im Kern zerstört. Sein Hauptargument ist, dass statische Member ausdrucksstarke, objektorientierte Designs in starre, prozedurale Skripte verwandeln. Indem Logik an eine Klasse statt an eine Instanz gebunden wird, entstehen "hartcodierte" Abhängigkeiten, die während des Unit-Tests ohne spezielle Werkzeuge nicht abgefangen, ersetzt oder durch Mocks simuliert werden können.

Yegor unterscheidet zudem zwischen "eager" (imperativer) und "lazy" (deklarativer) Programmierung. Er argumentiert, dass statische Methoden (wie `Math.sqrt(x)`) imperative Befehle sind, die sofort ausgeführt werden, während echte Objekte deklarative Repräsentanten von Werten sein sollten, die Berechnungen erst dann durchführen, wenn sie wirklich benötigt werden. Diese "Faulheit" ermöglicht eine bessere Komposition und Flexibilität. Schließlich attackiert er das Konzept der "Utility-Klassen" (z. B. `StringUtils`) und beschreibt sie als "Mülleimer" für Logik, die kein richtiges Zuhause hat. Diesen Klassen fehlt die Identität, sie verletzen das Single-Responsibility-Prinzip und führen zu einer hohen Kopplung bei geringer Kohäsion. Um "reines" OOP zu erreichen, plädiert Yegor dafür, jede statische Methode durch eine eigene Klasse und jedes statische Attribut durch gekapselten Objektzustand zu ersetzen.

## Kernaussagen
- "Statische Methoden sind ein Krebsgeschwür; sie machen aus Ihrem objektorientierten Code prozeduralen Müll."
- "Ein Objekt sollte ein 'fauler' Repräsentant eines Ergebnisses sein, kein 'eifriger' Ausführer eines Befehls."
- "Utility-Klassen sind lediglich Namensräume für Funktionen; sie sind keine Objekte und haben in einer sauberen Architektur nichts zu suchen."
- "Wenn man es nicht mocken kann, ist man am OOP gescheitert. Statische Methoden sind der Hauptgrund für un-testbaren Code."

## Relevanz: 5/5
Diese Vorlesung ist äußerst relevant für Softwarearchitekten und Entwickler, die die "Elegant Objects"-Philosophie verstehen wollen. Sie hinterfragt Branchenstandards (wie das Singleton-Muster und Utility-Klassen) und bietet einen strengen, wenn auch kontroversen Rahmen zur Verbesserung der Testbarkeit und Wartbarkeit von Code.
