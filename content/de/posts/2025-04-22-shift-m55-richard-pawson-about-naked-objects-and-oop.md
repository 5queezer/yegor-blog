---
title: "Shift-M/55: Richard Pawson über Naked Objects und OOP"
date: 2025-04-22T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
  - "oop"
cover:
  image: "https://img.youtube.com/vi/x6LKw-iQHZQ/maxresdefault.jpg"
  alt: "Shift-M/55: Richard Pawson über Naked Objects und OOP"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=x6LKw-iQHZQ](https://www.youtube.com/watch?v=x6LKw-iQHZQ)

## Zusammenfassung
In dieser Folge des Shift-M-Podcasts spricht Yegor Bugayenko mit Richard Pawson, dem Schöpfer des "Naked Objects"-Musters. Die Diskussion dreht sich um die grundlegende Philosophie der objektorientierten Programmierung (OOP) und deren heutige Umsetzung. Pawson erläutert die drei Prinzipien von Naked Objects: die vollständige Kapselung der Geschäftslogik in Domänenobjekten, eine Benutzeroberfläche (UI), die diese Objekte direkt widerspiegelt, und die automatische Erstellung dieser UI aus dem Domänenmodell.

Ein zentraler Punkt des Gesprächs ist die Unterscheidung zwischen Skalierbarkeit für Leistung und Skalierbarkeit für Komplexität. Pawson betont, dass Naked Objects besonders stark darin ist, die enorme Komplexität großer Enterprise-Systeme zu bewältigen. Er führt das Beispiel des irischen Sozialministeriums an, das ein System mit über 5.000 Klassen erfolgreich betreibt. 

Pawson kritisiert zudem, dass moderne OOP oft zu einer prozeduralen Programmierung mit "Datencontainern" (DTOs) verkommen ist. Er plädiert für eine Rückkehr zu behavioristischen Objekten, wie sie ursprünglich in Smalltalk angedacht waren. Er unterscheidet dabei zwischen "Sovereign Applications" (Experten-Systeme), für die Naked Objects ideal ist, und "Transient Applications" (Websites für Endverbraucher), bei denen ein individuelles Design wichtiger ist als die direkte Objektrepräsentation.

## Kernaussagen
- "Naked Objects ermöglicht es, Komplexität zu skalieren, indem man die UI-Entwicklung als separaten Schritt eliminiert."
- "Der Benutzer sollte als Problemlöser agieren, der sich in einer Welt von Objekten bewegt, statt nur starren Prozessen zu folgen."
- "Echte OOP bedeutet, dass das Objekt selbst weiß, was es tun kann, anstatt nur Daten für externe Services bereitzustellen."
- "Die Benutzeroberfläche sollte eine direkte Projektion des Domänenmodells sein, um die 'Ubiquitous Language' zu wahren."

## Relevanz: 5/5
Die Folge ist für Software-Architekten von großem Wert, da sie die gängige Architekturpraxis hinterfragt und einen radikalen, aber bewährten Ansatz zur Beherrschung von Geschäftslogik aufzeigt.
