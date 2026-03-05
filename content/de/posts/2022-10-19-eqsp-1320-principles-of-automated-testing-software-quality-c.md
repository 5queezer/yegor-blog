---
title: "EQSP 13/20: Prinzipien des automatisierten Testens"
date: 2022-10-19T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
  - "testing"
cover:
  image: "https://img.youtube.com/vi/hzrzq5HAhvM/maxresdefault.jpg"
  alt: "EQSP 13/20: Prinzipien des automatisierten Testens"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=hzrzq5HAhvM](https://www.youtube.com/watch?v=hzrzq5HAhvM)

## Zusammenfassung
In diesem Vortrag erläutert Yegor Bugayenko die grundlegende Philosophie und die technische Notwendigkeit automatisierter Tests im Rahmen der Softwarequalität. Er argumentiert, dass automatisierte Tests nicht nur ein Werkzeug zur Fehlersuche sind, sondern ein entscheidender Mechanismus zur Erhöhung der Entwicklungsgeschwindigkeit und zur Eliminierung der sogenannten „angstgetriebenen Entwicklung“ (Fear-Driven Development). Ohne eine robuste Testsuite entwickeln Programmierer Angst vor Änderungen am Code, was zu Stagnation und technischen Schulden führt.

Das Herzstück von Bugayenkos Ansatz ist das Konzept des „Sicherheitsnetzes“. Eine umfassende Suite automatisierter Tests ermöglicht es Entwicklern, mutige Änderungen vorzunehmen, da sie darauf vertrauen können, dass Regressionen sofort erkannt werden. Er unterscheidet strikt zwischen Unit-Tests – die extrem schnell sein und sofortiges Feedback liefern müssen – und Integrationstests, die das Systemverhalten breiter abdecken, aber naturgemäß langsamer sind.

Ein wesentliches Prinzip ist der obligatorische Zyklus der Fehlerreproduktion: Ein Fehler sollte niemals behoben werden, bevor ein automatisierter Test geschrieben wurde, der diesen Fehler reproduziert. Wenn der Code fehlerhaft ist, die Tests aber bestehen, liegt das Versagen in der Teststrategie selbst. Indem Tests als gleichwertiger Bestandteil des Quellcodes behandelt werden, stellen Teams sicher, dass ein einmal behobener Fehler nie wieder unbemerkt auftritt. Letztendlich ist das Ziel der Automatisierung die Schaffung einer deterministischen Umgebung, in der Qualität ein messbares Nebenprodukt des Entwicklungsprozesses ist.

## Kernaussagen
- „Wenn Sie einen Fehler haben, aber Ihre Tests bestehen, liegt das Problem nicht im Code, sondern in Ihren Tests.“
- „Manuelles Testen ist eine Verschwendung von menschlichem Potenzial; was eine Maschine prüfen kann, muss eine Maschine prüfen.“
- „Das Ziel automatisierter Tests ist es, Angst zu eliminieren, damit Entwickler produktiv 'unvorsichtig' sein können.“
- „Eine Fehlerbehebung ohne reproduzierenden Test ist nur ein temporäres Pflaster, das irgendwann wieder versagen wird.“

## Relevanz: 5/5
Dieser Vortrag ist grundlegend für das Verständnis der Integration von Tests in CI/CD-Pipelines und deren Einfluss auf die Teamproduktivität und Wartbarkeit.
