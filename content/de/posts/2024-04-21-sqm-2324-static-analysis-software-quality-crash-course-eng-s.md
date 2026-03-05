---
title: "SQM 23/24: Statische Code-Analyse [Software-Qualitätskurs]"
date: 2024-04-21T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/QK2XQvYoEpQ/maxresdefault.jpg"
  alt: "SQM 23/24: Statische Code-Analyse [Software-Qualitätskurs]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=QK2XQvYoEpQ](https://www.youtube.com/watch?v=QK2XQvYoEpQ)

## Zusammenfassung
In dieser Vorlesung erläutert Yegor Bugayenko die statische Analyse als einen der Grundpfeiler des Software-Qualitätsmanagements (SQM). Er definiert sie als die automatisierte Prüfung von Quellcode ohne dessen Ausführung und grenzt sie damit von der dynamischen Analyse (Testing) ab. Der Kurs beleuchtet die Entwicklung der Werkzeuge über drei Generationen: von einfachem Pattern-Matching (1. Gen) über Kontrollflussanalysen (2. Gen) bis hin zu komplexen, projektweiten Logikprüfungen (3. Gen).

Bugayenko unterteilt Code-Probleme in Stilverletzungen, "Code Smells" (Entwurfsfehler) und tatsächliche Bugs. Ein zentrales Thema ist die Problematik von "False Positives" (Fehlalarmen), die bei Entwicklern zu Desinteresse führen können, wenn das "Rauschen" zu groß wird. Er stellt Industriestandards wie SARIF vor, um die Integration verschiedener Tools in CI/CD-Pipelines zu vereinheitlichen.

Besonders hervorzuheben ist Bugayenkos pädagogischer Ansatz: Er betrachtet statische Analyse als Erziehungswerkzeug. Er lehnt "Auto-Fixer" ab, da diese den Lerneffekt verhindern. Entwickler sollen Fehlermeldungen manuell beheben, um die zugrunde liegenden Prinzipien zu verstehen und langfristig bessere Programmiergewohnheiten zu entwickeln. Das Ziel ist es, von schlechten Mustern zu sogenannten "Code Perfumes" (besonders sauberem Code) zu gelangen.

## Kernaussagen
* „Statische Analyse ist ein Lehrmittel; Entwickler sollten Warnungen manuell korrigieren, um wirklich aus ihren Fehlern zu lernen.“
* „Durch das 'Shift-Left'-Prinzip werden strukturelle Mängel erkannt, bevor der Code jemals ausgeführt wird.“
* „Falsch-positive Ergebnisse sind der größte Feind; zu viel Rauschen führt dazu, dass Entwickler selbst kritische Warnungen ignorieren.“
* „Wir sollten nach 'Code Perfumes' streben – Mustern, die so professionell sind, dass sie das Gegenteil von Code-Gerüchen darstellen.“

## Relevanz: 5/5
Äußerst relevant für Software-Architekten und Teamleiter, die Automatisierung zur Sicherung der Code-Qualität und zur Ausbildung ihrer Entwickler nutzen wollen.
