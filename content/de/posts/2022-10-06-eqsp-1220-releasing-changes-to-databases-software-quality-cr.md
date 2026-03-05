---
title: "EQSP 12/20: Veröffentlichung von Datenbankänderungen"
date: 2022-10-06T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
  - "infrastructure"
cover:
  image: "https://img.youtube.com/vi/qtTG1kRLzCY/maxresdefault.jpg"
  alt: "EQSP 12/20: Veröffentlichung von Datenbankänderungen"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=qtTG1kRLzCY](https://www.youtube.com/watch?v=qtTG1kRLzCY)

## Zusammenfassung
In dieser Lerneinheit seines Kurses über Softwarequalität vertritt Yegor Bugayenko die Ansicht, dass Datenbanken als integraler Bestandteil des Quellcodes behandelt werden müssen. Der Kern seiner Argumentation ist die absolute Ablehnung manueller Eingriffe in Produktionsdatenbanken. Solche "Hauruck-Aktionen" seien ein Zeichen mangelnder Professionalität und führten unweigerlich zu Inkonsistenzen und Fehlern. Stattdessen muss jede Änderung am Schema oder an den Daten durch automatisierte, versionierte Migrationsskripte (wie 001.sql, 002.sql) erfolgen, die im selben Repository wie der Anwendungscode liegen.

Bugayenko hebt die Bedeutung von Tools wie Liquibase oder Flyway hervor, die den Status der Datenbank verfolgen und sicherstellen, dass Migrationen deterministisch ablaufen. Der vorgeschlagene Workflow sieht vor, dass die CI/CD-Pipeline die einzige Instanz ist, die Schreibrechte auf die Produktionsdatenbank besitzt. Programmierer sollten keinen direkten Zugriff haben; ihre Aufgabe ist es, Änderungen über Merge-Requests einzureichen, die von einem Architekten geprüft werden. Dieser Ansatz entzieht dem Einzelnen die Macht über die Infrastruktur und überträgt sie auf den automatisierten Prozess. Dies garantiert nicht nur die Reproduzierbarkeit der Umgebungen, sondern verhindert auch das gefürchtete "Configuration Drift". Letztlich ist die Automatisierung der Datenbank-Releases laut Bugayenko die einzige Möglichkeit, bei wachsenden Systemen eine hohe Softwarequalität und Ausfallsicherheit zu gewährleisten.

## Kernaussagen
- "Die Datenbank ist kein externes Anhängsel, sondern ein lebendiger Teil des Codes, der mit ihm versioniert werden muss."
- "Manueller Zugriff auf die Produktion ist ein Freibrief für schlechte Qualität und technisches Chaos."
- "Wir müssen den Programmierern die Autorität entziehen und sie dem automatisierten Prozess übertragen."
- "Ein Architekt entscheidet über den Merge-Request, aber die Pipeline führt die Änderung aus – niemals ein Mensch direkt."

## Relevanz: 5/5
Äußerst relevant für DevOps, Software-Architekten und Teams, die den Übergang zu Continuous Delivery und stabilen, automatisierten Infrastrukturen meistern wollen.
