---
title: "SQM 17/24: Function-Points [Software-Qualitäts-Crashkurs]"
date: 2024-02-13T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/xt01nxxfAB0/maxresdefault.jpg"
  alt: "SQM 17/24: Function-Points [Software-Qualitäts-Crashkurs]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=xt01nxxfAB0](https://www.youtube.com/watch?v=xt01nxxfAB0)

## Zusammenfassung
In dieser Vorlesung erläutert Yegor Bugayenko die Function-Point-Analyse (FPA) als präzises Werkzeug zur Messung der Softwaregröße, das die veraltete Metrik "Lines of Code" (LOC) ersetzt. Bugayenko argumentiert, dass LOC zu einem "Produktivitätsparadoxon" führt: Ein Programmierer, der umständlichen Code in einer Low-Level-Sprache schreibt, wirkt produktiver als jemand, der dasselbe Problem effizient in einer modernen Sprache löst. Die von Allan Albrecht (IBM) Ende der 1970er Jahre entwickelten Function-Points lösen dieses Problem, indem sie den Fokus auf den geschäftlichen Nutzen für den Anwender legen.

Der Kern der Methode besteht aus fünf Komponenten: Interne logische Dateien (ILF) und externe Schnittstellendateien (EIF) für die Datenstruktur sowie externe Eingaben (EI), externe Ausgaben (EO) und externe Abfragen (EQ) für die Transaktionen. Diese werden gewichtet und können durch 14 allgemeine Systemcharakteristika (GSCs) angepasst werden, um technische Komplexität wie Performance oder Wiederverwendbarkeit zu berücksichtigen. Das Ergebnis ist eine technologieunabhängige Zahl, die den funktionalen Umfang beschreibt.

Yegor betont, dass diese Methode für das Projektmanagement unerlässlich ist, da sie objektive Benchmarks ermöglicht. Er weist auf internationale Standards wie IFPUG hin und erklärt, wie Function-Points in Schätzmodelle wie COCOMO-II einfließen. Obwohl die Zählung aufwendiger ist als das bloße Zählen von Zeilen, bietet sie die einzige verlässliche Basis für die Berechnung von Kosten, Aufwand und Qualität in professionellen Softwareprojekten, da sie die Software aus der Sicht des Kunden und nicht des Handwerkers misst.

## Kernaussagen
* "Function-Points verschieben den Fokus von der Implementierung auf den Nutzwert der Software."
* "Lines of Code hängen von der Sprache ab; Function-Points sind technologieunabhängig und ermöglichen faire Vergleiche."
* "Das Produktivitätsparadoxon zeigt, dass mehr Code oft weniger Effizienz bedeutet; echte Größe misst sich an der Funktionalität."
* "Die fünf Basiskomponenten erlauben eine standardisierte Beschreibung der Systemgrenzen und Datenflüsse."

## Relevanz: 5/5
Absolut kritisch für Software-Architekten und Projektleiter. FPA ist das Fundament für wissenschaftliches Projektmanagement und objektive Leistungsbewertung.
