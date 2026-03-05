---
title: "SQM 12/24: Código Muerto [curso intensivo de calidad de software] [subtítulos en inglés]"
date: 2023-12-17T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/zN0gX9m6a2k/maxresdefault.jpg"
  alt: "SQM 12/24: Código Muerto [curso intensivo de calidad de software] [subtítulos en inglés]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=zN0gX9m6a2k](https://www.youtube.com/watch?v=zN0gX9m6a2k)

## Resumen
En su conferencia "SQM 12/24: Dead Code", parte del curso intensivo de Métricas de Calidad de Software, Yegor Bugayenko aborda el problema generalizado del código muerto y su impacto perjudicial en el mantenimiento del software. El código muerto —código que nunca se ejecuta o cuyos resultados no se utilizan en absoluto— se clasifica como un "mal olor" (bad smell) severo en la programación orientada a objetos. Bugayenko enfatiza que su presencia infla artificialmente la carga cognitiva de los desarrolladores, dificultando significativamente la refactorización y acelerando la "podredumbre del software" (bit rot). Explica cómo las herramientas de análisis estático y los compiladores modernos manejan la Eliminación de Código Muerto (DCE), pero sostiene que los desarrolladores deben podar activamente sus bases de código en lugar de depender únicamente de herramientas automatizadas.

Una parte importante de la conferencia gira en torno a la arquitectura de repositorios, comparando específicamente los repositorios monolíticos (Monorepos) con los Polyrepos ("Manyrepos"). Aunque reconoce que gigantes tecnológicos como Google y Facebook utilizan con éxito monorepos para reducir la sobrecarga de integración, Bugayenko critica duramente este enfoque para la mayoría de los equipos. Argumenta que los monorepos conducen inevitablemente a una calidad de código comprometida, límites difusos y una mala encapsulación. En su lugar, defiende la estrategia de Manyrepo. Al dividir los proyectos en repositorios más pequeños y desacoplados, los equipos pueden lograr compilaciones independientes más rápidas, aplicar una encapsulación más estricta, mantener métricas más limpias y simplificar el proceso de pruebas. También introduce el concepto de "volatilidad" del código —midiendo la frecuencia con la que cambian los archivos— para identificar áreas estancadas que pueden ocultar código muerto.

## Ideas Clave
- "El código muerto no es solo texto inofensivo; es un lastre que aumenta activamente la carga cognitiva y frena la refactorización futura."
- "Aunque los monorepos pueden resolver los dolores de cabeza de la integración, a menudo lo hacen a costa de la encapsulación y la calidad del código."
- "El código que no cambia es código que se pudre. La alta volatilidad es un signo de vida, mientras que el código estancado a menudo enmascara lógica muerta o irrelevante."
- "No confíe exclusivamente en la eliminación de código muerto del compilador; mantener la base de código estrictamente limpia es responsabilidad directa del desarrollador."

## Relevancia: 5/5
Esta conferencia es altamente relevante para la ingeniería de software y la gestión de equipos. Aborda directamente los desafíos diarios del mantenimiento del código, la refactorización y las decisiones arquitectónicas (Monorepo vs. Manyrepo) que dictan la velocidad a largo plazo y la calidad del código.
