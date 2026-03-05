---
title: "Der Schmerz von OOP, Lektion #6: NULL-Referenzen"
date: 2023-08-09T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
  - "oop"
  - "ai"
cover:
  image: "https://img.youtube.com/vi/cTyIF20Kmz4/maxresdefault.jpg"
  alt: "Der Schmerz von OOP, Lektion #6: NULL-Referenzen"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=cTyIF20Kmz4](https://www.youtube.com/watch?v=cTyIF20Kmz4)

## Zusammenfassung
In dieser Lektion setzt sich Yegor Bugayenko kritisch mit NULL-Referenzen in der objektorientierten Programmierung auseinander, die er als den "Milliarden-Dollar-Fehler" bezeichnet. Er argumentiert, dass NULL ein prozedurales Überbleibsel aus Sprachen wie C ist, das Objekte als bloße Speicheradressen und nicht als autonome Einheiten behandelt. Wenn eine Methode NULL zurückgibt, bricht sie den Vertrag mit dem Aufrufer und zwingt diesen zu "defensiver Programmierung" durch ständige `if (x != null)`-Prüfungen.

Das Hauptproblem ist laut Yegor, dass NULL kein Objekt ist; es besitzt kein Verhalten und kann nicht auf Nachrichten reagieren. Dies untergräbt die Polymorphie und führt dazu, dass die Kapselung aufgehoben wird, da die Logik zur Behandlung von "Nichts" nach außen verlagert wird. Als Lösung schlägt er das "Fail Fast"-Prinzip vor: Wenn ein Objekt nicht geliefert werden kann, sollte sofort eine Exception geworfen oder ein "Null Object" zurückgegeben werden—eine Implementierung des Interfaces, die sinnvoll "nichts" tut. Er fordert, dass ein sauberes Design niemals NULL als Argument oder Rückgabewert zulassen sollte.

## Kernaussagen
- NULL ist kein Objekt, sondern ein technischer Zeiger, der in der konzeptionellen Welt der OOP nichts zu suchen hat.
- Jede NULL-Prüfung ist ein Zeichen für ein architektonisches Versagen und eine Verletzung des "Tell, Don't Ask"-Prinzips.
- Die Rückgabe von NULL ist ein Verrat am Vertrag der Methode und wälzt die Verantwortung auf den Aufrufer ab.
- Das Null-Object-Pattern oder das Werfen von Exceptions hält den Code deklarativ und stabil.

## Relevanz: 5/5
Diese Lektion ist von höchster Bedeutung für Software-Architekten, die die Codequalität durch die Eliminierung der häufigsten Ursache für Laufzeitfehler (NullPointerExceptions) verbessern wollen.
