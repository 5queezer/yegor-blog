---
title: "SQM 15/24: Code Coverage [Software-Qualitäts-Crashkurs]"
date: 2024-01-17T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/pJrXQ5rptig/maxresdefault.jpg"
  alt: "SQM 15/24: Code Coverage [Software-Qualitäts-Crashkurs]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=pJrXQ5rptig](https://www.youtube.com/watch?v=pJrXQ5rptig)

## Zusammenfassung
In dieser Vorlesung behandelt Yegor Bugayenko die Metrik "Code Coverage" (Testabdeckung) als wesentliches Instrument des Qualitätsmanagements. Er erläutert vier Arten der Abdeckung: Anweisungs-, Zweig-, Bedingungs- und Pfadüberdeckung, wobei jede Stufe die Komplexität und Strenge des Testprozesses erhöht. Historisch spannt er den Bogen von den Pionierarbeiten der 1960er Jahre bis hin zu modernen Industriestandards wie den Google-Testrichtlinien oder der ISO 26262 für sicherheitskritische Systeme im Automobilbereich.

Bugayenko vertritt die radikale Ansicht, dass eine Testabdeckung von 100 % der einzige akzeptable Standard ist. Seiner Meinung nach bedeutet eine Schwelle von beispielsweise 80 %, dass man offiziell erlaubt, 20 % des Codes ungeprüft und potenziell fehlerhaft im Projekt zu belassen. Er sieht die Metrik primär als Management-Werkzeug: Die Abdeckung sollte fest in den CI/CD-Prozess integriert sein. Sinkt die Abdeckung, muss der Build automatisch scheitern ("Fail the Build"). Er warnt jedoch vor sogenannten "Line Hitters"—Tests, die Code lediglich ausführen, ohne tatsächliche logische Überprüfungen (Asserts) durchzuführen. Daher sei Code Coverage zwar eine notwendige Bedingung für Qualität, aber erst in Kombination mit Mutationstests (Mutation Coverage) wirklich aussagekräftig, um die Wirksamkeit der Tests zu garantieren.

## Kernaussagen
* „Code Coverage ist eine Metrik Ihrer Unwissenheit. Sie zeigt den Teil des Codes, den Sie überhaupt nicht kontrollieren.“
* „Eine hohe Abdeckung garantiert keine Fehlerfreiheit, aber eine geringe Abdeckung garantiert das Vorhandensein von Fehlern.“
* „Wer 80 % Abdeckung akzeptiert, erlaubt seinen Programmierern offiziell, 20 % minderwertigen, ungeprüften und potenziell gefährlichen Code zu schreiben.“
* „Qualität lässt sich nicht durch Zureden verbessern, sondern nur durch Messung und strikte Einhaltung der Zahlen.“

## Relevanz: 5/5
Die Vorlesung ist essentiell für Software-Architekten und Teamleiter, da sie eine kompromisslose Sicht auf Qualitätskontrolle und die Automatisierung von Management-Entscheidungen bietet.
