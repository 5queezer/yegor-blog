---
title: "SQM 21/24: Builds [Software-Qualitäts-Crashkurs]"
date: 2024-04-03T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/QQUda0fAcxE/maxresdefault.jpg"
  alt: "SQM 21/24: Builds [Software-Qualitäts-Crashkurs]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=QQUda0fAcxE](https://www.youtube.com/watch?v=QQUda0fAcxE)

## Zusammenfassung
In dieser Vorlesung untersucht Yegor Bugayenko die historische Entwicklung und die technischen Metriken von Software-Builds im Rahmen des Software Quality Management (SQM). Er skizziert den Weg von den frühen 1990er Jahren, insbesondere Microsofts „Daily Build and Smoke Test“, über den Aufstieg von Extreme Programming (XP) im Jahr 1998 bis hin zur Formalisierung von Continuous Integration (CI) durch Martin Fowler und Continuous Delivery (CD) durch Jez Humble.

Ein wesentlicher Teil des Vortrags widmet sich der Analyse von Build-Metriken und der Verteilung von Build-Zeiten. Bugayenko hebt ein zentrales Problem der Branche hervor: **Flaky Tests** (unzuverlässige Tests). Er argumentiert, dass nicht-deterministische Tests – also solche, die fehlschlagen und nach einem einfachen Neustart bestehen – eine massive Bedrohung für die Softwarequalität darstellen, da sie das Vertrauen des Teams in den CI-Prozess zerstören. Wenn Entwickler Build-Fehler nicht mehr ernst nehmen, verliert die CI ihre Funktion als Qualitätsinstanz. Die Vorlesung behandelt zudem CI im großen Maßstab und betont die Wichtigkeit von Kennzahlen wie der „Time to Fix“ (Zeit bis zur Fehlerbehebung) und der „Flakiness-Quote“, um eine professionelle Entwicklungsumgebung aufrechtzuerhalten.

## Kernaussagen
- „Ein Build ist nicht nur ein technischer Schritt; es ist eine formale Bestätigung, dass der Code die Qualitätsstandards des Projekts erfüllt.“
- „Der größte Feind eines gesunden CI-Prozesses ist der ‚Re-run‘-Button. Unzuverlässige Tests zerstören das Vertrauen der Entwickler in die Automatisierung.“
- „Continuous Integration ist kein Werkzeug wie Jenkins; es ist die Praxis, Arbeit mehrmals täglich zu integrieren.“
- „Build-Fehler sollten schnell auftreten. Die teuerste Zeitverschwendung ist ein Build, der erst nach einer Stunde Laufzeit fehlschlägt.“

## Relevanz: 5/5
Äußerst relevant für Software-Architekten und Teamleiter. Die Vorlesung vermittelt das tiefere Verständnis von Builds als disziplinarisches Werkzeug zur Sicherung der Codequalität.
