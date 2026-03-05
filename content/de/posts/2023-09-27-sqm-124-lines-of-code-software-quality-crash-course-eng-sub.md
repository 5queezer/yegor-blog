---
title: "SQM 1/24: Codezeilen [Software-Qualitäts-Crashkurs]"
date: 2023-09-27T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/q9Gr2xguP5I/maxresdefault.jpg"
  alt: "SQM 1/24: Codezeilen [Software-Qualitäts-Crashkurs]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=q9Gr2xguP5I](https://www.youtube.com/watch?v=q9Gr2xguP5I)

## Zusammenfassung
In dieser Vorlesung untersucht Yegor Bugayenko die grundlegende Rolle von Metriken in der Softwareentwicklung, basierend auf dem Management-Axiom: „Man kann nur kontrollieren, was man messen kann.“ Er unterscheidet zwischen dem „Ingenieur“, der isolierte Probleme löst, und dem „Wissenschaftler“, der nach verallgemeinerbaren, messbaren Wahrheiten sucht. Der Kern der Diskussion konzentriert sich auf die Anzahl der Codezeilen (Lines of Code, LoC). Obwohl Bill Gates LoC als Maßstab für Fortschritt kritisierte – er verglich es damit, den Baufortschritt eines Flugzeugs nach seinem Gewicht zu messen –, argumentiert Yegor, dass LoC eine wichtige Metrik bleibt, wenn man sie richtig interpretiert. Anstatt den Fortschritt zu messen, sollte LoC als Maß für den „Wartungsaufwand“ und die Komplexität betrachtet werden.

Die Vorlesung führt „Non-Commenting Source Statements“ (NCSS) ein, um Rauschen wie Kommentare und Leerzeichen herauszufiltern. Yegor schlägt jedoch eine dynamischere Alternative vor: Hits-of-Code (HoC). Im Gegensatz zu statischen LoC verfolgt HoC jede Änderung in Git. Dies stellt sicher, dass die Metrik immer ansteigt und den tatsächlichen Arbeitsaufwand widerspiegelt, selbst wenn Code gelöscht oder refaktoriert wird. Darüber hinaus spricht er Code-„Smells“ an, insbesondere Leerzeilen innerhalb von Methoden als Zeichen für fragmentierte Logik. Schließlich plädiert Yegor für einen „Leidensansatz“ bei der statischen Analyse, bei dem Entwickler Stilverletzungen manuell beheben sollten, anstatt Auto-Formatter zu verwenden, da dieser Widerstand für das langfristige Lernen notwendig sei.

## Kernaussagen
- „Den Programmierfortschritt an Codezeilen zu messen, ist wie den Fortschritt beim Flugzeugbau am Gewicht zu messen.“ (Bill Gates, zitiert von Yegor)
- „Man kann nur kontrollieren, was man messen kann; ohne Metriken ist Softwarequalität nur eine Meinung.“
- „Hits-of-Code (HoC) ist LoC überlegen, da es die Historie des Aufwands und die 'Hotspots' der Komplexität erfasst.“
- „Leerzeilen innerhalb einer Methode sind ein Code-Smell; wenn man Codeblöcke trennen muss, tut die Methode zu viel.“

## Relevanz: 5/5
Die Vorlesung ist für Teamleiter und Architekten äußerst relevant, da sie eine umstrittene Metrik (LoC) als Werkzeug für Kostenschätzung und Wartungsmanagement zurückgewinnt und modernere Alternativen wie HoC einführt.
