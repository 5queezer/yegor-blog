---
title: "Der Schmerz von OOP, Vorlesung #5: Das Suffix -ER ist böse"
date: 2023-07-10T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
  - "oop"
  - "ai"
cover:
  image: "https://img.youtube.com/vi/6GMiosTLUTc/maxresdefault.jpg"
  alt: "Der Schmerz von OOP, Vorlesung #5: Das Suffix -ER ist böse"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=6GMiosTLUTc](https://www.youtube.com/watch?v=6GMiosTLUTc)

## Zusammenfassung
In dieser provokanten Vorlesung aus der Reihe „The Pain of OOP“ kritisiert Yegor Bugayenko eine der am weitesten verbreiteten Benennungskonventionen in der Softwareentwicklung: das Suffix „-er“. Er argumentiert, dass Klassennamen wie Manager, Controller, Helper, Validator oder Parser weit mehr als nur schlechter Stil sind; sie sind Symptome eines tief verwurzelten prozeduralen Denkens innerhalb einer vermeintlich objektorientierten Welt. Bugayenkos zentraler Punkt ist, dass ein Objekt durch das definiert werden sollte, „was es ist“ (ein Substantiv), und nicht durch das, „was es tut“ (ein als Substantiv getarntes Verb). Wenn wir eine Klasse `UserManager` nennen, geben wir implizit zu, dass wir eine passive Datenstruktur geschaffen haben, die von einem externen „Puppenspieler“ manipuliert wird. Dies führt unweigerlich zu einem „Anemic Domain Model“, bei dem Daten und Logik getrennt sind, was das Prinzip der Kapselung vollständig zerstört.

Die Vorlesung plädiert für einen anthropomorphen Ansatz in der Programmierung. Objekte sollten als lebendige Organismen betrachtet werden, denen man Verantwortung überträgt, anstatt sie als Sklaven für funktionale Aufgaben zu missbrauchen. Bugayenko schlägt vor, anstelle eines `FileSaver` eine Klasse wie `SavedFile` oder einfach ein intelligentes `File`-Objekt zu entwerfen, das seine eigene Persistenz repräsentiert. Durch den Verzicht auf das „-er“-Suffix werden Entwickler gezwungen, die Identität und die eigentliche Aufgabe ihrer Klassen neu zu bewerten. Dies führt zu kleineren, kohärenteren und deklarativeren Systemen. Bugayenko fordert die Branche heraus, sich von „Service-Layers“ und „Utility-Klassen“ zu verabschieden, da diese in seinen Augen lediglich prozedurale „Mülltonnen“ sind, die eine echte objektorientierte Dekomposition verhindern.

## Kernaussagen
- Objekte sind keine Werkzeuge oder Funktionssammlungen, sondern autonome Partner in einem Ökosystem.
- Wer eine Klasse „Manager“ nennt, gesteht ein, dass er die wahre Identität und den Zweck des Objekts nicht verstanden hat.
- Das Suffix „-er“ markiert den Übergang von OOP zu prozeduraler Programmierung, da es die Logik von den Daten trennt.
- Dekomposition muss nach Entitäten (Substantiven) erfolgen, nicht nach Funktionen (Verben). Ein `ValidatedUser` ist besser als ein `UserValidator`.

## Relevanz: 5/5
Diese Vorlesung ist essenziell für Software-Architekten und Entwickler, die die Prinzipien von Clean Code und echter Objektorientierung tiefgreifend verstehen wollen.
