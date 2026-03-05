---
title: "PPA 10/10: Codeanalyse mit maschinellem Lernen [Crashkurs Programmanalyse]"
date: 2023-05-19T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/6Z1EFTJ7Kdo/maxresdefault.jpg"
  alt: "PPA 10/10: Codeanalyse mit maschinellem Lernen [Crashkurs Programmanalyse]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=6Z1EFTJ7Kdo](https://www.youtube.com/watch?v=6Z1EFTJ7Kdo)

## Zusammenfassung
In der zehnten und letzten Lektion seines Kurses widmet sich Yegor Bugayenko der Integration von Machine Learning (ML) in die Welt der Programmanalyse, oft als „Big Code“ bezeichnet. Er stellt die These auf, dass herkömmliche statische Analysewerkzeuge durch die begrenzte Kapazität menschlicher Experten, Regeln zu formulieren, limitiert sind. Im Gegensatz dazu nutzt ML die riesigen Mengen an verfügbarem Quellcode (z. B. von GitHub), um statistische Muster zu erkennen, die auf Fehler oder schlechten Stil hinweisen. Da Programmcode von Menschen geschrieben wird, weist er ähnliche Redundanzen und Strukturen wie natürliche Sprache auf, was ihn für stochastische Modelle zugänglich macht.

Bugayenko erläutert die technischen Hürden bei der Vektorisierung von Code. Er erklärt, warum eine einfache Textanalyse nicht ausreicht und wie strukturelle Informationen aus dem Abstract Syntax Tree (AST) genutzt werden, um „Code-Embeddings“ (wie bei Code2Vec) zu erstellen. Diese ermöglichen es Computern, die Semantik von Funktionen und Klassen mathematisch zu vergleichen. Zu den Anwendungen gehören die automatische Fehlererkennung, die Benennung von Variablen und die Vervollständigung von Code. Kritisch betrachtet Bugayenko jedoch die „Black Box“-Problematik: Während ein klassischer Compiler oder Linter eine logische Begründung für einen Fehler liefert, bietet ML oft nur Wahrscheinlichkeiten. Für professionelle Softwareentwickler ist diese mangelnde Erklärbarkeit oft ein Hindernis, da sie eine präzise Anleitung zur Fehlerbehebung benötigen.

## Kernaussagen
- „Programmcode ist hochgradig repetitiv und besitzt eine 'Natürlichkeit', die es erlaubt, ihn mit Methoden der Computerlinguistik zu analysieren.“
- „Der Übergang von Expertenregeln zu gelernten Mustern markiert den Wechsel von der Heuristik zur Wahrscheinlichkeit in der Softwarequalitätssicherung.“
- „Das größte Problem für ML in der Programmanalyse ist die Interpretierbarkeit; eine Fehlermeldung ohne Begründung ist für einen Ingenieur wertlos.“
- „Technologien wie Code2Vec verwandeln die Struktur von Programmen in mathematische Räume, wodurch semantische Ähnlichkeiten messbar werden.“

## Relevanz: 5/5
Die Vorlesung ist essenziell für das Verständnis der Funktionsweise moderner KI-Assistenten (wie Copilot) und zeigt die Grenzen zwischen formaler Logik und statistischer Annäherung im Software-Engineering auf.
