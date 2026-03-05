---
title: "EQSP 11/20: Veröffentlichung von Anwendungen als Artefakte"
date: 2022-10-06T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/9YeTbqFr85s/maxresdefault.jpg"
  alt: "EQSP 11/20: Veröffentlichung von Anwendungen als Artefakte"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=9YeTbqFr85s](https://www.youtube.com/watch?v=9YeTbqFr85s)

## Zusammenfassung
In diesem Vortrag erläutert Yegor Bugayenko den entscheidenden Unterschied zwischen einer Softwarebibliothek (Paket) und einer vollständigen Anwendung im Kontext des Release-Managements. Während eine Bibliothek eine Abhängigkeit für andere Entwickler ist, stellt eine Anwendung ein Endprodukt dar, das eine robustere Bereitstellungsstrategie erfordert. Die zentrale These ist die „Artefakt-Philosophie“: Eine Anwendung sollte als eine einzige, unveränderliche und versionierte Einheit geliefert werden – beispielsweise als Docker-Image oder als „Fat JAR“. Dieser Ansatz gewährleistet die Unabhängigkeit von der Umgebung und eliminiert die Risiken, die mit manuellen Dateiübertragungen oder Konfigurationsfehlern verbunden sind.

Yegor betont, dass ein Deployment niemals ein „git pull“ auf einem Produktionsserver beinhalten sollte. Stattdessen sollte es ein kontrollierter „Switch“ sein, bei dem eine neue Version des Artefakts parallel zur alten gestartet wird. Um die Datenintegrität während dieses Übergangs zu wahren, schlägt er einen „Read-Only-Modus“ vor, in dem die alte Version kurz vor der Umleitung des Datenverkehrs aufhört, in die Datenbank zu schreiben. Darüber hinaus muss der gesamte Prozess vollständig automatisiert sein. Mithilfe von Tools wie Rultor sollten Entwickler Releases durch einfache Befehle in einem Ticket auslösen und das Testen, Taggen und Deployen autonomen Bots überlassen. Dies schließt menschliche Fehler aus und stellt sicher, dass die Produktionsumgebung ein unberührter Raum bleibt.

## Kernaussagen
- „Eine Anwendung ist nicht nur Code; sie ist ein einziges, unveränderliches Artefakt, das alles enthalten muss, was es zum Ausführen benötigt.“
- „Wenn Sie ein 'git pull' auf Ihrem Produktionsserver durchführen, sind Sie kein Profi, sondern ein Hobbyist, der mit dem Feuer spielt.“
- „Der Bereitstellungsprozess ist im Wesentlichen ein Umschalten des Datenverkehrs zwischen zwei unveränderlichen Zuständen des Systems.“
- „Zero-Downtime wird nicht durch Magie erreicht, sondern indem das System während der kritischen Sekunden des Übergangs in den schreibgeschützten Modus versetzt wird.“

## Relevanz: 5/5
Dieses Video ist von grundlegender Bedeutung für das Verständnis moderner CI/CD-Praktiken und der DevOps-Kultur. Es vermittelt die Abkehr von der codezentrierten hin zur artefaktzentrierten Auslieferung.
