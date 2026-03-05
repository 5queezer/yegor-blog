---
title: "SQM 16/24: Cobertura de Mutación [curso intensivo de calidad de software] [eng sub]"
date: 2024-01-31T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/WYWSv_PucHc/maxresdefault.jpg"
  alt: "SQM 16/24: Cobertura de Mutación [curso intensivo de calidad de software] [eng sub]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=WYWSv_PucHc](https://www.youtube.com/watch?v=WYWSv_PucHc)

## Resumen
En esta exhaustiva conferencia del curso de Métricas de Calidad de Software (SQM), Yegor Bugayenko critica la dependencia de la industria en las métricas tradicionales de cobertura de código, como líneas y ramas. Argumenta que estas métricas son defectuosas porque se limitan a rastrear la ejecución del código en lugar de realizar una verificación genuina. Un conjunto de pruebas puede alcanzar un 100% de cobertura ejecutando todas las rutas sin contener una sola aserción, proporcionando una falsa seguridad. Para abordar esto, Bugayenko presenta la Cobertura de Mutación (Pruebas de Mutación) como una alternativa mucho más rigurosa y fiable para evaluar la calidad de las pruebas.

La metodología de las pruebas de mutación implica inyectar deliberadamente pequeños fallos artificiales, denominados "mutantes", en el código fuente. Estas mutaciones incluyen alterar operadores matemáticos, cambiar operadores relacionales o invertir lógica booleana. El objetivo es observar la reacción de las pruebas. Si al menos una prueba falla en respuesta al fallo inyectado, el mutante es "asesinado", lo que significa que las pruebas validan eficazmente el comportamiento del código. Por el contrario, si todas las pruebas siguen pasando, el mutante "sobrevive". Un mutante que sobrevive expone un punto ciego donde el código se ejecuta, pero su comportamiento no se verifica con precisión. Aunque las pruebas de mutación son costosas computacionalmente debido al elevado número de ejecuciones requeridas, Bugayenko subraya que ofrecen retroalimentación directa y una "puntuación de mutación" objetiva que es extremadamente difícil de manipular para los desarrolladores, conduciendo a una mayor fiabilidad del software.

## Ideas Clave
1. "La cobertura de código tradicional solo mide la ejecución, no la verificación; las pruebas pueden pasar perfectamente sin hacer una sola aserción."
2. "Un mutante asesinado demuestra que su conjunto de pruebas está validando activamente la lógica y el comportamiento del código, en lugar de simplemente ejecutarlo."
3. "La puntuación de mutación proporciona una métrica objetiva y a prueba de manipulaciones que es extremadamente difícil de alterar para los desarrolladores."
4. "Aunque es computacionalmente costoso, las pruebas de mutación proporcionan comentarios muy procesables al revelar puntos ciegos exactos en la verificación de pruebas."

## Relevancia: 5/5
Altamente relevante para la ingeniería de software, las pruebas y la gestión de equipos, ya que fomenta prácticas sólidas de control de calidad y evita que se infle artificialmente la calidad de las pruebas.
