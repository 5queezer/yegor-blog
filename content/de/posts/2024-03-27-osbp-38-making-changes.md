---
title: "OSBP 3/8: Änderungen vornehmen"
date: 2024-03-27T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/D6CUW9eZ5yk/maxresdefault.jpg"
  alt: "OSBP 3/8: Änderungen vornehmen"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=D6CUW9eZ5yk](https://www.youtube.com/watch?v=D6CUW9eZ5yk)

## Zusammenfassung
In diesem achten Teil der Serie „Open Source Best Practices“ erläutert Yegor Bugayenko die Kunst, Code-Änderungen effektiv in Softwareprojekte einzubringen. Er verwendet die kraftvolle Metapher einer geschäftlichen Transaktion: Der Entwickler ist der Verkäufer, der Maintainer der Kunde und der Pull Request (PR) das angebotene Produkt. Um erfolgreich zu „verkaufen“, muss der Entwickler den Review-Prozess für den Maintainer so reibungslos wie möglich gestalten. Die wichtigste Regel hierbei ist die radikale Verkleinerung der PRs. Bugayenko betont, dass kleine Änderungen – oft nur eine einzige Zeile – deutlich schneller akzeptiert werden als umfangreiche Updates. Große PRs mit Hunderten von Zeilen wirken abschreckend, überfordern die Prüfer kognitiv und führen dazu, dass diese oft wochenlang aufgeschoben werden, da das Risiko unentdeckter Fehler zu hoch erscheint.

Ein weiterer zentraler Punkt ist die Atomarität: Ein PR sollte genau ein isoliertes Problem lösen. Werden verschiedene Fehlerbehebungen in einem einzigen PR gemergt, riskiert man, dass die gesamte Arbeit blockiert wird, falls der Maintainer mit auch nur einem kleinen Teil nicht einverstanden ist. Bugayenko fordert die Entwickler zudem auf, die „Führungsrolle“ für ihren eigenen PR zu übernehmen. Das bedeutet, dass der Autor allein dafür verantwortlich ist, dass der PR erfolgreich gemergt wird. Dazu gehört das proaktive Reagieren auf Feedback, das Einhalten von Styleguides ohne unnötige Diskussionen und das beharrliche, aber höfliche Nachfassen bei Verzögerungen. In der Dokumentation des PRs sollte stets das „Warum“ (die Motivation und das gelöste Problem) im Vordergrund stehen, da das „Was“ bereits aus dem Code ersichtlich sein sollte. Zur Untermauerung seiner Thesen zitiert er wissenschaftliche Studien von Forschern wie Bram Adams, Caitlin Sadowski und Marco Ortu, die belegen, dass die Größe eines PRs und die emotionale Tonalität der Kommentare entscheidende Faktoren für die Geschwindigkeit der Integration und die Zufriedenheit im Team sind.

## Kernaussagen
- „Ein Pull Request ist eine Transaktion. Sie sind der Verkäufer, der Maintainer ist der Kunde.“
- „Kleine PRs werden viel schneller gemergt. Sogar ein PR mit nur einer Zeile ist völlig akzeptabel.“
- „Sie sind der Chef Ihres Pull Requests. Es liegt an Ihnen, ihn bis zum Merge zu führen.“
- „Erklären Sie das 'Warum', nicht das 'Was'. Der Code selbst zeigt, was geändert wurde.“

## Relevanz: 5/5
Grundlegende Prinzipien für die Arbeit in modernen, agilen Teams, die auf Micro-Commits und kontinuierliche Integration setzen.
