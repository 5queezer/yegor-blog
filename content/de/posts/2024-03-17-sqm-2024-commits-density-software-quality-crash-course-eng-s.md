---
title: "SQM 20/24: Commit-Dichte"
date: 2024-03-17T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/BrG3HiuYC5U/maxresdefault.jpg"
  alt: "SQM 20/24: Commit-Dichte"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=BrG3HiuYC5U](https://www.youtube.com/watch?v=BrG3HiuYC5U)

## Zusammenfassung
In dieser Vorlesung aus dem Kurs "Software Quality Metrics" (SQM) untersucht Yegor Bugayenko das Konzept der "Commit-Dichte" als eine entscheidende Metrik zur Bewertung der Disziplin in der Softwareentwicklung. Er definiert diese Metrik auf zwei Arten: zeitliche Dichte (Commits pro Tag) und strukturelle Dichte (Commits pro tausend geänderter Codezeilen). Bugayenko argumentiert, dass eine höhere Commit-Dichte direkt mit einer höheren Softwarequalität korreliert.

Anstatt massive, umfassende Änderungen ("Big Bang") vorzunehmen, sollten Entwickler ihre Arbeit in kleine, häufige Commits aufteilen. Dieser Ansatz bietet mehrere große Vorteile. Erstens verbessert er die Rückverfolgbarkeit erheblich, was es mit Werkzeugen wie `git bisect` viel einfacher macht, genau festzustellen, wann und warum ein Fehler eingeführt wurde. Zweitens sind kleinere Änderungen für Kollegen viel einfacher und gründlicher zu überprüfen. Große Commits bündeln oft unzusammenhängende Änderungen, überfordern die Prüfer und machen ein Rollback nahezu unmöglich. Bugayenko betont, dass häufige Commits die Grundlage für eine effektive kontinuierliche Integration (CI) sind, da sie die Stabilität der Codebasis gewährleisten und Merge-Konflikte minimieren.

## Kernaussagen
- "Eine höhere Commit-Dichte ist ein direkter Indikator für starke technische Disziplin und führt zu höherer Codequalität."
- "Kleine, häufige Commits machen Peer-Reviews sinnvoll und verhindern das Übersehen versteckter Fehler."
- "Massive 'Big-Bang'-Commits sind riskant; sie bündeln unzusammenhängende Änderungen und machen ein Rollback unmöglich."
- "Häufige Integration reduziert Merge-Konflikte und hält das Projekt in einem ständigen Zustand der Einsatzbereitschaft."

## Relevanz: 5/5
Äußerst relevant für Software Engineering und Teammanagement. Es unterstreicht die praktische Versionskontroll-Disziplin, die sich direkt auf die Qualität von Code-Reviews, die Wirksamkeit von CI/CD und die Wartbarkeit des gesamten Projekts auswirkt.
