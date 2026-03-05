---
title: "Warum Code-Style-Prüfung obligatorisch ist?"
date: 2022-09-04T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/ZeraaVNW1mo/maxresdefault.jpg"
  alt: "Warum Code-Style-Prüfung obligatorisch ist?"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=ZeraaVNW1mo](https://www.youtube.com/watch?v=ZeraaVNW1mo)

## Zusammenfassung
In diesem Vortrag legt Yegor Bugayenko dar, dass automatisierte Style-Checks weit mehr als nur eine Frage der Ästhetik sind; sie sind ein essentielles Werkzeug zur Durchsetzung von Teamdisziplin. Er argumentiert, dass Style-Checker als unparteiische „Richter“ fungieren, die subjektive Konflikte in Code-Reviews eliminieren. Ohne diese Automatisierung verschwenden Entwickler wertvolle Zeit mit Diskussionen über Formatierungen, was zu unnötigen Spannungen führt. Sobald ein Tool die Regeln vorgibt, endet die Debatte über Meinungen, und es gilt das Gesetz des Projekts.

Bugayenko sieht die Beachtung des Codestils zudem als Lackmustest für die Professionalität eines Entwicklers. Wer bei oberflächlichen Details wie Einrückungen nachlässig ist, wird höchstwahrscheinlich auch bei kritischen Aspekten wie der Speicherverwaltung oder der Softwarearchitektur schlampen. Qualität lässt sich laut Yegor nicht durch freundliche Bitten oder Meetings erreichen, sondern muss durch das Build-System erzwungen werden: Wenn der Style-Check fehlschlägt, bricht der Build ab. Dies entlastet den menschlichen Reviewer, der sich nun auf die Logik konzentrieren kann, während die Maschine die Einhaltung formaler Standards garantiert. Ein professioneller Workflow zeichnet sich dadurch aus, dass am Ende ein „Roboter“ den Merge-Button drückt, nachdem alle automatisierten Hürden genommen wurden.

## Kernaussagen
- „Ein Style-Checker ist wie ein Richter für uns; es zählt nicht mehr meine oder deine Meinung, sondern die Entscheidung des Tools.“
- „Wenn ein Programmierer nicht auf den Stil achtet, wird er auch nicht auf die Qualität des restlichen Codes achten.“
- „Gib nicht den Menschen die Schuld für schlechten Code, sondern dem System, das diesen Code zugelassen hat.“
- „Menschliche Reviewer sollten sich auf Logik und Architektur konzentrieren; überlasst Leerzeichen und Klammern den Robotern.“

## Relevanz: 5/5
Ein entscheidender Beitrag zum Verständnis von Softwarequalität und zur Effizienzsteigerung in der agilen Softwareentwicklung.
