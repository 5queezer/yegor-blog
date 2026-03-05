---
title: "SQM 12/24: Toter Code [Crashkurs für Softwarequalität] [engl. Untertitel]"
date: 2023-12-17T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/zN0gX9m6a2k/maxresdefault.jpg"
  alt: "SQM 12/24: Toter Code [Crashkurs für Softwarequalität] [engl. Untertitel]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=zN0gX9m6a2k](https://www.youtube.com/watch?v=zN0gX9m6a2k)

## Zusammenfassung
In seiner Vorlesung „SQM 12/24: Dead Code“, einem Teil des Crashkurses für Softwarequalitätsmetriken, befasst sich Yegor Bugayenko mit dem allgegenwärtigen Problem des toten Codes und dessen schädlichen Auswirkungen auf die Wartbarkeit von Software. Toter Code – also Code, der nie ausgeführt wird oder dessen Ergebnisse ungenutzt bleiben – wird als schwerwiegender „Bad Smell“ eingestuft. Bugayenko betont, dass das Vorhandensein solchen Codes die kognitive Belastung für Entwickler künstlich in die Höhe treibt, Refactoring-Prozesse erheblich erschwert und die sogenannte „Bit-Fäule“ (Bit Rot) beschleunigt. Er erläutert, wie Werkzeuge zur statischen Analyse und moderne Compiler die Eliminierung von totem Code (DCE) handhaben, argumentiert jedoch, dass Entwickler ihre Codebasis aktiv bereinigen müssen und sich nicht allein auf automatisierte Tools verlassen dürfen.

Ein wesentlicher Teil der Vorlesung widmet sich der Repository-Architektur und vergleicht monolithische Repositories (Monorepos) mit Polyrepos („Manyrepos“). Obwohl er anerkennt, dass Technologiegiganten wie Google und Facebook Monorepos erfolgreich einsetzen, um den Integrationsaufwand zu verringern, übt Bugayenko starke Kritik an diesem Ansatz. Er argumentiert, dass Monorepos unweigerlich zu kompromittierter Codequalität, verschwimmenden Grenzen und schlechter Kapselung führen. Stattdessen plädiert er nachdrücklich für die Manyrepo-Strategie. Durch die Aufteilung von Projekten in kleinere, entkoppelte Repositories können Teams schnellere, unabhängige Builds erreichen, eine strengere Kapselung durchsetzen, sauberere Metriken pflegen und die Test-Pipeline vereinfachen. Zudem führt er das Konzept der Code-„Volatilität“ ein – die Messung, wie häufig sich Dateien ändern –, um stagnierende Bereiche zu identifizieren, in denen sich möglicherweise toter Code verbirgt.

## Kernaussagen
- „Toter Code ist nicht einfach nur harmloser Text; er ist eine Belastung, die die kognitive Last aktiv erhöht und zukünftiges Refactoring ausbremst.“
- „Während Monorepos vielleicht Integrationsprobleme lösen, tun sie dies oft auf Kosten von Kapselung und grundlegender Codequalität.“
- „Code, der sich nicht ändert, ist Code, der verrottet. Hohe Volatilität ist ein Zeichen von Leben, während stagnierender Code oft tote oder irrelevante Logik verbirgt.“
- „Verlassen Sie sich nicht ausschließlich auf die Dead-Code-Eliminierung des Compilers; die Codebasis rigoros sauber zu halten, liegt in der direkten Verantwortung des Entwicklers.“

## Relevanz: 5/5
Diese Vorlesung ist für Softwareentwicklung und Teammanagement von höchster Relevanz. Sie behandelt direkte tägliche Herausforderungen der Code-Wartung, des Refactorings und grundlegender architektonischer Entscheidungen (Monorepo vs. Manyrepo), die die langfristige Geschwindigkeit eines Teams bestimmen.
