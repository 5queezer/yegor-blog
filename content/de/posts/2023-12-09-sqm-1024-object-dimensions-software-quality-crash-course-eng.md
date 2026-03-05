---
title: "SQM 10/24: Objekt-Dimensionen [Software-Qualitäts-Crashkurs]"
date: 2023-12-09T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
  - "oop"
cover:
  image: "https://img.youtube.com/vi/jdEFoz-OQ44/maxresdefault.jpg"
  alt: "SQM 10/24: Objekt-Dimensionen [Software-Qualitäts-Crashkurs]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=jdEFoz-OQ44](https://www.youtube.com/watch?v=jdEFoz-OQ44)

## Zusammenfassung
In dieser Vorlesung erörtert Yegor Bugayenko die quantitativen Dimensionen der objektorientierten Programmierung. Anstatt sich auf die bloße Anzahl der Zeilen (LoC) zu verlassen, stellt er Metriken vor, die die strukturelle Qualität eines Systems messen: Kapselung, Vererbung, Polymorphie und Komplexität. Im Mittelpunkt stehen die MOOD-Metriken (Abreu) und die C&K-Metriken (Chidamber & Kemerer).

Bugayenko betont die Bedeutung des Method Hiding Factor (MHF) und des Attribute Hiding Factor (AHF). Er argumentiert, dass Attribute fast immer privat sein sollten (AHF nahe 1), da eine niedrige Kapselung das System in ein prozedurales Design verwandelt. Bei der Vererbung (MIF/AIF) warnt er vor einer zu flachen Hierarchie, aber auch vor zu komplexen Abhängigkeiten, die durch zu viele Basismethoden entstehen.

Zusätzlich werden Metriken wie die Vererbungstiefe (DIT) und die Anzahl der Kinder (NOC) analysiert. Diese zeigen auf, wie kritisch eine Klasse für das Gesamtsystem ist. Eine hohe "Response For a Class" (RFC) wird als Warnsignal für starke Kopplung und erschwerte Wartbarkeit identifiziert. Die Kernaussage ist, dass Softwarequalität kein Bauchgefühl sein sollte, sondern durch mathematische Verhältnisse objektiv bewertbar ist.

## Kernaussagen
- "Codezeilen sagen wenig über Qualität aus; wir müssen die Dimensionen von Kapselung und Vererbung messen."
- "Ein niedriger Attribut-Hiding-Faktor bedeutet, dass man kein OOP betreibt, sondern lediglich Datenstrukturen prozedural manipuliert."
- "Vererbung ist ein Werkzeug zur Wiederverwendung, aber ein zu hoher Faktor macht Basisklassen zerbrechlich und schwer zu ändern."
- "Der RFC-Wert (Response For a Class) ist entscheidend für die Testbarkeit – ein zu komplexes Antwortverhalten führt zu Fehlern."

## Relevanz: 5/5
Essentiell für Entwickler, die Metriken zur Code-Analyse einführen möchten, um Design-Entscheidungen objektiv zu begründen.
