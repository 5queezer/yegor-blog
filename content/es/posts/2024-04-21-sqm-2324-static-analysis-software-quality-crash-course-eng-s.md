---
title: "SQM 23/24: Análisis Estático [curso de calidad de software]"
date: 2024-04-21T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/QK2XQvYoEpQ/maxresdefault.jpg"
  alt: "SQM 23/24: Análisis Estático [curso de calidad de software]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=QK2XQvYoEpQ](https://www.youtube.com/watch?v=QK2XQvYoEpQ)

## Resumen
En esta lección, Yegor Bugayenko presenta el análisis estático como un pilar fundamental de la Gestión de Calidad de Software (SQM). Lo define como la inspección automática del código fuente sin ejecutarlo, diferenciándolo del análisis dinámico (pruebas). La sesión recorre la evolución de estas herramientas a través de tres generaciones: desde la simple coincidencia de patrones (1ª gen) hasta el análisis de flujo de control (2ª gen) y el análisis lógico global e interprocedural (3ª gen).

Yegor categoriza los problemas en: Violaciones de Estilo, "Code Smells" (olores de código) y Bugs. Dedica una parte importante a los desafíos técnicos, especialmente al "ruido" generado por los falsos positivos, que pueden llevar a los desarrolladores a ignorar las herramientas. También menciona estándares industriales como SARIF para la integración de resultados en flujos de CI/CD.

Lo más distintivo de la charla es la filosofía pedagógica de Bugayenko. Sostiene que el análisis estático es una herramienta de entrenamiento. Se opone al uso de "auto-fixers" (correctores automáticos) porque eliminan el aprendizaje. Según él, el desarrollador debe "sufrir" corrigiendo manualmente las advertencias para interiorizar las buenas prácticas, pasando de los "olores de código" a los "perfumes de código" (patrones de excelencia).

## Ideas Clave
* "El análisis estático es una herramienta de formación; los desarrolladores deben corregir las advertencias manualmente para aprender de sus errores."
* "El objetivo de 'shift-left' es identificar fallos estructurales mucho antes de que el código llegue a un entorno de ejecución."
* "Los falsos positivos son el enemigo principal; si hay demasiado ruido, los desarrolladores acabarán ignorando incluso los errores críticos."
* "Debemos aspirar a los 'perfumes de código': patrones tan limpios que representen lo opuesto a un código maloliente."

## Relevancia: 5/5
Fundamental para ingenieros de software y líderes técnicos interesados en la automatización de estándares y la mejora continua del equipo.
