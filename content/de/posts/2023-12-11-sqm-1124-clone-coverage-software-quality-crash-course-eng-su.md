---
title: "SQM 11/24: Klon-Abdeckung [Software-Qualitätskurs]"
date: 2023-12-11T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/ynPTEzDTutc/maxresdefault.jpg"
  alt: "SQM 11/24: Klon-Abdeckung [Software-Qualitätskurs]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=ynPTEzDTutc](https://www.youtube.com/watch?v=ynPTEzDTutc)

## Zusammenfassung
In dieser Vorlesung aus seiner Reihe „Software Quality Management“ untersucht Yegor Bugayenko das Konzept der „Clone Coverage“ (Klon-Abdeckung) – eine Metrik, die den Prozentsatz der Codebasis misst, der aus duplizierten Fragmenten besteht. Bugayenko argumentiert, dass Codeduplizierung einer der schädlichsten „Code-Smells“ ist, da sie die Wartbarkeit eines Systems direkt untergräbt. Das Hauptproblem bei Klonen ist der Effekt der Fehlerfortpflanzung: Wenn in einem Schnipsel ein Fehler gefunden wird, muss ein Entwickler jede identische oder ähnliche Kopie im gesamten Projekt manuell finden und korrigieren. Geschieht dies nicht, bleiben latente Fehler zurück, die später erneut auftreten.

Die Vorlesung beschreibt vier verschiedene Arten von Code-Klonen. Typ-1 (Exakt) und Typ-2 (Parametrisiert) sind am einfachsten durch einfache Text- oder Token-basierte Analysen zu erkennen. Typ-3 (Lückenhaft) beinhaltet leichte Variationen, während Typ-4 (Semantisch) Codeabschnitte darstellt, die dieselbe Logik ausführen, aber mit völlig unterschiedlichen Algorithmen oder Syntax geschrieben sind, was sie für automatisierte Werkzeuge fast unsichtbar macht. Bugayenko betont die „Regel der Drei“: Code einmal zu duplizieren ist für die Geschwindigkeit akzeptabel, aber beim dritten Mal ist ein sofortiges Refactoring erforderlich. Er erörtert auch verschiedene Erkennungsmethoden, die von einfachen Textvergleichen bis hin zu komplexen Analysen des abstrakten Syntaxbaums (AST) reichen. Letztendlich definiert er eine hohe Klon-Abdeckung als eine erhebliche Form von technischen Schulden, die Qualitätsmanager durch konsequente Abstraktion und Dekomposition minimieren müssen.

## Kernaussagen
- „Codeduplizierung ist nicht nur ein Stilproblem; es ist eine Wartungsfalle, die die Kosten jeder Fehlerbehebung und jedes Feature-Updates vervielfacht.“
- „Typ-4-Klone sind am gefährlichsten, da sie die Logik, aber nicht die Form teilen, was sie für Standard-Linting-Tools unsichtbar macht.“
- „Die ‚Regel der Drei‘ dient als pragmatische Schwelle für das Refactoring: Zwei Kopien sind ein Zufall, drei Kopien sind ein strukturelles Versagen.“
- „In großen Legacy-Systemen erreicht die Klon-Abdeckung oft 20-30 %, was wie ein massiver Anker für die Entwicklungsgeschwindigkeit wirkt.“

## Relevanz: 5/5
Die Vorlesung ist äußerst relevant, da sie die architektonischen Grundlagen von sauberem Code anspricht und umsetzbare Metriken für das Management technischer Schulden in professionellen Softwareteams liefert.
