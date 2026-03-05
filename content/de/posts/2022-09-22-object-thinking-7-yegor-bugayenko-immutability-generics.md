---
title: "Object Thinking #7: Yegor Bugayenko / Unveränderlichkeit + Generics"
date: 2022-09-22T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
  - "oop"
cover:
  image: "https://img.youtube.com/vi/C6CQWzOKEJs/maxresdefault.jpg"
  alt: "Object Thinking #7: Yegor Bugayenko / Unveränderlichkeit + Generics"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=C6CQWzOKEJs](https://www.youtube.com/watch?v=C6CQWzOKEJs)

## Zusammenfassung
In dieser Folge von "Object Thinking" analysiert Yegor Bugayenko die architektonische Gestaltung der Java-Bibliothek **xsline**. Das Hauptthema ist die Anwendung von **Unveränderlichkeit (Immutability)** und **Generics** beim Entwurf von Transformations-Pipelines. Yegor kritisiert den Einsatz von veränderlichem Zustand und prozeduralen Methoden wie `add()`, die ein Objekt in einen "Datenbeutel" verwandeln würden.

Stattdessen stellt er das Konzept von **Shift** (einzelne Transformation) und **Train** (Pipeline) vor. Anstelle der Manipulation bestehender Instanzen verwendet er eine `with()`-Methode, die stets eine neue, unveränderliche Instanz zurückgibt. Dies fördert die Thread-Sicherheit und die Vorhersehbarkeit des Codes. 

Ein besonderer Schwerpunkt liegt auf der Verwendung von **Generics**, um verschiedene Eingabetypen (wie `String`-Dateipfade oder `Shift`-Objekte) in einer flüssigen API (Fluent API) zu verarbeiten. Yegor präsentiert das "Temporary Interface"-Muster: Durch eine `back()`-Methode kann ein Objekt während der Konfiguration seinen generischen Typ ändern (z. B. von `Train<String>` zurück zu `Train<Shift>`), ohne die strikte Kapselung zu verletzen. Das Ziel ist es, den Code deklarativ zu gestalten, sodass er eher wie eine Definition als wie eine Liste von Befehlen wirkt.

## Kernaussagen
- **"Objekte müssen unveränderlich sein, um als eigenständige, zuverlässige Akteure im System zu fungieren."**
- **"Öffentliche Methoden, die nicht Teil eines Interfaces sind, stellen einen Designfehler dar und führen zu 'Leaky Abstractions'."**
- **"Generics ermöglichen es einem Objekt, seinen Typ während einer Konfigurationsphase sicher zu 'entwickeln'."**
- **"Guter Code sollte deklarativ sein und beschreiben, 'was' etwas ist, anstatt 'wie' es Schritt für Schritt aufgebaut wird."**

## Relevanz: 5/5
Äußerst wertvoll für Software-Architekten, die lernen möchten, wie man theoretische OOP-Konzepte nutzt, um robuste und wartbare Java-APIs zu entwickeln, die prozedurale Logik durch elegante Objekt-Strukturen ersetzen.
