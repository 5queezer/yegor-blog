---
title: "EQSP 10/20: Versionado Semántico de Artefactos [curso intensivo de calidad de software]"
date: 2022-10-06T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/xGjjRVmeCWA/maxresdefault.jpg"
  alt: "EQSP 10/20: Versionado Semántico de Artefactos [curso intensivo de calidad de software]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=xGjjRVmeCWA](https://www.youtube.com/watch?v=xGjjRVmeCWA)

## Resumen
Yegor Bugayenko sostiene que el versionado de software es un contrato estricto entre desarrolladores y usuarios. Aunque el estándar es el Versionado Semántico (MAJOR.MINOR.PATCH), la realidad es que los desarrolladores rara vez leen las notas de lanzamiento; simplemente actualizan y observan si algo falla. Para gestionar esto, Yegor enfatiza la **inmutabilidad de los artefactos**. Una vez que un paquete se publica en un repositorio central (como Maven Central), nunca debe modificarse ni eliminarse.

El video destaca la diferencia entre el control de versiones volátil (GitHub) y los repositorios de artefactos estables. GitHub es "fluido" y poco confiable para dependencias de producción, mientras que los gestores de paquetes ofrecen la estabilidad necesaria. Bugayenko también critica prácticas "anticuadas" como los registros de cambios manuales y la duplicación de información de versión en múltiples archivos, considerándolo una fuente primaria de errores. Propone en su lugar la automatización total, documentación ejecutable y el uso de insignias (badges) dinámicas como única fuente de verdad.

## Ideas Clave
* "La duplicación de información es la fuente de la mayoría de los problemas en la programación."
* "GitHub es una fuente de información muy volátil; no debemos confiar en ella. Podemos confiar plenamente en Maven Central al 100%."
* "Los lanzamientos deben ser inmutables... la versión que fue publicada debe permanecer allí para siempre."
* Las notas de lanzamiento manuales son obsoletas; la fuente de verdad debe estar automatizada e integrada en el proceso de construcción.

## Relevancia: 5/5
Crucial para arquitectos de software y líderes técnicos que buscan robustez en sus procesos de despliegue.
