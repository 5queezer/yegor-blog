---
title: "SQM 19/24: Kommentardichte [Crashkurs Softwarequalität]"
date: 2024-03-10T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/4_SNhBeyato/maxresdefault.jpg"
  alt: "SQM 19/24: Kommentardichte [Crashkurs Softwarequalität]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=4_SNhBeyato](https://www.youtube.com/watch?v=4_SNhBeyato)

## Zusammenfassung
In dieser Vorlesung des Kurses Software Quality Metrics (SQM) erörtert Yegor Bugayenko die "Kommentardichte" als Metrik zur Bewertung der Qualität einer Codebasis. Die Kernprämisse ist, dass das Verhältnis von Kommentaren zu Code ein wichtiger Indikator ist, jedoch nur, wenn man zwischen verschiedenen Arten von Kommentaren unterscheidet. Bugayenko zieht eine strenge Grenze zwischen API-Dokumentation (wie Javadoc) und Inline-Kommentaren innerhalb von Methoden.

Er argumentiert, dass Dokumentation auf Klassen- und Methodenebene obligatorisch und äußerst nützlich ist, da sie das "Was" und "Warum" der Softwarekomponenten definiert und klare Verträge schafft. Folglich ist eine hohe Dichte an API-Dokumentation ein Zeichen für ein qualitativ hochwertiges Projekt.

Umgekehrt werden Inline-Kommentare als klares "Code Smell" (schlechter Programmierstil) betrachtet. Wenn ein Entwickler das Bedürfnis hat, mit einem Kommentar zu erklären, *wie* ein bestimmter Codeblock funktioniert, bedeutet dies, dass der Code selbst zu komplex oder schlecht benannt ist. Die Lösung besteht nicht darin, einen Kommentar hinzuzufügen, sondern den Code zu refaktorisieren – meist durch das Auslagern in kleinere, gut benannte Methoden. Zudem sind Kommentare nicht ausführbar und veralten oft, was zu irreführenden "Lügen" im Repository führt. Letztendlich plädiert Bugayenko dafür, die Architekturdokumentation zu maximieren und die Inline-Kommentardichte auf absolut null zu reduzieren.

## Kernaussagen
- "Inline-Kommentare sind ein Warnsignal; wenn Sie erklären müssen, wie Ihr Code funktioniert, sollten Sie ihn stattdessen refaktorisieren."
- "Es gibt einen strikten Unterschied zwischen API-Dokumentation (dem Vertrag) und internen Kommentaren (der Implementierung)."
- "Code lügt nie, aber Kommentare veralten schnell und werden zu Lügen, die zukünftige Entwickler in die Irre führen."
- "Eine hochwertige Codebasis maximiert die Dichte der API-Dokumentation und hält die Inline-Kommentardichte bei null."

## Relevanz: 5/5
Dieses Thema ist für Softwareentwickler und Teamleiter äußerst relevant, da es klare Regeln für die Wartbarkeit von Code, Refactoring und Dokumentationspraktiken in der objektorientierten Programmierung aufstellt.
