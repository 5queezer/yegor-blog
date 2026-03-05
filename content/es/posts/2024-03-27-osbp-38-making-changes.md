---
title: "OSBP 3/8: Realizando Cambios"
date: 2024-03-27T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/D6CUW9eZ5yk/maxresdefault.jpg"
  alt: "OSBP 3/8: Realizando Cambios"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=D6CUW9eZ5yk](https://www.youtube.com/watch?v=D6CUW9eZ5yk)

## Resumen
En la octava entrega de su serie "Open Source Best Practices", Yegor Bugayenko analiza a fondo la dinámica técnica y psicológica de contribuir código mediante Pull Requests (PR). Bugayenko propone un cambio de paradigma: ver cada PR como una transacción comercial. En este modelo, el programador actúa como un vendedor que ofrece su "mercancía" (el código), mientras que el mantenedor del repositorio es el cliente que decide si la "compra". Para que esta transacción sea exitosa, el colaborador debe reducir al máximo el esfuerzo y la carga cognitiva del revisor. El consejo fundamental es mantener los PR extremadamente pequeños. Según el autor, una sola línea de cambio suele ser procesada mucho más rápido que un bloque de 500 líneas, ya que las contribuciones voluminosas generan fatiga mental y dudas sobre posibles errores ocultos, lo que posterga su integración indefinidamente.

Otro pilar de su filosofía es la gestión de la atomicidad: cada PR debe resolver un único problema o implementar una sola funcionalidad aislada. Agrupar varias tareas en una sola propuesta es un error estratégico; si el mantenedor objeta una parte mínima, todo el trabajo queda bloqueado. Además, sostiene que el colaborador debe actuar como el "jefe" o líder de su propia propuesta. Esto implica asumir la responsabilidad total del ciclo de vida del cambio: desde asegurar que pase todas las pruebas de integración continua (CI) hasta gestionar las críticas sobre el estilo o la arquitectura sin tomarlas como algo personal. En la descripción del cambio, se debe priorizar el "por qué" (la motivación y el valor aportado) por encima del "qué" (los detalles técnicos ya visibles en el diff). Bugayenko respalda estas prácticas citando investigaciones académicas de expertos como Bram Adams, Caitlin Sadowski y Marco Ortu, demostrando que la velocidad de fusión del código y la retención de desarrolladores dependen directamente de la gestión del tamaño de los PR y del tono emocional de las interacciones durante el proceso de revisión por pares.

## Ideas Clave
- "Un Pull Request es una transacción. Tú eres el vendedor, el mantenedor es el cliente".
- "Los PR pequeños se integran mucho más rápido. Incluso un PR de una sola línea es perfecto".
- "Tú eres el líder de la transacción. Si el PR no se fusiona, es tu responsabilidad".
- "Explica el 'Por qué', no el 'Qué'. El código por sí solo muestra lo que se cambió".

## Relevancia: 5/5
Vital para la cultura de ingeniería de software moderna, especialmente en entornos de desarrollo distribuido y revisión por pares.
