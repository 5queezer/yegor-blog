---
title: "PPA 8/10: Symbolische Ausführung [Crashkurs Programmanalyse]"
date: 2023-04-28T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/PaCEIGcnx80/maxresdefault.jpg"
  alt: "PPA 8/10: Symbolische Ausführung [Crashkurs Programmanalyse]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=PaCEIGcnx80](https://www.youtube.com/watch?v=PaCEIGcnx80)

## Zusammenfassung
In dieser Vorlesung erklärt Yegor Bugayenko die symbolische Ausführung als eine Methode der Programmanalyse, bei der ein Programm mit "symbolischen" anstelle von konkreten Werten "simuliert" wird. Anstatt eine Variable mit einer Zahl wie 10 zu belegen, wird ihr ein Symbol (z. B. $X$) zugewiesen. Während der Analyse werden Operationen an diesen Symbolen durchgeführt, sodass Variablen zu komplexen mathematischen Ausdrücken werden.

Ein zentrales Element sind die Pfadbedingungen (Path Conditions). Wenn das Programm auf eine Verzweigung (z. B. eine `if`-Anweisung) trifft, teilt sich die Analyse in zwei Pfade auf. Für jeden Pfad wird die entsprechende logische Bedingung gespeichert. Ein Constraint-Solver (wie Z3) prüft dann, ob ein Pfad überhaupt erreichbar ist. Wenn der Solver eine Lösung findet, kann er automatisch Testdaten generieren, die genau diesen Pfad im echten Programm auslösen.

Die symbolische Ausführung ist besonders stark darin, versteckte Fehler wie Pufferüberläufe oder Divisionen durch Null zu finden, die beim normalen Testen oft übersehen werden. Die größte Herausforderung bleibt jedoch die "Pfadexplosion": Da die Anzahl der möglichen Pfade bei Schleifen und vielen Verzweigungen exponentiell ansteigt, stößt die Methode bei großen Programmen an ihre Rechengrenzen.

## Kernaussagen
* „Symbolische Ausführung ist keine echte Ausführung, sondern eine Simulation der Logik.“
* „Anstatt mit Zahlen zu rechnen, arbeiten wir mit algebraischen Symbolen, um alle Möglichkeiten abzudecken.“
* „Die Pfadexplosion ist der größte Feind; wir können nicht jede Abzweigung in einer komplexen Software analysieren.“
* „Automatisierte Testgenerierung durch SMT-Solver ist die Zukunft der Softwarequalität.“

## Relevanz: 5/5
Dieses Thema ist essenziell für Software-Architekten und Entwickler, die sich mit formaler Verifikation und automatisierter Fehlererkennung beschäftigen, um die Zuverlässigkeit kritischer Systeme zu erhöhen.
