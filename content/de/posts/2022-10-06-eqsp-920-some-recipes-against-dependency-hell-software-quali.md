---
title: "EQSP 9/20: Einige Rezepte gegen die Abhängigkeitshölle"
date: 2022-10-06T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
  - "ai"
cover:
  image: "https://img.youtube.com/vi/_NU0IYv8ZJo/maxresdefault.jpg"
  alt: "EQSP 9/20: Einige Rezepte gegen die Abhängigkeitshölle"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=_NU0IYv8ZJo](https://www.youtube.com/watch?v=_NU0IYv8ZJo)

## Zusammenfassung
In diesem Vortrag befasst sich Yegor Bugayenko mit der berüchtigten „Abhängigkeitshölle“ (Dependency Hell), einem Zustand, in dem widersprüchliche Anforderungen an gemeinsam genutzte Bibliotheken ein System instabil oder unbaubar machen. Er argumentiert, dass die Hauptursache oft ein falsches Vertrauen in die Einhaltung von Semantic Versioning (SemVer) durch Drittanbieter ist. Bugayenko unterteilt Abhängigkeiten in zwei Gruppen: solche, denen wir vertrauen (wo dynamische Bereiche wie `^` oder `~` akzeptabel sind), und solche, denen wir misstrauen (wo Versionen strikt fixiert werden müssen).

Ein zentrales Thema ist das „Fail Fast“-Prinzip. Er empfiehlt Build-Tools wie das Maven Enforcer Plugin, um Versionskonflikte frühzeitig zu erkennen. Anstatt dem Paketmanager die stille Lösung eines Konflikts zu überlassen, sollte der Build abbrechen und den Entwickler zwingen, die korrekte Version explizit festzulegen. Darüber hinaus betont er, dass jede neue Abhängigkeit ein Risiko darstellt, das die Angriffsfläche und Komplexität erhöht. Entwickler sollten Abhängigkeitsbäume prüfen (z. B. mit `npm list`), bevor sie neue Bibliotheken integrieren. Schließlich plädiert Bugayenko für automatisierte Release-Pipelines, bei denen jedes Artefakt auf einen Git-Tag rückführbar ist, um Reproduzierbarkeit zu gewährleisten. Dieser disziplinierte Ansatz macht das Abhängigkeitsmanagement von einer Chaosquelle zu einer kontrollierten architektonischen Entscheidung.

## Kernaussagen
- „Betrachten Sie jede neue Abhängigkeit als potenzielle Belastung.“
- „Der Build sollte sofort fehlschlagen, anstatt nicht-deterministisches Verhalten zuzulassen.“
- „Ihre Versionierungsstrategie sollte durch Ihr Vertrauen in die Entwickler der Abhängigkeit bestimmt werden.“
- Lösen Sie transitive Konflikte explizit auf, anstatt das Build-Tool „raten“ zu lassen.

## Relevanz: 5/5
Äußerst relevant für Software-Architekten und DevOps-Ingenieure, die stabile und wartbare Build-Prozesse sicherstellen müssen.
