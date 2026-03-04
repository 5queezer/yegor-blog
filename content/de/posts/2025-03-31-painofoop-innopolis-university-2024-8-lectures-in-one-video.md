---
title: "Schmerz der OOP, Innopolis Universität, 2024, 8 Vorlesungen in einem Video"
date: 2025-03-31T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
  - "oop"
  - "ai"
cover:
  image: "https://img.youtube.com/vi/awB08yeXfZM/maxresdefault.jpg"
  alt: "Schmerz der OOP, Innopolis Universität, 2024, 8 Vorlesungen in einem Video"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=awB08yeXfZM](https://www.youtube.com/watch?v=awB08yeXfZM)

## Zusammenfassung
Yegor Bugayenkos Kurs „Pain of OOP“ an der Universität Innopolis nimmt gängige Praktiken der objektorientierten Programmierung (OOP) systematisch auseinander. Er argumentiert, dass moderne Enterprise-Software größtenteils aus prozeduraler Programmierung besteht, die lediglich als OOP getarnt ist. In acht umfassenden Vorlesungen kritisiert Bugayenko tief verwurzelte Gewohnheiten: Getter und Setter, statische Methoden, Null-Referenzen und ORM-Frameworks. Er plädiert stattdessen für „Elegant Objects“, ein strengeres und reineres Paradigma, bei dem Objekte als aktive, lebendige Entitäten und nicht als passive Datencontainer behandelt werden.

Der Kurs behandelt detailliert praktische Regeln für ein echtes objektorientiertes Design. Bugayenko setzt sich für strikte Unveränderlichkeit (Immutability) ein und argumentiert, dass veränderliche Objekte unvorhersehbar und schwer zu warten sind. Er fordert die absolute Auslöschung von `null` und empfiehlt stattdessen die Verwendung von Null-Objekten. Darüber hinaus müssen Konstruktoren absolut codefrei sein – ihre einzige Aufgabe besteht darin, Variablen zuzuweisen. Jegliche Berechnung sollte verzögert werden, bis eine spezifische Methode aufgerufen wird. Wahre Kapselung ist ein zentrales Thema; Bugayenko erklärt, dass die Offenlegung des internen Zustands durch DTOs (Data Transfer Objects) die Kohäsion des Objekts zerstört.

Er kritisiert auch moderne Testpraktiken, insbesondere Mocking-Frameworks, und empfiehlt stattdessen die Verwendung von „Fake“-Objekten, die dieselben Interfaces implementieren. Komposition wird gegenüber Vererbung stark bevorzugt, und der intensive Einsatz von Interfaces und Decorators wird als der richtige Weg zur Erweiterung von Verhalten präsentiert. Letztendlich bezieht sich der „Schmerz“ auf die steile Lernkurve und das Unbehagen, das Entwickler verspüren, wenn sie toxische Industriestandards verlernen müssen – belohnt werden sie jedoch mit einer äußerst wartbaren und stabilen Softwarearchitektur.

## Kernaussagen
- "Getter und Setter berauben Objekte ihrer Würde und machen sie zu bloßen Datenbehältern."
- "Statische Methoden sind ein prozeduraler Virus in der objektorientierten Welt."
- "Konstruktoren müssen codefrei sein; ein Objekt sollte schnell instanziiert werden und erst arbeiten, wenn seine Methoden aufgerufen werden."
- "Null ist kein Objekt; die Rückgabe oder Annahme von null ist ein Vertrauensbruch zwischen Objekten."

## Relevanz: 5/5
Diese Vorlesungsreihe ist äußerst relevant, da sie die Standardpraktiken des Software-Engineerings grundlegend infrage stellt und eine strikte, kohärente Alternative für den Entwurf robuster objektorientierter Systeme bietet.
