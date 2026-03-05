---
title: "SQM 8/24: TCC und LCC [Crashkurs Softwarequalität]"
date: 2023-12-02T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/JOKxjpAglFU/maxresdefault.jpg"
  alt: "SQM 8/24: TCC und LCC [Crashkurs Softwarequalität]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=JOKxjpAglFU](https://www.youtube.com/watch?v=JOKxjpAglFU)

## Zusammenfassung
In dieser Folge seines Kurses über Softwarequalität erläutert Yegor Bugayenko die Messung der Klassenkohäsion mittels der Metriken Tight Class Cohesion (TCC) und Loose Class Cohesion (LCC). Basierend auf den Arbeiten von Bieman und Kang wird Kohäsion als das entscheidende Merkmal definiert, das den Zusammenhalt eines Objekts bestimmt. Eine hohe Kohäsion ist ein Zeichen für ein fokussiertes Design, bei dem alle Teile einer Klasse einem gemeinsamen Zweck dienen.

TCC berechnet das Verhältnis von direkt verbundenen Methodenpaaren (solche, die auf dieselbe Instanzvariable zugreifen) zur Gesamtzahl der möglichen Paare. LCC berücksichtigt zusätzlich indirekte Verbindungen über Transitivität. Yegor warnt davor, dass Klassen mit einem TCC-Wert unter 0,5 oft "Gott-Objekte" oder lose Sammlungen von Funktionen sind, die keine echte Einheit bilden.

Ein zentraler Kritikpunkt des Vortrags ist die Verwendung von Vererbung. Laut Bugayenko führt Vererbung häufig zu einer Verwässerung der Kohäsion, da Unterklassen Code erben, den sie nicht benötigen oder der nicht zu ihrem primären Zweck passt. Er plädiert stattdessen für Komposition, um die strukturelle Integrität und Testbarkeit des Codes zu gewährleisten.

## Kernaussagen
- „Kohäsion ist der Zement eines gut entworfenen Moduls – ohne sie zerfällt das Objekt in lose Einzelteile.“
- „Ein TCC-Wert unter 0,5 ist ein klares Signal dafür, dass eine Klasse zu viele Verantwortlichkeiten hat.“
- „Vererbung ist oft nur ein prozeduraler Trick zur Wiederverwendung von Code, der die objektorientierte Kohäsion zerstört.“
- „Metriken wie TCC und LCC machen architektonische Qualität messbar und entziehen sie der rein subjektiven Meinung.“

## Relevanz: 5/5
Die Anwendung mathematischer Metriken auf OOP-Designprinzipien bietet eine fundierte Grundlage für Code-Reviews und Refactoring-Entscheidungen.
