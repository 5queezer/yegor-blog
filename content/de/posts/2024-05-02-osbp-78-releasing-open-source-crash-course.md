---
title: "OSBP 7/8: Releasing [Open-Source-Crashkurs]"
date: 2024-05-02T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/VTsbvZSMwYE/maxresdefault.jpg"
  alt: "OSBP 7/8: Releasing [Open-Source-Crashkurs]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=VTsbvZSMwYE](https://www.youtube.com/watch?v=VTsbvZSMwYE)

## Zusammenfassung
In dieser Folge seiner "Open Source Best Practices"-Reihe legt Yegor Bugayenko dar, dass Software-Releases als routinemäßige, automatisierte und häufige Ereignisse betrachtet werden sollten, statt als stressige Meilensteine. Er stellt die traditionelle Denkweise infrage, mit einer Veröffentlichung zu warten, bis das Produkt "gut" oder "perfekt" ist. Stattdessen vertritt er die Ansicht, dass ein Release immer dann ausgelöst werden sollte, wenn Änderungen (ein "Delta") vorhanden sind. Dieser Ansatz senkt die Kosten pro Release und beschleunigt den Feedback-Zyklus, was langfristig die Softwarequalität erhöht.

Bugayenko betont zwei technische Säulen: vollständige Automatisierung und strikte Versionierung. Er besteht darauf, dass der Release-Prozess komplett skriptgesteuert sein muss, ohne jegliche manuelle Eingriffe. Jeder manuelle Schritt wird als Systemfehler betrachtet. Er plädiert für die konsequente Anwendung von Semantic Versioning (SemVer), um den Nutzern die Art der Änderungen klar zu kommunizieren. Zudem unterstreicht er, dass ein Release nicht bloß ein Git-Tag ist, sondern eine "Komponente" – ein fertiges Paket oder eine Bibliothek, die in zentralen Repositories (wie Maven Central oder PyPI) veröffentlicht wird. Schließlich empfiehlt er, Release-Notes automatisch zu generieren, um den administrativen Aufwand zu minimieren und Konsistenz zu gewährleisten.

## Kernaussagen
- "Veröffentliche, wenn es anders ist, nicht wenn es gut ist": Der Auslöser für ein Release ist die Veränderung, kein subjektives Qualitätsmaß.
- "Ein Release ist eine Komponente, kein bloßer Tag": Wenn Nutzer kein fertiges Artefakt herunterladen können, wurde faktisch nichts veröffentlicht.
- "Automatisiere alles oder scheitere": Manuelle Schritte im Release-Prozess sind Fehlerquellen, die zwangsläufig zu Disziplinlosigkeit und Projektabbau führen.

## Relevanz: 5/5
Das Video ist äußerst relevant für Softwareentwickler und Teamleiter, die professionelle CI/CD-Pipelines aufbauen und eine hohe Disziplin in Open-Source-Projekten etablieren möchten.
