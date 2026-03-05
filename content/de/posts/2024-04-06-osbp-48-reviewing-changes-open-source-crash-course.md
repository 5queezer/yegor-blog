---
title: "OSBP 4/8: Änderungen prüfen [Open-Source-Crashkurs]"
date: 2024-04-06T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/TJ83ePwyH_A/maxresdefault.jpg"
  alt: "OSBP 4/8: Änderungen prüfen [Open-Source-Crashkurs]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=TJ83ePwyH_A](https://www.youtube.com/watch?v=TJ83ePwyH_A)

## Zusammenfassung
In diesem vierten Teil des "Open Source Best Practices"-Kurses definiert Yegor Bugayenko die Rolle des Code-Reviewers neu: Er ist kein Gehilfe, sondern ein "Torwächter" und "Gegner" des Autors. Die Kernphilosophie besagt, dass Code-Reviews streng und kompromisslos sein müssen, um die langfristige architektonische Integrität zu wahren. Ein Reviewer sollte aktiv nach Gründen suchen, einen Pull Request (PR) abzulehnen, um das Repository vor "Code-Fäule" zu schützen.

Yegor stellt mehrere praktische Regeln auf: Erstens sollte ein Reviewer den Code niemals lokal ausführen. Die funktionale Korrektheit muss durch automatisierte Tests und CI gewährleistet sein; wenn ein Reviewer den Code manuell testen muss, sind die Tests unzureichend. Zweitens sollten große PRs (mit Dutzenden von Dateien) sofort abgelehnt werden, da sie nicht effektiv geprüft werden können. Änderungen müssen atomar und klein sein. Drittens ist ein Bugfix ungültig, wenn er nicht ein "Rätsel" (einen Testfall) enthält, der ohne den Fix fehlschlägt und mit ihm erfolgreich ist. Dies stellt sicher, dass der Fehler wirklich verstanden und dauerhaft behoben wurde.

Schließlich betont Yegor den pädagogischen Wert von Reviews. Ein Reviewer sollte Probleme aufzeigen, sie aber niemals selbst lösen. Durch die Erläuterung der zugrunde liegenden Prinzipien und Standards fungiert der Reviewer als Mentor für den Mitwirkenden. Dies schafft eine Kultur hoher Standards, in der Qualität niemals zugunsten der Geschwindigkeit geopfert wird.

## Kernaussagen
*   **Der Reviewer als Gegner:** Die Hauptaufgabe des Reviewers besteht darin, Fehler zu finden und den Code abzulehnen, um als Filter für die Gesundheit des Projekts zu dienen.
*   **Vertrauen in CI, nicht in lokale Tests:** Die Zeit des Menschen ist zu wertvoll für manuelle Tests; die funktionale Verifizierung gehört in die automatisierte Pipeline.
*   **Keine großen Pull Requests:** Nur kleine, atomare Änderungen ermöglichen eine tiefgehende Code-Analyse und verhindern oberflächliche Abnahmen.
*   **Die "Puzzle"-Anforderung:** Jeder Bugfix muss von einem fehlschlagenden Testfall begleitet werden, um die Wirksamkeit zu beweisen und Regressionen zu verhindern.

## Relevanz: 5/5
Dieser Inhalt ist für jeden Software-Leiter oder Maintainer von entscheidender Bedeutung. Er stellt die "freundliche", aber oberflächliche Review-Kultur in Frage und bietet ein Konzept für hochwertiges Teammanagement.
