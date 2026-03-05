---
title: "EQSP 4/20: Erstellen eigener GitHub Actions, am Beispiel [Software Quality Crash Course]"
date: 2022-09-07T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/7oKqqgpKjIM/maxresdefault.jpg"
  alt: "EQSP 4/20: Erstellen eigener GitHub Actions, am Beispiel [Software Quality Crash Course]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=7oKqqgpKjIM](https://www.youtube.com/watch?v=7oKqqgpKjIM)

## Zusammenfassung
In dieser Lektion bietet Yegor Bugayenko eine praxisorientierte Anleitung zur Erstellung eigener GitHub Actions. Er betont, dass dies eine unverzichtbare Fähigkeit für Teams ist, die über Standardlösungen hinausgehen und ihre Softwarequalitätsprüfungen individuell automatisieren möchten. Laut Bugayenko erfordert professionelle Entwicklung die volle Kontrolle über den Automatisierungs-Stack, um spezifische Projektregeln ("Gesetze") konsequent durchzusetzen. Er unterscheidet dabei zwischen JavaScript-basierten und Docker-basierten Actions und spricht sich deutlich für die Docker-Variante aus. Docker-basierte Actions verpacken die gesamte Ausführungsumgebung (Betriebssystem, Abhängigkeiten und Tools) in einen Container, wodurch sichergestellt wird, dass die Action unabhängig von der Konfiguration des GitHub-Runners immer identisch ausgeführt wird.

Der technische Teil der Lektion konzentriert sich auf drei zentrale Dateien: `action.yml` (das Manifest, das Eingaben und Logik definiert), ein `Dockerfile` (die Definition der Umgebung) und ein Entry-Skript (meist `entry.sh`). Yegor demonstriert, wie man ein Kommandozeilen-Tool in einen Container integriert und so konfiguriert, dass es den Quellcode im Verzeichnis `/github/workspace` analysiert. Das Ziel ist die Schaffung eines "Fail-Fast"-Mechanismus: Jede Verletzung der Qualitätsstandards führt sofort zu einem fehlgeschlagenen Build-Status im Pull Request. Dies ersetzt subjektive menschliche Prüfungen durch objektive, automatisierte Skripte und sichert so ein konstant hohes Qualitätsniveau.

## Kernaussagen
- **Automatisierte "Gesetze":** Qualitätsstandards dürfen keine bloßen Empfehlungen sein; sie müssen als Skripte implementiert werden, die den Build im Fehlerfall abbrechen.
- **Umgebungskonsistenz:** Docker-basierte Actions sind JavaScript-Actions überlegen, da sie die Umgebung standardisieren und somit Abhängigkeitsprobleme eliminieren.
- **Objektives Feedback:** Der Hauptzweck eigener Actions besteht darin, Entwicklern über die CI/CD-Pipeline sofortiges, objektives und nicht verhandelbares Feedback zu geben.
- **Unabhängigkeit:** Sich nur auf Drittanbieter-Actions zu verlassen ist riskant; professionelle Teams sollten eigene Automatisierungskomponenten für kritische Qualitätsprüfungen entwickeln.

## Relevanz: 5/5
Äußerst relevant für Software-Entwickler und DevOps-Ingenieure. Die Lektion vermittelt die "Fail-Fast"-Philosophie und zeigt, wie man durch radikale Automatisierung die Codequalität in Teams nachhaltig sichert.
