---
title: "SQM 19/24: Densidad de Comentarios [curso intensivo de calidad de software]"
date: 2024-03-10T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/4_SNhBeyato/maxresdefault.jpg"
  alt: "SQM 19/24: Densidad de Comentarios [curso intensivo de calidad de software]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=4_SNhBeyato](https://www.youtube.com/watch?v=4_SNhBeyato)

## Resumen
En esta lección del curso de Métricas de Calidad de Software (SQM), Yegor Bugayenko analiza la "Densidad de Comentarios" como una métrica para evaluar la salud del código base. La premisa central es que la proporción de comentarios respecto al código es un indicador importante, pero solo si se distingue entre diferentes tipos de comentarios. Bugayenko traza una línea estricta entre la documentación de la API (como Javadoc o Doxygen) y los comentarios en línea colocados dentro de los cuerpos de los métodos.

Argumenta que la documentación a nivel de clase y método es obligatoria y altamente beneficiosa, ya que define el "qué" y el "por qué" de los componentes, estableciendo contratos claros para los usuarios de la API. Por lo tanto, una alta densidad de documentación de API es señal de un proyecto mantenible y de alta calidad.

Por el contrario, los comentarios en línea se consideran un "code smell" (síntoma de mal código) grave. Si un desarrollador se ve obligado a escribir un comentario explicando *cómo* funciona un bloque específico, significa que el código en sí es demasiado complejo o tiene malos nombres. La solución no es agregar un comentario, sino refactorizar el código, generalmente extrayendo métodos más pequeños y bien nombrados que se expliquen por sí mismos. Además, los comentarios no son ejecutables y a menudo se desincronizan del código real, convirtiéndose en "mentiras" engañosas. En última instancia, Bugayenko aboga por maximizar la documentación arquitectónica mientras se reduce la densidad de comentarios en línea a cero absoluto.

## Ideas Clave
- "Los comentarios en línea son un mal síntoma; si tienes que explicar cómo funciona tu código, deberías refactorizarlo."
- "Existe una diferencia estricta entre la documentación de la API (el contrato) y los comentarios internos (la implementación)."
- "El código nunca miente, pero los comentarios se desactualizan fácilmente y se convierten en mentiras que confunden a futuros desarrolladores."
- "Un código de alta calidad maximiza la densidad de la documentación de la API mientras mantiene la densidad de comentarios en línea en cero."

## Relevancia: 5/5
Este tema es altamente relevante para ingenieros de software y líderes de equipo, ya que establece reglas claras para el mantenimiento del código, la refactorización y las prácticas de documentación en la programación orientada a objetos.
