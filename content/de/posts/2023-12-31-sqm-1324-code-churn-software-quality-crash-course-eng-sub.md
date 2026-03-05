---
title: "SQM 13/24: Code Churn [Software-Qualitäts-Crashkurs]"
date: 2023-12-31T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/dvuyJ5LvHvQ/maxresdefault.jpg"
  alt: "SQM 13/24: Code Churn [Software-Qualitäts-Crashkurs]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=dvuyJ5LvHvQ](https://www.youtube.com/watch?v=dvuyJ5LvHvQ)

## Zusammenfassung
In diesem Vortrag erläutert Yegor Bugayenko das Konzept des „Code Churn“ als entscheidende Metrik für das Software-Qualitätsmanagement. Im Gegensatz zu statischen Metriken wie „Lines of Code“ (LoC), die nur die aktuelle Größe eines Projekts messen, erfasst Code Churn die evolutionäre Dynamik – also wie viel Code über einen bestimmten Zeitraum hinzugefügt, gelöscht oder geändert wurde. Bugayenko argumentiert, dass die Änderungshistorie wesentlich aussagekräftiger ist als der aktuelle Zustand des Codes.

Ein zentrales Element ist die Forschung von Nagappan und Ball (2005), die zeigt, dass der „Relative Code Churn“ ein weitaus besserer Indikator für die Fehlerdichte ist als herkömmliche Maße. Dateien, die häufig und massiv verändert werden, werden als „Hotspots“ identifiziert. Diese Bereiche weisen eine statistisch höhere Wahrscheinlichkeit für Bugs auf, was oft auf instabile Anforderungen, architektonische Mängel oder mangelndes Verständnis der Entwickler für das jeweilige Modul hindeutet.

Zudem stellt Bugayenko seine eigene Metrik vor: Hits-of-Code (HoC). Er kritisiert LoC dafür, dass Refactoring oft als „negativer Fortschritt“ erscheint, wenn Code gelöscht wird. HoC hingegen summiert alle Änderungen in Git kumulativ auf und steigt immer an, was den tatsächlichen Aufwand und den geschäftlichen Nutzen der Entwicklerarbeit realistischer widerspiegelt. Die Vorlesung plädiert dafür, Churn-Daten proaktiv zu nutzen, um Risiken frühzeitig zu erkennen und technische Schulden gezielt abzubauen.

## Kernaussagen
- „Qualität hängt nicht nur davon ab, wie der Code jetzt aussieht, sondern wie stark er sich verändert.“
- „Hits-of-Code (HoC) zeigt dem Unternehmen, dass man tatsächlich gearbeitet hat, selbst wenn man mehr Code gelöscht als hinzugefügt hat.“
- „Dateien mit hohem relativen Churn sind ‚Hotspots‘ – wir müssen nicht auf Bugs warten, um zu wissen, dass sie dort entstehen werden.“
- „Das Ziel eines Managers sollte es sein, die Churn-Rate instabiler Module zu senken, statt nur die Anzahl der Features zu erhöhen.“

## Relevanz: 5/5
Äußerst relevant für Software-Architekten und Teamleiter, da es zeigt, wie man Git-Historien nutzt, um Wartungsrisiken objektiv zu bewerten.
