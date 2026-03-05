---
title: "SQM 24/24: Neuronale Metriken [Software-Qualitäts-Crashkurs]"
date: 2024-04-29T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/6Rog8QhuXTY/maxresdefault.jpg"
  alt: "SQM 24/24: Neuronale Metriken [Software-Qualitäts-Crashkurs]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=6Rog8QhuXTY](https://www.youtube.com/watch?v=6Rog8QhuXTY)

## Zusammenfassung
In dieser abschließenden Vorlesung des Kurses "Software Quality Metrics" (SQM) thematisiert Yegor Bugayenko den Paradigmenwechsel von regelbasierten Metriken hin zu neuronalen Metriken. Während klassische Ansätze wie Cyclomatic Complexity auf festen mathematischen Regeln basieren, nutzen neuronale Metriken Machine Learning (ML) und Large Language Models (LLM), um Muster in großen Codebasen zu erkennen.

Der Vortrag behandelt Konzepte wie "DeepBugs", das Fehler durch semantische Anomalien (z. B. unpassende Variablennamen) identifiziert, und "code2vec", das Programmcode in Vektoren übersetzt, um Funktionalitäten vorherzusagen. Bugayenko erläutert, dass neuronale Netze in der Lage sind, "semantische Klone" zu finden — Codefragmente, die unterschiedlich geschrieben sind, aber dieselbe Logik ausführen. Ein weiterer Schwerpunkt ist der Einsatz von LLMs in der statischen Analyse, insbesondere um die hohe Rate an "False Positives" (Fehlalarmen) traditioneller Tools zu reduzieren. Trotz ihrer Mächtigkeit warnt er davor, dass neuronale Metriken oft als "Black Boxes" fungieren, deren Entscheidungen schwerer nachvollziehbar sind als die herkömmlicher Metriken.

## Kernaussagen
- **Semantisches Verständnis:** Im Gegensatz zu Regex-basierten Tools können neuronale Metriken verstehen, dass unterschiedliche Bezeichner (z. B. `user_age` vs. `customer_years`) denselben Kontext haben.
- **Das Problem der "Ground Truth":** Die Qualität neuronaler Modelle steht und fällt mit den Trainingsdaten; minderwertiger Code führt zu Modellen, die schlechte Praktiken akzeptieren.
- **LLMs als Filter:** Die aktuelle Stärke von KI liegt darin, die "Geräuschkulisse" statischer Analyse-Tools zu filtern und Entwicklern nur die relevantesten Warnungen zu zeigen.
- **Black-Box-Problematik:** Die Herausforderung für künftige Ingenieure besteht darin, die Präzision von KI mit der Interpretierbarkeit klassischer Metriken zu vereinen.

## Relevanz: 5/5
Essentiell für Entwickler und Manager, die verstehen wollen, wie KI die automatisierte Code-Analyse und Qualitätssicherung grundlegend verändert.
