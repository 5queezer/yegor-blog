---
title: "SQM 7/24: LCOM [Software-Qualitäts-Crashkurs]"
date: 2023-11-14T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/74YigDo8_BE/maxresdefault.jpg"
  alt: "SQM 7/24: LCOM [Software-Qualitäts-Crashkurs]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=74YigDo8_BE](https://www.youtube.com/watch?v=74YigDo8_BE)

## Zusammenfassung
In dieser Vorlesung analysiert Yegor Bugayenko das Konzept der Kohäsion, wobei der Schwerpunkt auf der Metrik LCOM (Lack of Cohesion of Methods) liegt. Er beginnt mit der Gegenüberstellung von Kohäsion (die Stärke der Bindung innerhalb eines Moduls) und Kopplung (die Abhängigkeit zwischen Modulen). Das Ziel jeder sauberen Architektur ist eine hohe Kohäsion bei gleichzeitig geringer Kopplung. Eine Klasse ohne Kohäsion gleicht einer "Rumpelkammer", in der unzusammenhängende Funktionen wahllos gesammelt werden.

Der Vortrag beleuchtet die klassische Hierarchie der Kohäsion – von der zufälligen (Coincidental) bis zur funktionalen (Functional) Bindung. Der technische Kern befasst sich mit der LCOM-Metrik nach Chidamber und Kemerer. Yegor erklärt, dass LCOM misst, inwieweit Methoden einer Klasse auf dieselben Instanzvariablen zugreifen. Ein hoher LCOM-Wert ist ein klares Indiz für ein "Code-Smell", das darauf hindeutet, dass die Klasse das Single-Responsibility-Prinzip (SRP) verletzt.

Besondere Aufmerksamkeit widmet er der Variante LCOM4. Diese nutzt einen graphbasierten Ansatz: Wenn LCOM4 größer als 1 ist, bedeutet dies, dass die Klasse in unabhängige Komponenten zerfällt und somit zwingend aufgeteilt werden sollte. Yegor empfiehlt Tools wie "jpeek", um diese theoretischen Metriken in der Praxis sichtbar und nutzbar zu machen.

## Kernaussagen
- "Kohäsion ist der Klebstoff eines Moduls; eine schwache Bindung führt zwangsläufig zu instabilem Code."
- "LCOM4 liefert den mathematischen Beweis für schlechtes Design: Ein Wert über 1 bedeutet, dass man eigentlich mehrere Klassen in einer hat."
- "Hohe Kohäsion ist der beste Schutz gegen das 'God Object'-Antipattern."
- "Metriken wie LCOM sind keine bloße Theorie, sondern essenzielle Werkzeuge zur Reduzierung von technischer Schuld."

## Relevanz: 5/5
Die Vorlesung ist hochrelevant für die objektorientierte Programmierung, da sie abstrakte Designprinzipien in messbare Qualitätskriterien überführt.
