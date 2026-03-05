---
title: "Der Schmerz von OOP, Lektion #8: Vererbung"
date: 2023-08-22T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
  - "oop"
  - "ai"
cover:
  image: "https://img.youtube.com/vi/m0OEOoGgIuM/maxresdefault.jpg"
  alt: "Der Schmerz von OOP, Lektion #8: Vererbung"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=m0OEOoGgIuM](https://www.youtube.com/watch?v=m0OEOoGgIuM)

## Zusammenfassung
In dieser Vorlesung setzt sich Yegor Bugayenko mit einem der umstrittensten Themen der objektorientierten Programmierung auseinander: der Vererbung. Er unterscheidet strikt zwischen "Subtyping" (Schnittstellen) und "Implementierungsvererbung" (das Schlüsselwort `extends`). Während Subtyping als Grundlage für Polymorphie und das Liskovsche Substitutionsprinzip (LSP) gelobt wird, wird die Implementierungsvererbung als prozeduraler "Hack" zur Codewiederverwendung verurteilt, der die Kapselung zerstört.

Bugayenko argumentiert, dass Vererbung eine enge Kopplung zwischen Eltern- und Kindklassen erzeugt, was zum Problem der "fragilen Basisklasse" führt – bei dem Änderungen in einer Basisklasse unerwartet Unterklassen beschädigen. Er kritisiert die Verwendung von `protected`-Modifikatoren, da diese das "Black-Box"-Prinzip von Objekten verletzen. Die Vorlesung behandelt auch die Tücken der Methodenüberladung und der Mehrfachvererbung. Als Lösung plädiert er für "Komposition statt Vererbung" und schlägt vor, dass Objekte Verhalten kapseln und delegieren sollten, anstatt es zu erben. Dieser Ansatz führt zu kleineren, wartungsfreundlicheren und entkoppelten Codebasen.

## Kernaussagen
- "Implementierungsvererbung hat nichts mit Objektdenken zu tun; sie ist eine prozedurale Abkürzung für faule Codewiederverwendung."
- "In dem Moment, in dem Sie den `protected`-Modifikator verwenden, haben Sie zugegeben, dass Ihre Kapselung fehlerhaft ist."
- "Objekte sollten unabhängige Verhaltenseinheiten sein, keine Datentaschen mit gemeinsamen Implementierungsdetails."
- "Ein wahrer OOP-Architekt nutzt Interfaces, um Typen zu definieren, und Komposition, um Logik wiederzuverwenden."

## Relevanz: 5/5
Diese Vorlesung ist äußerst relevant, da sie gängige Industriestandards infrage stellt und tief in Architekturprinzipien eintaucht, die die Wartbarkeit und Skalierbarkeit von Software direkt beeinflussen.
