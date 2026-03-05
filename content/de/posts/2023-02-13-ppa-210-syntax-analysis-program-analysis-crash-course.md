---
title: "PPA 2/10: Syntaxanalyse [Absturzkurs Programmanalyse]"
date: 2023-02-13T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/RTsrFG7NdvY/maxresdefault.jpg"
  alt: "PPA 2/10: Syntaxanalyse [Absturzkurs Programmanalyse]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=RTsrFG7NdvY](https://www.youtube.com/watch?v=RTsrFG7NdvY)

## Zusammenfassung
In der zweiten Vorlesung seiner Reihe „Practical Program Analysis“ widmet sich Yegor Bugayenko der Syntaxanalyse. Er erläutert den entscheidenden Prozess, bei dem unstrukturierter Quelltext in eine hierarchische Form überführt wird, die ein Computer verarbeiten kann. Der Vortrag unterteilt diesen Prozess in zwei Hauptschritte: die lexikalische Analyse (Lexing) und die syntaktische Analyse (Parsing). Beim Lexing werden Zeichenfolgen mithilfe endlicher Automaten in bedeutungsvolle Einheiten, sogenannte Tokens oder Terminalsymbole, gruppiert.

Der Schwerpunkt liegt auf dem Parsing-Prozess, bei dem diese Tokens anhand einer formalen Grammatik in einem Syntaxbaum angeordnet werden. Bugayenko erklärt die Backus-Naur-Form (BNF) und die erweiterte Backus-Naur-Form (EBNF) als Standardwerkzeuge zur Beschreibung der Regeln einer Programmiersprache. Dabei unterscheidet er klar zwischen Terminalen (den eigentlichen Symbolen) und Nicht-Terminalen (abstrakten Strukturen wie „Anweisung“ oder „Ausdruck“).

Ein weiterer wichtiger Teil der Vorlesung befasst sich mit den Werkzeugen der Branche. Während klassische Tools wie Lex/Flex und Yacc/Bison erwähnt werden, liegt ein Fokus auf moderneren Lösungen wie ANTLR, die heute weit verbreitet sind. Abschließend thematisiert Bugayenko die Fehlerbehandlung: Ein robuster Parser muss in der Lage sein, bei fehlerhaftem Code („Müll“) nicht abzubrechen, sondern sich zu erholen und die Analyse fortzusetzen. Die zentrale Lehre ist, dass die Syntaxanalyse rein strukturell ist; sie prüft nur, ob der Code grammatikalisch korrekt ist, nicht ob er logisch sinnvoll ist.

## Kernaussagen
- „Syntaxanalyse ist die Brücke zwischen Rohtext und Semantik, befasst sich aber ausschließlich mit der Struktur, nicht mit dem Sinn.“
- „Ein Lexer erkennt die ‚Wörter‘ der Sprache, aber erst der Parser versteht die ‚Sätze‘.“
- „Die Qualität eines Parsers zeigt sich darin, wie gut er mit Fehlern umgeht und trotzdem weiterarbeitet.“
- „Die BNF ist die mathematische Sprache, mit der wir die Grammatik unserer digitalen Welten definieren.“

## Relevanz: 4/5
Äußerst relevant für Entwickler, die eigene Sprachen, DSLs oder statische Analysetools entwickeln möchten, da sie das grundlegende Verständnis für die Verarbeitung von Programmcode vermittelt.
