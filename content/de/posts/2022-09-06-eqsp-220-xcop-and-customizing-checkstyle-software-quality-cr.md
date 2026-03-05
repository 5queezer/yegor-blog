---
title: "EQSP 2/20: XCOP und Anpassung von Checkstyle"
date: 2022-09-06T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/utKC7Bkkuzk/maxresdefault.jpg"
  alt: "EQSP 2/20: XCOP und Anpassung von Checkstyle"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=utKC7Bkkuzk](https://www.youtube.com/watch?v=utKC7Bkkuzk)

## Zusammenfassung
Dieses Video aus dem Kurs „Engineering Quality of Software Projects“ (EQSP) behandelt die konsequente Automatisierung der Softwarequalität durch XCOP und Checkstyle. Yegor Bugayenko stellt XCOP vor, ein von ihm entwickeltes Tool zur Validierung von XML-Dateien. Er argumentiert, dass auch XML-Konfigurationen wie `pom.xml` strengen Formatierungsregeln und Lizenzvorgaben entsprechen müssen, um die Wartbarkeit zu gewährleisten. XCOP prüft dabei insbesondere die Einrückung und das Vorhandensein korrekter Lizenztexte.

Der zweite Teil widmet sich der Anpassung von Checkstyle für Java-Projekte. Bugayenko fordert eine extrem strikte Konfiguration, die den Build bei jeder kleinsten Abweichung sofort abbricht („Fail-Fast“). Er lehnt IDE-Auto-Formatter ab, da diese die Lernkurve der Entwickler untergraben; stattdessen sollen Fehler manuell behoben werden, um die Regeln zu verinnerlichen. Die zentrale Botschaft ist, dass statische Analyse menschliche Diskussionen über Codestil ersetzen sollte, um eine konsistente, hochwertige Codebasis nach den Prinzipien der „Elegant Objects“ zu schaffen.

## Kernaussagen
- „XML ist ebenso Code wie Java; Unordnung in Konfigurationsdateien deutet auf mangelnde Professionalität hin.“
- „Ein Build-Prozess, der bei Stilfehlern nicht abbricht, ist wertlos.“
- „Checkstyle-Regeln sollten architektonische Prinzipien wie Immutability erzwingen, nicht nur die Platzierung von Klammern.“
- „Manuelle Code-Reviews für Stilfragen sind Zeitverschwendung – überlassen Sie das der Maschine.“

## Relevanz: 5/5
Essentiell für die Etablierung einer professionellen Build-Pipeline und strenger OOP-Standards.
