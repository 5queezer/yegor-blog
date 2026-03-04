---
title: "I23: A. S. Medvednikov | Die Programmiersprache V - einfach, schnell, sicher, kompiliert, Open Source"
date: 2024-05-28T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/xMGNlUZQ-6w/maxresdefault.jpg"
  alt: "I23: A. S. Medvednikov | Die Programmiersprache V - einfach, schnell, sicher, kompiliert, Open Source"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=xMGNlUZQ-6w](https://www.youtube.com/watch?v=xMGNlUZQ-6w)

## Zusammenfassung
In diesem Interview spricht Yegor Bugayenko mit Alexander Medwednikow, dem Schöpfer der Programmiersprache V (vlang). Alexander erläutert, dass V aus der praktischen Notwendigkeit heraus entstanden ist, eine Sprache zu haben, die so einfach wie Go, aber so schnell und sicher wie Rust ist – primär für die Entwicklung seines Messaging-Clients "Volt". Ein zentrales Thema ist die extreme Kompiliergeschwindigkeit von V (über eine Million Zeilen pro Sekunde), die durch einen winzigen, selbst-bootstrappenden Compiler erreicht wird, der standardmäßig auf schwere Abhängigkeiten wie LLVM verzichtet und stattdessen nach C übersetzt oder direkt Maschinencode erzeugt.

Die Diskussion umfasst technische Innovationen wie das Speichermanagement von V, das mittels Compile-Zeit-Analyse (Autofree) einen Mittelweg zwischen manueller Kontrolle und Garbage Collection sucht. Alexander betont Sicherheitsmerkmale wie das Fehlen von Null-Pointern, den Verzicht auf globale Variablen und die standardmäßige Immutabilität. Zudem thematisieren sie die Skepsis der Entwickler-Community gegenüber den ehrgeizigen Versprechen von V, der Alexander mit dem Hinweis auf das wachsende Ökosystem und funktionierende Anwendungen begegnet. Das Gespräch unterstreicht eine Philosophie der radikalen Einfachheit: Es gibt nur einen Weg, ein Problem zu lösen, und der Sprachkern bleibt klein genug, um von einem einzelnen Entwickler vollständig verstanden zu werden.

## Kernaussagen
- "V ist als Sprache ohne Altlasten konzipiert; sie übernimmt das Beste von Go, Rust und Oberon, entfernt aber die Komplexität."
- "Eine Kompilierung von 1,2 Millionen Zeilen pro Sekunde ist kein reiner Marketing-Gag; sie verändert grundlegend den Feedback-Zyklus des Entwicklers."
- "Sicherheit sollte keine akademische Übung sein; es geht darum, häufige Fehler wie Null-Pointer-Zugriffe und globale Status-Korruption durch strikte Sprachregeln zu verhindern."

## Relevanz: 5/5
Höchst relevant für Software-Ingenieure, die sich für Sprachdesign, Compiler-Performance und die Balance zwischen Sicherheit und Einfachheit in der Systemprogrammierung interessieren.
