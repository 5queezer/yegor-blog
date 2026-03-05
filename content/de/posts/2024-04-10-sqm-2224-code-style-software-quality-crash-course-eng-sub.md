---
title: "SQM 22/24: Codestil [Crashkurs für Softwarequalität]"
date: 2024-04-10T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/hPZGoEAXwY0/maxresdefault.jpg"
  alt: "SQM 22/24: Codestil [Crashkurs für Softwarequalität]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=hPZGoEAXwY0](https://www.youtube.com/watch?v=hPZGoEAXwY0)

## Zusammenfassung
In dieser Vorlesung aus der Reihe „Software Quality Management“ legt Yegor Bugayenko dar, dass Codestil kein subjektives ästhetisches Merkmal, sondern eine grundlegende Metrik für die Wartbarkeit von Software ist. Er verfolgt die Entwicklung des Codestils von den frühen Grundlagenwerken wie Brian Kernighans *The Elements of Programming Style* (1974) bis hin zu modernen empirischen Studien. Die Kernkapitalhese lautet: „Schöner“ Code ist objektiv überlegen, da er die kognitive Belastung für die Wartenden minimiert.

Bugayenko plädiert für die vollständige Eliminierung individueller „Kreativität“ bei der Formatierung. Er betont, dass eine professionelle Codebasis so aussehen sollte, als sei sie von einer einzigen Person geschrieben worden. Um dies zu erreichen, fordert er den Einsatz strenger, automatisierter „Quality Gates“ mittels Werkzeugen wie Checkstyle oder RuboCop. Seine Haltung ist kompromisslos: Die Durchsetzung des Stils muss binär sein – wenn der Code auch nur gegen eine einzige Regel verstößt, muss der Build fehlschlagen. Diese Disziplin verwandelt Stil von einer Frage des „guten Geschmacks“ in einen strengen technischen Standard.

## Kernaussagen
- „Beim Codestil geht es nicht um Schönheit, sondern rein um die Wartbarkeit und die Senkung der Änderungskosten.“
- „Der Build muss fehlschlagen, wenn der Stil nicht perfekt ist. Bei der automatisierten Durchsetzung gibt es keinen Mittelweg.“
- „Das Ziel eines Styleguides ist es, den gesamten Code so aussehen zu lassen, als wäre er von einer Person geschrieben worden, nicht von einem Team aus Individualisten.“
- „Wenn ein Mensch oder eine KI die Struktur Ihres Codes nicht leicht interpretieren kann, hat der Stil seinen Hauptzweck verfehlt.“

## Relevanz: 5/5
Dieser Vortrag ist für Senior-Entwickler und Teamleiter unerlässlich, da er den praktischen Rahmen für die Durchsetzung von Konsistenz in großen Teams bietet.
