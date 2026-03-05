---
title: "EQSP 15/20: Testen zweiter Ordnung [Software-Qualitäts-Crashkurs]"
date: 2023-03-13T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
  - "testing"
cover:
  image: "https://img.youtube.com/vi/O6cl3X8gOzs/maxresdefault.jpg"
  alt: "EQSP 15/20: Testen zweiter Ordnung [Software-Qualitäts-Crashkurs]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=O6cl3X8gOzs](https://www.youtube.com/watch?v=O6cl3X8gOzs)

## Zusammenfassung
In dieser Vorlesung führt Yegor Bugayenko das Konzept des „Testens zweiter Ordnung“ ein. Während herkömmliche Tests (erster Ordnung) prüfen, ob die Geschäftslogik korrekt funktioniert, zielt die zweite Ordnung darauf ab, die Qualität und Wirksamkeit dieser Tests selbst zu überprüfen. Bugayenko argumentiert, dass man Tests nicht blind vertrauen darf, da sie unvollständig sein oder falsche Sicherheit bieten können.

Ein zentrales Element ist die strikte „Coverage Control“ (Abdeckungskontrolle). Laut Bugayenko sollte die Testabdeckung ein blockierendes Kriterium in der Build-Pipeline sein: Sinkt die Abdeckung auch nur um 0,1 %, muss der Build fehlschlagen. Dies erzwingt Disziplin und verhindert das Entstehen von ungetestetem Code. Noch wichtiger ist jedoch das „Mutation Testing“. Hierbei verändern Werkzeuge wie PITest den Quellcode minimal (z. B. wird ein „>“ zu einem „<“). Wenn die Tests trotz dieser Fehler bestehen, sind sie mangelhaft. Ein guter Test muss in der Lage sein, solche „Mutanten“ zu finden und zu eliminieren.

Des Weiteren bespricht die Vorlesung „Strukturtests“, die mit Tools wie ArchUnit architektonische Regeln erzwingen (z. B. dass alle Klassen `final` sein müssen). Auch „Property-based Testing“, also das Testen mit zufälligen Eingabewerten, wird als Methode zur Entdeckung von Grenzfällen genannt. Abschließend betont Bugayenko die Testhygiene: Tests müssen vollkommen isoliert sein und dürfen niemals von externen Ressourcen wie dem Internet abhängen. Das Ziel ist es, die Qualitätssicherung von einer subjektiven Einschätzung in einen harten, automatisierten und mathematisch belegbaren Prozess zu verwandeln.

## Kernaussagen
1. „Testen zweiter Ordnung beantwortet die Frage: 'Wie gut sind unsere Tests eigentlich?'“
2. „Mutationstests sind der einzige Weg, die Nützlichkeit von Tests mathematisch zu beweisen.“
3. „Der Build muss abbrechen, wenn die Code-Abdeckung um 0,1 % sinkt; Abdeckung ist eine Einbahnstraße nach oben.“
4. „Ein Test, der vom Internet abhängt, ist kein Test, sondern eine Lotterie, die das Vertrauen in die CI zerstört.“

## Relevanz: 5/5
Äußerst relevant für Software-Architekten und Teamleiter. Die vorgestellten Methoden bieten einen klaren Weg, um die Testqualität objektiv messbar zu machen und die technische Schuld systematisch zu reduzieren.
