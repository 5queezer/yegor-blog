---
title: "SQM 6/24: Kopplung [Software-Qualitäts-Crashkurs]"
date: 2023-11-02T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/G0vN6Ah8-js/maxresdefault.jpg"
  alt: "SQM 6/24: Kopplung [Software-Qualitäts-Crashkurs]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=G0vN6Ah8-js](https://www.youtube.com/watch?v=G0vN6Ah8-js)

## Zusammenfassung
In diesem Video analysiert Yegor Bugayenko die Kopplung (Coupling) als eine der kritischsten Metriken für die Softwarequalität. Kopplung beschreibt den Grad der gegenseitigen Abhängigkeit zwischen Modulen. Yegor betont, dass eine hohe Kopplung zwangsläufig zu technischer Schuld führt, da Änderungen an einem Modul oft unvorhersehbare Auswirkungen auf andere Teile des Systems haben. 

Die Vorlesung behandelt wichtige Metriken wie CBO (Coupling Between Objects) und DCC (Direct Class Coupling). Ein besonderer Fokus liegt auf der „Distanz der Kopplung“ – je mehr Zwischenschritte ein Objekt durchlaufen muss, desto instabiler wird das Design. Yegor warnt zudem vor zeitlicher Kopplung (Temporal Coupling), bei der Methoden in einer bestimmten Reihenfolge aufgerufen werden müssen, und vor versteckter Kopplung durch Reflexion oder globale Zustände. Er räumt mit dem Vorurteil auf, dass starke Entkopplung den Code unübersichtlich mache („Lasagna Code“), und argumentiert stattdessen, dass eine geringe Kopplung die einzige Möglichkeit sei, langfristige Testbarkeit und Wartbarkeit zu garantieren.

## Kernaussagen
- „Kopplung ist der größte Feind des Wandels in der Softwareentwicklung.“
- „Ein stabiles Modul zeichnet sich dadurch aus, dass es wenig über seine Umgebung wissen muss.“
- „Zeitliche Kopplung sollte durch Unveränderlichkeit (Immutability) oder besseres Information Hiding vermieden werden.“
- „Die Metrik CBO hilft dabei, Klassen zu identifizieren, die zu komplex und zu zerbrechlich für eine einfache Wiederverwendung sind.“

## Relevanz: 5/5
Kopplung ist ein zentrales Thema der Informatik; das Verständnis dieser Metrik ist entscheidend für sauberes OOP-Design.
