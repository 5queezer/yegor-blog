---
title: "SQM 18/24: Fehlerdichte"
date: 2024-02-21T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/M-yHXzROVno/maxresdefault.jpg"
  alt: "SQM 18/24: Fehlerdichte"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=M-yHXzROVno](https://www.youtube.com/watch?v=M-yHXzROVno)

## Zusammenfassung
In dieser Vorlesung aus seinem Kurs „Software Quality Management“ (SQM) analysiert Yegor Bugayenko die Metrik der Fehlerdichte (Defect Density) und stellt gängige Mythen über Codegröße und Komplexität infrage. Die Fehlerdichte wird als Anzahl der bestätigten Fehler pro Tausend Zeilen Code (KLOC) definiert. Basierend auf einer Studie von Yamashita et al., die Yegors Team repliziert hat, wird untersucht, ob kleinere Dateien tatsächlich eine höhere Qualität aufweisen.

Die zentrale Erkenntnis ist das Paradoxon der Aufteilung: Entgegen der weitläufigen Meinung, dass kleine Klassen und Dateien inhärent besser sind, zeigt die Statistik oft eine geringere Fehlerdichte bei größeren Dateien. Bugayenko argumentiert, dass beim Aufteilen einer großen, komplexen Komponente in viele kleine Fragmente die Komplexität nicht verschwindet. Sie verschiebt sich lediglich von der internen Logik der Datei hin zu den Interaktionen und Abhängigkeiten zwischen den neu entstandenen Dateien. Da diese Schnittstellen oft schwieriger zu überwachen sind, kann die Gesamtzahl der Fehler sogar steigen. Der Vortrag macht deutlich, dass starre Grenzwerte für Zeilenanzahl oder zyklomatische Komplexität unzuverlässige Qualitätsindikatoren sind. Refactoring sollte daher nicht blind nach Metriken erfolgen, sondern die Wartbarkeit des gesamten Systems im Blick behalten.

## Kernaussagen
- „Die Fehlerdichte setzt die Anzahl der Bugs ins Verhältnis zur Codemenge, was ein objektiveres Bild der Qualität vermittelt als reine Fehlerzahlen.“
- „Wenn man eine große Datei aufspaltet, verschwindet die Komplexität nicht – sie wandert nur in die Interaktionen zwischen den Komponenten.“
- „Studien belegen, dass größere Dateien oft eine niedrigere relative Fehlerdichte aufweisen als viele kleine, hochgradig vernetzte Dateien.“
- „Grenzwerte für Codegröße oder Komplexität sind oft irreführend und garantieren keine fehlerfreie Software.“

## Relevanz: 5/5
Die Vorlesung bietet eine kritische Perspektive auf „Clean Code“-Dogmen und ist essenziell für Teams, die versuchen, Qualität durch das bloße Einhalten von Metriken zu erzwingen.
