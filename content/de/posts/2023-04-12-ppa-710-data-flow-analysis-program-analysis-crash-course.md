---
title: "PPA 7/10: Datenflussanalyse [Crashkurs Programmanalyse]"
date: 2023-04-12T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/loAVqyfP374/maxresdefault.jpg"
  alt: "PPA 7/10: Datenflussanalyse [Crashkurs Programmanalyse]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=loAVqyfP374](https://www.youtube.com/watch?v=loAVqyfP374)

## Zusammenfassung
In diesem siebten Teil seines Crashkurses zur Programmanalyse erläutert Yegor Bugayenko die Datenflussanalyse (Data Flow Analysis, DFA). Dabei handelt es sich um eine statische Technik, um Informationen über die möglichen Werte an verschiedenen Stellen eines Programms zu sammeln, ohne den Code tatsächlich auszuführen. Die Grundlage hierfür bildet der Kontrollflussgraph (CFG), auf dem sogenannte "Datenfluss-Fakten" propagiert werden.

Bugayenko führt das mathematische Grundgerüst der DFA ein, bestehend aus GEN- und KILL-Mengen. Die GEN-Menge enthält Fakten, die in einem Basisblock neu entstehen (z. B. eine Variablenzuweisung), während die KILL-Menge Fakten enthält, die durch den Block ungültig werden. Eine Transferfunktion berechnet basierend auf diesen Mengen den Ausgangszustand eines Blocks aus seinem Eingangszustand. An Verzweigungspunkten kommt ein "Meet-Operator" zum Einsatz, um die Informationen aus verschiedenen Pfaden zu kombinieren.

Ein zentraler Aspekt der Vorlesung ist der iterative Prozess zur Erreichung eines Fixpunktes. Da Programme Schleifen enthalten können, muss der Analysealgorithmus (oft der Worklist-Algorithmus) den Graphen mehrfach durchlaufen, bis sich die Datenfluss-Fakten nicht mehr ändern. Der Vortrag geht zudem auf verschiedene Sensitivitätsstufen ein: flusssensitiv, pfadsensitiv und kontextsensitiv. Abschließend zeigt Bugayenko den praktischen Nutzen auf, etwa bei der Erkennung nicht initialisierter Variablen oder bei Compiler-Optimierungen wie der Entfernung von totem Code (Dead Code Elimination).

## Kernaussagen
- „Datenflussanalyse ist die Kunst der Annäherung; wir versuchen nicht, das Programm zu verstehen, sondern seine Grenzen zu berechnen.“
- „Der Fixpunkt ist das Ziel jeder statischen Analyse – der Moment, in dem unsere Informationen über den Code stabil werden.“
- „GEN erzeugt Wissen, KILL vernichtet es; die Transferfunktion ist der Buchhalter, der den aktuellen Stand verwaltet.“
- „Ein guter statischer Analysator ist lieber konservativ und meldet einen Fehler zu viel, als einen echten Bug zu übersehen.“

## Relevanz: 5/5
Die DFA ist die theoretische Basis für moderne IDE-Inspektionen und Sicherheits-Audit-Tools, was sie für Software-Architekten und Tool-Entwickler unverzichtbar macht.
