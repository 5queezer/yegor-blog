---
title: "Build-Automatisierung am Beispiel von Makefile (EQSP 7-8/20)"
date: 2022-10-23T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/tHNBhNlUah8/maxresdefault.jpg"
  alt: "Build-Automatisierung am Beispiel von Makefile (EQSP 7-8/20)"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=tHNBhNlUah8](https://www.youtube.com/watch?v=tHNBhNlUah8)

## Zusammenfassung
In dieser Lektion aus dem "Software Quality Crash Course" legt Yegor Bugayenko dar, dass die Automatisierung des Build-Prozesses eine Grundvoraussetzung für Softwarequalität ist. Er propagiert `Makefile` als universelle Schnittstelle für jedes Projekt, unabhängig von der verwendeten Programmiersprache. Das zentrale Konzept ist das "One-Click-Build"-Prinzip: Jeder Entwickler oder CI-Server muss in der Lage sein, das Projekt mit einem einzigen Befehl (`make`) vollständig zu bauen und zu validieren, ohne manuelle Vorbereitungen treffen zu müssen.

Ein entscheidender Vorteil von Makefile ist seine deklarative Natur, die auf "Zielen" (targets) und "Abhängigkeiten" (dependencies) basiert. Dies ermöglicht inkrementelle Builds, bei denen nur veränderte Komponenten neu verarbeitet werden. Yegor betont, dass der Build-Prozess als "Quality Gate" fungieren muss, indem er Linter, statische Analysen und Tests integriert. Er empfiehlt, auch komplexe Werkzeuge wie Docker oder Maven hinter Makefile-Zielen zu kapseln, um eine saubere und konsistente Entwicklungsumgebung zu gewährleisten. Der Fokus liegt darauf, menschliche Fehler zu eliminieren und sicherzustellen, dass die Software jederzeit reproduzierbar gebaut werden kann.

## Kernaussagen
* "Ein Projekt, das nicht mit einem einzigen Klick gebaut werden kann, ist kein professionelles Projekt, sondern ein Chaos."
* "Makefile dient als universeller Wrapper, der die spezifischen Tools der jeweiligen Programmiersprache vor dem Benutzer verbirgt."
* "Automatisierung bedeutet, dass ein 'Roboter' (CI) den Build ohne menschliche Hilfe durchführen kann."
* "Der Build-Prozess ist der wichtigste Wächter der Qualität; er muss sofort abbrechen, wenn eine Regel verletzt wird."

## Relevanz: 5/5
Äußerst relevant für Software-Architekten und DevOps-Ingenieure, die Wert auf reproduzierbare Umgebungen und automatisierte Qualitätskontrolle legen.
