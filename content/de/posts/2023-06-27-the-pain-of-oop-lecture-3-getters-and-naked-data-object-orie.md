---
title: "Die Qual von OOP, Vorlesung #3: Getter und nackte Daten"
date: 2023-06-27T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
  - "oop"
  - "ai"
cover:
  image: "https://img.youtube.com/vi/2YyVmIQQ23w/maxresdefault.jpg"
  alt: "Die Qual von OOP, Vorlesung #3: Getter und nackte Daten"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=2YyVmIQQ23w](https://www.youtube.com/watch?v=2YyVmIQQ23w)

## Zusammenfassung
In dieser Vorlesung thematisiert Yegor Bugayenko eines der hartnäckigsten Probleme der modernen Softwareentwicklung: den Einsatz von Gettern. Er vertritt die Ansicht, dass Methoden mit dem Präfix `get...` ein Objekt von einem aktiven Akteur in einen passiven Datenbehälter („nackte Daten“) verwandeln. Die zentrale These lautet, dass echte Kapselung nicht nur bedeutet, Felder privat zu machen, sondern die Struktur der Daten gänzlich zu verbergen. Wenn ein Objekt es zulässt, dass sein Inneres nach außen getragen wird, verliert es seine Identität als Objekt und wird zu einer reinen Datenstruktur.

Bugayenko kritisiert moderne IDEs und Bibliotheken wie Lombok, die das automatische Erzeugen von Gettern fördern und so zur Entstehung „anämischer Modelle“ beitragen. In solchen Modellen besitzen Objekte keine eigene Logik; stattdessen wird die Geschäftslogik in externe Dienste ausgelagert, was eine Rückkehr zum prozeduralen Programmieren darstellt. Besonders scharf kritisiert er Data Transfer Objects (DTOs), die er als „das ultimative Übel“ bezeichnet, da sie zwar wie Objekte aussehen, aber keine deren Eigenschaften besitzen.

Als Alternative zu Gettern schlägt er das Prinzip „Tell, Don't Ask“ (Sag es ihm, frag nicht) vor. Anstatt Daten abzurufen, um außerhalb eine Entscheidung zu treffen, sollte man das Objekt anweisen, eine Aktion basierend auf seinem internen Zustand selbst auszuführen. Zudem plädiert er für die Abschaffung des `get`-Präfixes. Methoden sollten als Substantive benannt werden (z. B. `weight()` statt `getWeight()`), um zu verdeutlichen, dass man mit einer lebendigen Entität interagiert. Die Vorlesung endet mit einer Kritik am Spring-Framework, dessen Fokus auf „Beans“ und Getter/Setter Java in eine prozedurale Sprache zurückverwandelt.

## Kernaussagen
*   „Ein Getter ist ein Weg, ein Objekt auszuziehen und seine nackten Daten der Welt zu zeigen.“
*   „Ein Objekt ist kein Dateneimer; es ist ein lebender Organismus mit eigenem Verhalten.“
*   „DTOs sind das ultimative Übel in OOP, weil sie das restliche System zwingen, prozedural zu sein.“
*   „Kapselung bedeutet nicht, Felder zu verstecken, sondern die Tatsache zu verbergen, dass überhaupt Daten im Objekt existieren.“

## Relevanz: 5/5
Diese Vorlesung ist von entscheidender Bedeutung für Entwickler, die sich mit sauberem Code und echter Objektorientierung auseinandersetzen möchten, insbesondere um anämische Domänenmodelle zu vermeiden.
