---
title: "OSBP 5/8: Richtlinien festlegen [Open-Source-Crashkurs]"
date: 2024-04-17T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/mWi2S5FJiJ4/maxresdefault.jpg"
  alt: "OSBP 5/8: Richtlinien festlegen [Open-Source-Crashkurs]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=mWi2S5FJiJ4](https://www.youtube.com/watch?v=mWi2S5FJiJ4)

## Zusammenfassung
In diesem Teil seines Kurses erklärt Yegor Bugayenko, wie man durch strikte Regeln und Automatisierung die Qualität eines Open-Source-Projekts sichert. Er vertritt die Ansicht, dass Disziplin wichtiger ist als Flexibilität. Zu den wichtigsten Empfehlungen gehört das Vorhandensein einer klaren **Lizenz** (vorzugsweise MIT), da Code ohne Lizenz rechtlich nicht frei verwendbar ist. Zudem muss die **README.md** professionell wirken, Badges enthalten und dem Nutzer innerhalb von 10 Sekunden den Nutzen des Projekts vermitteln.

Ein zentraler Aspekt ist der Schutz des **Master-Branch**. Dieser sollte schreibgeschützt sein, sodass jede Änderung über einen Pull Request (PR) erfolgen muss. Bugayenko rät zudem davon ab, zu viel Energie in soziale „Code of Conducts“ zu stecken, und empfiehlt stattdessen die **Automatisierung von Richtlinien**. Er fordert Entwickler auf, GitHub Actions zu nutzen, um Codestil, Tests und statische Analysen automatisch zu prüfen. Wenn ein „Roboter“ einen PR ablehnt, spart dies dem Maintainer mühsame Diskussionen und sorgt für eine konsistente Codebasis.

## Kernaussagen
- „Je restriktiver du deinen Master-Branch schützt, desto gesünder bleibt dein Repository.“
- „Erkläre keine Regeln in Dokumenten – automatisiere sie als Check in der CI/CD-Pipeline.“
- „Ein Pull Request ist die einzige Tür zum Code; es gibt keine Abkürzungen.“

## Relevanz: 5/5
Hervorragend geeignet für Software-Architekten und Teamleiter, die Prozesse durch Tooling statt durch Mikromanagement optimieren wollen.
