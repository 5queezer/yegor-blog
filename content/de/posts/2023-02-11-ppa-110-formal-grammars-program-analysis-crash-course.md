---
title: "PPA 1/10: Formale Grammatiken [Programmanalyse-Crashkurs]"
date: 2023-02-11T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/rsoPqA1CYmE/maxresdefault.jpg"
  alt: "PPA 1/10: Formale Grammatiken [Programmanalyse-Crashkurs]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=rsoPqA1CYmE](https://www.youtube.com/watch?v=rsoPqA1CYmE)

## Zusammenfassung
In dieser ersten Vorlesung des Programmanalyse-Crashkurses führt Yegor Bugayenko formale Grammatiken als die wesentliche Grundlage für die Softwareanalyse ein. Die Sitzung konzentriert sich auf das „Front-End“ der Analyse-Pipeline: die Umwandlung von Quellcode aus einem einfachen Zeichenstrom in ein strukturiertes mathematisches Modell. Bugayenko betont, dass vor jeder sinnvollen Analyse des Verhaltens eines Programms (Semantik) eine strenge Definition seiner Struktur (Syntax) erforderlich ist.

Der Vortrag beleuchtet die Geschichte und Bedeutung der Backus-Naur-Form (BNF) und verfolgt deren Ursprünge bis in die späten 1950er Jahre zurück. Dieser Übergang von informellen Beschreibungen zu formalen Notationen ermöglichte die Erstellung eindeutiger Sprachspezifikationen. Der Transformationsprozess wird in zwei Hauptphasen unterteilt: Die lexikalische Analyse, bei der Zeichen zu „Terminals“ (Token wie Schlüsselwörter und Bezeichner) gruppiert werden, und die Syntaxanalyse, die diese Token mithilfe von „Nicht-Terminals“ (Platzhalter wie `<Anweisung>` oder `<Ausdruck>`) in einem abstrakten Syntaxbaum (AST) organisiert. Formalisierung wird als Voraussetzung für die Beseitigung von Mehrdeutigkeiten dargestellt, was es Computern ermöglicht, komplexe Aufgaben wie statische Fehlersuche, Code-Optimierung und formale Verifizierung durchzuführen. Letztendlich dienen formale Grammatiken als das Tor, das Rohtext in eine für automatisiertes Denken geeignete Datenstruktur verwandelt, die die Basis für alle weiteren Analyseschritte im Kurs bildet.

## Kernaussagen
* „Formale Grammatiken sind das mathematische Werkzeug, um Mehrdeutigkeiten aus Sprachdefinitionen zu entfernen.“
* „Man kann nicht analysieren, was ein Programm tut, bevor man nicht streng definiert hat, wie es aussieht.“
* „Die lexikalische Analyse macht aus Zeichen Terminals; die Syntaxanalyse macht aus Terminals eine Baumstruktur.“
* „Die Einführung der BNF machte Programmiersprachen zu mathematisch beweisbaren Einheiten.“

## Relevanz: 5/5
Grundlegend für das Verständnis von Compilern, statischen Analysetools und der Definition eigener Sprachen.
