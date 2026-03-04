---
title: "I23: A. S. Medvednikov | El lenguaje de programación V: simple, rápido, seguro, compilado, de código abierto"
date: 2024-05-28T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/xMGNlUZQ-6w/maxresdefault.jpg"
  alt: "I23: A. S. Medvednikov | El lenguaje de programación V: simple, rápido, seguro, compilado, de código abierto"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=xMGNlUZQ-6w](https://www.youtube.com/watch?v=xMGNlUZQ-6w)

## Resumen
En esta entrevista, Yegor Bugayenko conversa con Alexander Medvednikov, el creador del lenguaje de programación V (vlang). Alexander explica que V nació de la necesidad práctica de un lenguaje tan sencillo como Go pero tan rápido y seguro como Rust, específicamente para desarrollar su cliente de mensajería de alto rendimiento, "Volt". Un tema central es la extrema velocidad de compilación de V (más de un millón de líneas por segundo), lograda mediante un compilador diminuto que evita dependencias pesadas como LLVM por defecto, traduciendo a C o directamente a código máquina.

La discusión abarca innovaciones técnicas como el manejo de memoria de V, que busca un punto medio entre el control manual y la recolección de basura mediante análisis en tiempo de compilación (autofree). Alexander destaca características de seguridad como la ausencia de punteros nulos, la falta de variables globales y la inmutabilidad obligatoria por defecto. También abordan el escepticismo de la comunidad de desarrolladores ante las ambiciosas promesas de V, a lo que Alexander responde señalando el ecosistema creciente y las aplicaciones reales funcionales. La conversación subraya una filosofía de simplicidad radical: proporcionar una sola forma de resolver un problema y mantener el núcleo del lenguaje lo suficientemente pequeño para ser comprendido por un solo desarrollador.

## Ideas Clave
- "V está diseñado para ser un lenguaje sin legado; toma lo mejor de Go, Rust y Oberon pero elimina la complejidad."
- "Compilar a 1.2 millones de líneas por segundo no es solo un truco; cambia fundamentalmente el ciclo de retroalimentación del desarrollador."
- "La seguridad no debe ser un ejercicio académico; se trata de prevenir errores comunes mediante reglas estrictas en el lenguaje, como evitar el estado global."

## Relevancia: 5/5
Extremadamente relevante para ingenieros interesados en el diseño de lenguajes, el rendimiento de los compiladores y el equilibrio entre seguridad y simplicidad.
