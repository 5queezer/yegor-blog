---
title: "Der Schmerz von OOP Lektion #4: Setter und Objekt-Mutabilität"
date: 2023-07-04T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
  - "oop"
  - "ai"
cover:
  image: "https://img.youtube.com/vi/h0jf9E1tjf4/maxresdefault.jpg"
  alt: "Der Schmerz von OOP Lektion #4: Setter und Objekt-Mutabilität"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=h0jf9E1tjf4](https://www.youtube.com/watch?v=h0jf9E1tjf4)

## Zusammenfassung
In der vierten Vorlesung der Reihe „The Pain of OOP“ übt Yegor Bugayenko scharfe Kritik an der Verwendung von Settern und dem Konzept der Objekt-Mutabilität (Veränderbarkeit). Seine zentrale These ist, dass Setter Objekte in passive „Datensäcke“ verwandeln, ihnen ihre Autonomie rauben und das fundamentale Prinzip der Kapselung verletzen. In der reinen objektorientierten Programmierung sollte ein Objekt eine autarke Einheit sein, die ihren eigenen Zustand und ihre eigene Logik verwaltet. Wenn wir Setter verwenden, erlauben wir externen Prozeduren, das Innere des Objekts zu manipulieren, was objektorientierten Code faktisch in prozeduralen Code verwandelt, bei dem die Logik über die gesamte Anwendung verstreut ist.

Yegor hebt drei kritische Probleme hervor, die durch Mutabilität verursacht werden. Erstens der Verlust der Identität: Wenn sich die Felder eines Objekts ständig ändern, wird es schwierig sicherzustellen, dass es dieselbe Geschäftseinheit darstellt. Zweitens die immense Schwierigkeit beim Debuggen, da der Zustand eines Objekts jederzeit von jedem Teil des Programms aus geändert werden kann, was die Suche nach der Fehlerquelle erschwert. Drittens der Mangel an inhärenter Thread-Sicherheit; veränderliche Objekte erfordern komplexe Sperrmechanismen in Multi-Thread-Umgebungen. Die einzige architektonisch sinnvolle Lösung ist die vollständige Immutabilität (Unveränderlichkeit). Objekte sollten alle notwendigen Daten über den Konstruktor erhalten, und jede „Änderung“ sollte zur Erstellung einer neuen Instanz führen. Dieser Ansatz macht Software vorhersehbar, vereinfacht das Testen und zwingt Entwickler, in realen Verhaltensweisen statt in technischen Feldmanipulationen zu denken.

## Kernaussagen
1. „Setter verwandeln Objekte in einfache Datensäcke.“
2. „Ein Objekt muss eine lebendige Einheit sein, kein passiver Container.“
3. „Mutabilität ist die Hauptquelle für Probleme und Fehler in der Softwarearchitektur.“
4. „In einer wahrhaft objektorientierten Welt sollten alle Objekte standardmäßig unveränderlich sein.“

## Relevanz: 5/5
Diese Vorlesung ist grundlegend für das Verständnis der „Elegant Objects“-Philosophie. Sie stellt gängige Industriestandards (wie Java Beans) in Frage und bietet einen radikalen, aber konsistenten Ansatz für wartbare Systeme.
