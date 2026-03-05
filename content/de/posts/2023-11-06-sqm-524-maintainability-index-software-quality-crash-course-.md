---
title: "SQM 5/24: Wartbarkeitsindex"
date: 2023-11-06T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
  - "ai"
cover:
  image: "https://img.youtube.com/vi/xnSnPfVkmkM/maxresdefault.jpg"
  alt: "SQM 5/24: Wartbarkeitsindex"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=xnSnPfVkmkM](https://www.youtube.com/watch?v=xnSnPfVkmkM)

## Zusammenfassung
In dieser Vorlesung aus der Reihe Software Quality Management (SQM) befasst sich Yegor Bugayenko mit dem **Maintainability Index (MI)**, einer Kennzahl, die messen soll, wie einfach ein Softwaresystem zu warten und zu erweitern ist. Die Sitzung beginnt mit einem Rückgriff auf Fred Brooks (essenzielle vs. akzidentelle Komplexität) und Ward Cunninghams Konzept der technischen Schulden. Bugayenko erläutert, dass der MI Anfang der 1990er Jahre von Paul Oman und Jack Hagemeister entwickelt wurde, um die Softwarebewertung von subjektiven Eindrücken auf objektive Daten umzustellen.

Die ursprüngliche MI-Formel basiert auf drei Hauptvariablen: dem **Halstead-Volumen** (Informationsgehalt), der **zyklomatischen Komplexität nach McCabe** (Logikpfade) und der Anzahl der **Codezeilen (LOC)**. Gelegentlich wird auch die Kommentardichte einbezogen. Bugayenko zeigt auf, wie Microsoft eine normalisierte Version dieses Index (0 bis 100) in Visual Studio populär gemacht hat. Der Vortrag übt jedoch auch Kritik und zitiert Forscher wie Arie van Deursen, die den MI als potenziell „schädlich“ bezeichnen. Da die Metrik stark von der Zeilenanzahl abhängt, kann sie leicht manipuliert werden (z. B. durch das Löschen von Kommentaren), um die Werte künstlich zu verbessern, ohne die tatsächliche Wartbarkeit zu erhöhen. Bugayenko empfiehlt daher, den MI lediglich als „Smoke-Test“ zu verwenden: Er kann signalisieren, dass etwas nicht stimmt, sollte aber nicht das einzige Kriterium für die Bewertung der Codequalität sein.

## Kernaussagen
*   „Der Wartbarkeitsindex versucht, das menschliche Empfinden von 'unordentlichem Code' in eine einzige, objektive mathematische Zahl zu fassen.“
*   „Da der MI so stark von den Codezeilen abhängt, ist es einfach, die Metrik zu 'überlisten', ohne die Software tatsächlich zu verbessern.“
*   „Nutzen Sie den Wartbarkeitsindex als 'Smoke-Test' – er zeigt Ihnen, dass es brennt, aber er garantiert nicht, dass das Haus perfekt gebaut ist.“

## Relevanz: 4/5
Die Vorlesung ist für Teamleiter und Architekten von großer Bedeutung, da sie zeigt, wie man technische Schulden quantifiziert, ohne dabei den Blick für die Grenzen automatisierter Metriken zu verlieren.
