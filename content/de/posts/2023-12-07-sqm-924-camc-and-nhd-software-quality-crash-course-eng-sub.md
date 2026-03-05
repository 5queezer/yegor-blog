---
title: "SQM 9/24: CAMC und NHD [Software-Qualitäts-Crashkurs]"
date: 2023-12-07T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/oCxJ_YSSAGo/maxresdefault.jpg"
  alt: "SQM 9/24: CAMC und NHD [Software-Qualitäts-Crashkurs]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=oCxJ_YSSAGo](https://www.youtube.com/watch?v=oCxJ_YSSAGo)

## Zusammenfassung
In dieser Vorlesung konzentriert sich Yegor Bugayenko auf die Messung der Klassen-Kohäsion mittels der Metriken CAMC (Cohesion Among Methods in Class) und NHD (Normalized Hamming Distance). Er beginnt mit einer Analyse des Rational Unified Process (RUP) und betont, dass trotz der heutigen Bevorzugung von Agile die architektonische Disziplin des RUP wichtige Lehren für die Softwarequalität bereithielt, insbesondere in Bezug auf die Entkopplung durch Schnittstellen.

Der technische Kern befasst sich mit der Parameter-Vorkommens-Matrix. CAMC berechnet das Verhältnis der tatsächlich verwendeten Parametertypen zur Gesamtzahl der möglichen Kombinationen in einer Klasse. Ein hoher CAMC-Wert deutet auf eine starke thematische Einheit hin. NHD geht einen Schritt weiter und nutzt die Hamming-Distanz, um die strukturelle Ähnlichkeit zwischen Methoden zu bewerten. Dies hilft dabei, "unnatürliche" Klassen zu identifizieren, in denen Methoden in unabhängige Gruppen zerfallen.

Abschließend verknüpft Bugayenko diese Metriken mit dem Interface Segregation Principle (ISP). Am Beispiel der Java-Klasse `InputStream` zeigt er auf, wie ein "fettes Interface" die Kohäsion senkt und Entwickler dazu zwingt, Dummy-Methoden oder Ausnahmen für nicht unterstützte Funktionen zu implementieren, was die Wartbarkeit erheblich verschlechtert.

## Kernaussagen
- "Metriken sind der Weg, um Architektur von einer subjektiven Meinung in eine objektive Wissenschaft zu verwandeln."
- "Ein niedriges CAMC-Ergebnis ist ein klares Signal dafür, dass eine Klasse gegen das Single Responsibility Principle verstößt."
- "Das Design von Java's InputStream ist fehlerhaft, da es Markierungs- und Reset-Logik in eine Basisabstraktion zwingt, die sie nicht universell garantieren kann."
- "Hamming-Distanz in der Programmierung erlaubt es uns, die 'Fremdartigkeit' von Methoden innerhalb desselben Objekts mathematisch zu erfassen."

## Relevanz: 5/5
Diese Vorlesung ist höchst relevant für Software-Architekten, die formale Methoden zur Bewertung von Objektdesign und Kohäsion verstehen wollen.
