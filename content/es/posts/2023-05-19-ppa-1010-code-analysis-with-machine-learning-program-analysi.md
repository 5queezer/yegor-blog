---
title: "PPA 10/10: Análisis de código con aprendizaje automático [curso intensivo de análisis de programas]"
date: 2023-05-19T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/6Z1EFTJ7Kdo/maxresdefault.jpg"
  alt: "PPA 10/10: Análisis de código con aprendizaje automático [curso intensivo de análisis de programas]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=6Z1EFTJ7Kdo](https://www.youtube.com/watch?v=6Z1EFTJ7Kdo)

## Resumen
En esta última sesión del curso, Yegor Bugayenko aborda la convergencia entre el análisis de programas y el aprendizaje automático (ML), un campo conocido como "Big Code". Bugayenko sostiene que el análisis estático tradicional está limitado por la necesidad de que expertos humanos escriban reglas manualmente. El ML rompe esta barrera al permitir que las máquinas aprendan de millones de líneas de código disponibles en repositorios públicos. El concepto central es que el código no es solo lógica pura, sino que tiene una "naturalidad" estadística similar al lenguaje humano, lo que permite identificar patrones de uso, errores comunes y convenciones de estilo de manera automatizada.

El video profundiza en cómo representar el código para que sea procesable por algoritmos de ML. Bugayenko explica que tratar el código como simple texto es insuficiente; es necesario extraer su estructura mediante Árboles de Sintaxis Abstracta (AST) y grafos de flujo. Menciona herramientas y enfoques como Code2Vec, que transforman fragmentos de código en vectores numéricos (embeddings), permitiendo que el sistema "entienda" la intención del programador. Entre las aplicaciones destacan la detección de vulnerabilidades complejas, la sugerencia de nombres de variables y el autocompletado inteligente. Sin embargo, advierte sobre el desafío de la interpretabilidad: los desarrolladores necesitan entender el razonamiento detrás de una alerta de bug. Si un modelo de ML no puede explicar por qué considera que algo está mal, su utilidad en un entorno de ingeniería riguroso se ve comprometida.

## Ideas Clave
- "El código fuente es predecible y repetitivo, lo que lo hace perfecto para el análisis probabilístico mediante Big Code."
- "No estamos reemplazando las reglas lógicas, sino complementándolas con patrones que son demasiado complejos para ser descritos por un humano."
- "El problema fundamental del ML en el análisis de software es la explicabilidad: un ingeniero necesita una razón lógica, no una estadística, para cambiar su código."
- "Mediante el uso de AST y embeddings, podemos capturar la semántica profunda del programa más allá de las simples palabras clave."

## Relevancia: 5/5
Excelente para entender la base teórica de las herramientas modernas de IA aplicadas al desarrollo y cómo la estadística está transformando la verificación de software tradicional.
