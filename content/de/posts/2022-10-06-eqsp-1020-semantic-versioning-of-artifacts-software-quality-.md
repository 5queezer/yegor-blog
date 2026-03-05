---
title: "EQSP 10/20: Semantische Versionierung von Artefakten [Softwarequalitäts-Crashkurs]"
date: 2022-10-06T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/xGjjRVmeCWA/maxresdefault.jpg"
  alt: "EQSP 10/20: Semantische Versionierung von Artefakten [Softwarequalitäts-Crashkurs]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=xGjjRVmeCWA](https://www.youtube.com/watch?v=xGjjRVmeCWA)

## Zusammenfassung
Yegor Bugayenko legt dar, dass die Versionierung von Software ein strikter Vertrag zwischen Anbieter und Nutzer ist. Im Zentrum steht das Semantic Versioning (MAJOR.MINOR.PATCH). Da Entwickler Release-Notes selten lesen und stattdessen nach dem Prinzip „Upgrade und Test“ verfahren, ist die **Unveränderlichkeit von Artefakten** (Immutability) entscheidend. Sobald ein Artefakt in einem zentralen Repository wie Maven Central veröffentlicht wurde, darf es niemals mehr verändert oder gelöscht werden.

Ein wesentlicher Aspekt ist die Unterscheidung zwischen flüchtigem Quellcode (GitHub) und stabilen Artefakt-Speichern. GitHub ist für Produktionsabhängigkeiten zu unzuverlässig, da Repositories jederzeit gelöscht werden können. Zudem kritisiert Bugayenko manuelle Changelogs als veraltete Praxis aus den 80er Jahren. Die Duplizierung von Versionsnummern in verschiedenen Dateien wird als Hauptquelle für Synchronisationsfehler identifiziert. Stattdessen plädiert er für automatisierte Prozesse, „Executable Documentation“ (wie Rusts Doctests) und automatisierte Versions-Badges.

## Kernaussagen
* „Informationsduplizierung ist die Quelle der meisten Probleme in der Programmierung.“
* „GitHub ist eine sehr flüchtige Informationsquelle... Auf Maven Central können wir uns zu 100 % verlassen.“
* „Releases müssen unveränderlich sein... die einmal veröffentlichte Version muss für immer dort bleiben.“
* Manuelle Release-Notes sind obsolet; die Wahrheit sollte automatisiert aus dem Build-Prozess hervorgehen.

## Relevanz: 5/5
Grundlegend für das Verständnis von CI/CD-Pipelines und professionellem Abhängigkeitsmanagement.
