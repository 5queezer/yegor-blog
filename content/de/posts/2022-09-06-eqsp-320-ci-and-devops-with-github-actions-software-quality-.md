---
title: "EQSP 3/20: CI und DevOps mit GitHub Actions [Software-Qualitäts-Crashkurs]"
date: 2022-09-06T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/c2_h7CMzUgA/maxresdefault.jpg"
  alt: "EQSP 3/20: CI und DevOps mit GitHub Actions [Software-Qualitäts-Crashkurs]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=c2_h7CMzUgA](https://www.youtube.com/watch?v=c2_h7CMzUgA)

## Zusammenfassung
In dieser Vorlesung aus seinem „Software Quality Crash Course“ erläutert Yegor Bugayenko die praktischen und philosophischen Grundlagen von Continuous Integration (CI) und DevOps unter Verwendung von GitHub Actions. Er definiert CI nicht nur als Testverfahren, sondern als einen „Schutzmechanismus“, der verhindert, dass minderwertiger Code in das Haupt-Repository gelangt. Das Herzstück seines Ansatzes ist das Prinzip des „Read-Only Master“: Entwickler dürfen niemals direkt in den Master-Branch pushen. Stattdessen müssen alle Änderungen eine strenge, automatisierte Pipeline durchlaufen, die Unit-Tests (Maven), Stilprüfungen (Xcop), Qualitätsmetriken (Kulis) und Sicherheits-Scans (Snyk) umfasst.

Bugayenko hebt die Vorteile von GitHub Actions hervor, insbesondere die YAML-basierte Konfiguration und die kostenlose Infrastruktur für Open-Source-Projekte. Er demonstriert fortgeschrittene Funktionen wie Matrix-Builds, um Code gleichzeitig auf verschiedenen JDK-Versionen zu testen. Ein wesentlicher Teil des Vortrags ist „Rulor“ gewidmet, einem Chatbot, der den Merge-Prozess steuert. Durch Befehle wie `@rulor merge` erstellt der Bot eine isolierte Umgebung, führt den Merge lokal aus, durchläuft alle Prüfungen und pusht erst dann in den Master, wenn alles fehlerfrei ist. Dies verlagert die Verantwortung für die Qualität vom einzelnen Programmierer auf das „System“. Wenn ein Fehler den Master erreicht, wird dies als Versagen der Pipeline und nicht der Person gewertet.

## Kernaussagen
- „Qualität entsteht, wenn man die schlechten Teile bewusst und explizit entfernt.“
- „Der Master ist heilig: Pushen Sie niemals direkt; lassen Sie die Roboter ihn beschützen.“
- „Beschuldigen Sie das System, nicht die Person: Wenn ein Fehler den Master erreicht, ist Ihre CI-Pipeline gescheitert.“
- „Jede Codezeile muss mit einem Ticket verknüpft sein; ohne explizite Absicht gibt es keinen Code.“

## Relevanz: 5/5
Äußerst relevant für das moderne Software-Engineering. Die Vorlesung bietet eine klare Anleitung für den Aufbau robuster Delivery-Pipelines und eine Kultur der automatisierten Verantwortlichkeit.
