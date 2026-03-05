---
title: "PPA 6/10: Bestandteile der Programmanalyse [Programm-Analyse-Crashkurs]"
date: 2023-04-10T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/ItJwyiUFjrs/maxresdefault.jpg"
  alt: "PPA 6/10: Bestandteile der Programmanalyse [Programm-Analyse-Crashkurs]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=ItJwyiUFjrs](https://www.youtube.com/watch?v=ItJwyiUFjrs)

## Zusammenfassung
In dieser Vorlesung erläutert Yegor Bugayenko die grundlegenden Konzepte und theoretischen Grenzen der Programmanalyse. Das Hauptziel der Analyse ist es, die Semantik und Syntax eines Programms zu verstehen, um dessen Eigenschaften zu bewerten. Ein zentraler Aspekt ist die Erkenntnis, dass eine perfekte Programmanalyse mathematisch unmöglich ist (Rice-Theorem, Halteproblem). Daher müssen Analysewerkzeuge anhand von zwei Kriterien bewertet werden: Korrektheit (Soundness) und Vollständigkeit (Completeness).

Eine "korrekte" (sound) Analyse überapproximiert: Wenn sie keinen Fehler findet, ist das Programm garantiert fehlerfrei, auch wenn sie Fehlalarme (False Positives) produzieren kann. Eine "vollständige" (complete) Analyse hingegen unterapproximiert: Jeder gemeldete Fehler ist echt, aber sie könnte echte Fehler übersehen (False Negatives). Bugayenko unterscheidet zudem zwischen statischer Analyse, Lintern (Stilprüfung) und dynamischer Analyse (Testen zur Laufzeit). Er schließt mit den mathematischen Grundlagen ab, insbesondere Verbänden (Lattices) und Halbordnungen, die es ermöglichen, Informationen aus verschiedenen Ausführungspfaden sicher zusammenzuführen.

## Kernaussagen
- "Eine perfekte Programmanalyse ist unmöglich; wir müssen uns zwischen Korrektheit und Vollständigkeit entscheiden."
- "Statische Analyse ist die Untersuchung von Code, ohne ihn jemals auszuführen."
- "Verbände (Lattices) sind das mathematische Werkzeug, um Zustände an Verzweigungspunkten im Programm zu verschmelzen."
- "Ein 'sound' Werkzeug garantiert Sicherheit auf Kosten von gelegentlichen Fehlalarmen."

## Relevanz: 5/5
Essentiell für das Verständnis, wie moderne Qualitätswerkzeuge funktionieren und warum sie niemals alle Fehler finden können.
