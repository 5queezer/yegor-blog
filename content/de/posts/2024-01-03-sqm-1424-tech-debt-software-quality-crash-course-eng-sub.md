---
title: "SQM 14/24: Technische Schulden [Software-Qualitäts-Crashkurs]"
date: 2024-01-03T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/pvZDcytPU3w/maxresdefault.jpg"
  alt: "SQM 14/24: Technische Schulden [Software-Qualitäts-Crashkurs]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=pvZDcytPU3w](https://www.youtube.com/watch?v=pvZDcytPU3w)

## Zusammenfassung
In dieser Vorlesung seines Kurses für Software-Qualitätsmanagement (SQM) präsentiert Yegor Bugayenko eine disziplinierte und architektonische Sicht auf das Thema „Technische Schulden“. Der Kern seiner Argumentation ist die strikte Unterscheidung zwischen „Technischen Schulden“ und „Technischem Chaos“ (Mess). Schulden sind laut Yegor eine strategische, bewusste Entscheidung, Qualitätsstandards vorübergehend zu umgehen, um einen geschäftlichen Meilenstein zu erreichen – vorausgesetzt, dieser Kompromiss wird formal in einem Aufgabenmanagementsystem dokumentiert. Im Gegensatz dazu ist „Chaos“ einfach minderwertiger Code, der durch Nachlässigkeit entsteht und unsichtbar bleibt.

Yegor stützt sich auf die Metapher von Ward Cunningham und erklärt, dass technische Schulden wie ein Finanzkredit funktionieren. Sie ermöglichen es einem Team, Zeit in der Gegenwart zu „kaufen“, gehen aber mit obligatorischen „Zinszahlungen“ einher. Diese Zinsen äußern sich in dem erhöhten Aufwand, der für jede nachfolgende Funktion erforderlich ist, da die Codebasis durch die suboptimalen Lösungen komplexer geworden ist. Er warnt davor, dass die Zinsen irgendwann die Kapazität des Teams zur Wertschöpfung übersteigen können, was zum „technischen Bankrott“ führt, wenn die Schulden nicht durch Refactoring getilgt werden.

Um dies zu bewältigen, plädiert Yegor für das „Puzzle Driven Development“ (PDD). Er argumentiert, dass herkömmliche `// TODO`-Kommentare wirkungslos sind, da sie passiv sind und oft ignoriert werden. PDD verlangt von Entwicklern, strukturierte „Puzzles“ im Code zu hinterlassen, die automatisch in verfolgbare GitHub-Issues umgewandelt werden. Dadurch wird sichergestellt, dass die Schulden für das Management sichtbar sind und priorisiert werden können. Letztlich betont die Vorlesung, dass das Schuldenmanagement eine Verantwortung auf Prozessebene ist, bei der der Architekt entscheidet, welche „Kredite“ sinnvoll sind.

## Kernaussagen
1. „Wenn es nicht im Task-Tracker steht, sind es keine technischen Schulden, sondern einfach nur technisches Chaos.“
2. „Technische Schulden sind ein bewusster Kompromiss, bei dem man sich Produktivität von der Zukunft leiht, um heute Geschwindigkeit zu gewinnen.“
3. „Die Zinsen für technische Schulden sind eine Steuer, die man auf jede einzelne neue Zeile Code zahlt, die man in einem überladenen System schreibt.“
4. „PDD verwandelt die passive Hoffnung auf Refactoring in eine aktive, verfolgbare und verwaltbare Aufgabe.“

## Relevanz: 5/5
Yegors Ansatz ist hochrelevant für Teamleiter und Architekten, die den geschäftlichen Druck mit der langfristigen Wartbarkeit in Einklang bringen müssen.
