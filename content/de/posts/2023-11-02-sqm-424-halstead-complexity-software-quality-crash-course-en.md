---
title: "SQM 4/24: Halstead-Komplexität [Software-Qualität Crashkurs]"
date: 2023-11-02T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/YsGzjv0hgcc/maxresdefault.jpg"
  alt: "SQM 4/24: Halstead-Komplexität [Software-Qualität Crashkurs]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=YsGzjv0hgcc](https://www.youtube.com/watch?v=YsGzjv0hgcc)

## Zusammenfassung
In dieser Vorlesung erläutert Yegor Bugayenko die **Halstead-Komplexität**, eine grundlegende Metrik der "Software-Wissenschaft", die 1977 von Maurice Halstead eingeführt wurde. Im Gegensatz zur zyklomatischen Komplexität, die sich auf den Kontrollfluss und Verzweigungen konzentriert, basiert Halsteads Ansatz auf der Zählung der grundlegenden Bausteine des Codes: **Operatoren** (Schlüsselwörter, Symbole, Funktionsaufrufe) und **Operanden** (Variablen, Konstanten).

Die Vorlesung beschreibt die vier Basismetriken: eindeutige Operatoren ($n_1$), eindeutige Operanden ($n_2$), Gesamtzahl der Operatoren ($N_1$) und Gesamtzahl der Operanden ($N_2$). Daraus werden abgeleitete Indikatoren wie **Volumen ($V$)**, **Schwierigkeit ($D$)** und **Aufwand ($E$)** berechnet. Bugayenko betont, dass der **Aufwand ($E = D \times V$)** der wichtigste Aspekt für Softwareentwickler ist, da er versucht, die mentale Energie und Zeit zu quantifizieren, die ein Mensch benötigt, um einen bestimmten Algorithmus zu verstehen oder zu implementieren.

Yegor setzt diese Metriken in den Kontext der Wartbarkeit und der "Kosten von Code". Er argumentiert, dass Halsteads Arbeit, obwohl sie Jahrzehnte alt ist, einen strengen mathematischen Rahmen bietet, um zu verstehen, warum "dichter" Code schwerer zu warten ist. Durch die Messung des Vokabulars und der Dichte eines Programms können Teams Module mit hohem Aufwand identifizieren, die wahrscheinlich zu Engpässen bei der zukünftigen Entwicklung und Fehlersuche werden.

## Kernaussagen
* **Code als Information:** Programmieren geht über Logik hinaus; es geht um Informationsdichte. Halstead-Metriken betrachten Code als einen Strom von Symbolen, die vom menschlichen Gehirn verarbeitet werden müssen.
* **Die Metrik "Aufwand":** Der wertvollste Teil der Halstead-Theorie ist die Quantifizierung des "mentalen Aufwands", der direkt mit der Zeit korreliert, die ein Entwickler für eine Aufgabe benötigt.
* **Volumen vs. Schwierigkeit:** Ein Programm kann ein geringes Volumen, aber eine hohe Schwierigkeit aufweisen, wenn es eine große Vielfalt an Operatoren komplex nutzt, was das Lesen erschwert.
* **Wissenschaftliche Basis:** Halstead versuchte, Software-Engineering in eine "exakte Wissenschaft" zu verwandeln, indem er die Informationstheorie auf den Quellcode anwandte.

## Relevanz: 4/5
Äußerst relevant für das Verständnis der Wartungskosten und des psychologischen Aspekts der Code-Lesbarkeit, insbesondere in komplexen Systemen.
