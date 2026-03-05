---
title: "I16: E. A. Ryschkow | PVS-Studio, Statische Code-Analyse, KI-Analysatoren, Legacy-Code, Open Source"
date: 2024-03-13T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
  - "ai"
cover:
  image: "https://img.youtube.com/vi/hp_hFI1rl9A/maxresdefault.jpg"
  alt: "I16: E. A. Ryschkow | PVS-Studio, Statische Code-Analyse, KI-Analysatoren, Legacy-Code, Open Source"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=hp_hFI1rl9A](https://www.youtube.com/watch?v=hp_hFI1rl9A)

## Zusammenfassung
In diesem aufschlussreichen Interview spricht Yegor Bugayenko mit Jewgeni Ryschkow, dem Mitbegründer und CEO von PVS-Studio, über die Entwicklung, Akzeptanz und praktische Anwendung der statischen Code-Analyse in der modernen Softwareentwicklung. Sie diskutieren detailliert die Kernmechanismen von PVS-Studio und wie es sich in einem wettbewerbsintensiven Markt für Code-Qualitätswerkzeuge abhebt. Ein wesentlicher Schwerpunkt ihres Gesprächs ist der rasante Aufstieg von künstlicher Intelligenz und großen Sprachmodellen in der Programmierung. Ryschkow macht deutlich, dass KI zwar ein hervorragender Assistent für Code-Vervollständigungen, Refactorings oder kleinere Korrekturen ist, traditionelle, deterministische statische Analysatoren jedoch absolut unersetzlich bleiben. Analysatoren bieten die strenge, halluzinationsfreie Zuverlässigkeit, die erforderlich ist, um komplexe, tief verwurzelte Fehler in Unternehmenssoftware zu identifizieren.

Darüber hinaus befassen sie sich mit der bekanntermaßen schwierigen Herausforderung, statische Analysen in riesige, bereits bestehende Legacy-Codebasen zu integrieren. Ryschkow erklärt den äußerst effektiven "Baseline"-Ansatz: Indem Tausende von bestehenden Warnungen unterdrückt werden, um einen sauberen Ausgangspunkt zu schaffen, können Teams eine strikte Null-Warnungs-Richtlinie für alle neuen Commits durchsetzen. Dies verhindert Frustration bei den Entwicklern und verbessert die Codequalität im Laufe der Zeit schrittweise. Schließlich diskutieren sie die brillante und erfolgreiche Marketingstrategie von PVS-Studio, beliebte Open-Source-Projekte zu analysieren, kritische Fehler zu finden und detaillierte Artikel zu veröffentlichen, was der Community zugutekommt und den Wert des Produkts unbestreitbar beweist.

## Kernaussagen
- "Deterministische statische Analyse bietet eine Zuverlässigkeit, die aktuelle KI-Modelle aufgrund von Halluzinationen nicht garantieren können."
- "Um Legacy-Code zu bewältigen, muss man die technischen Schulden einfrieren: Alte Warnungen unterdrücken und strenge Prüfungen nur für neue Commits erzwingen."
- "Das Finden von Fehlern in bekannten Open-Source-Projekten ist der beste und transparenteste Beweis für die Wirksamkeit eines Analysators."
- "Statische Analysatoren sollten fest in die CI/CD-Pipeline integriert werden, anstatt nur lokal von einzelnen Entwicklern ausgeführt zu werden."

## Relevanz: 5/5
Sehr relevant. Das Gespräch liefert praxisnahe Strategien für den Umgang mit technischen Schulden, die Integration von Qualitätskontrollwerkzeugen in CI/CD und das Verständnis der Grenzen zwischen traditionellen Tools und KI-Technologien in der Unternehmenssoftware.
