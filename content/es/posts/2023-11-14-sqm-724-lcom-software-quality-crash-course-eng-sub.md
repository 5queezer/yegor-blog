---
title: "SQM 7/24: LCOM [curso intensivo de calidad de software]"
date: 2023-11-14T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/74YigDo8_BE/maxresdefault.jpg"
  alt: "SQM 7/24: LCOM [curso intensivo de calidad de software]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=74YigDo8_BE](https://www.youtube.com/watch?v=74YigDo8_BE)

## Resumen
En esta sesión, Yegor Bugayenko profundiza en el concepto de Cohesión, centrándose en la métrica LCOM (Lack of Cohesion of Methods). Comienza diferenciando entre Cohesión (la fuerza de los vínculos internos de un módulo) y Acoplamiento (la dependencia entre módulos distintos). Según Yegor, una clase con baja cohesión es como un "cajón de sastre" donde se acumula lógica no relacionada, lo que complica enormemente el mantenimiento.

La lección recorre los niveles históricos de cohesión, desde la Coincidencial (la peor) hasta la Funcional (la ideal). El núcleo técnico explica la métrica LCOM, propuesta originalmente por Chidamber y Kemerer, que cuantifica cuántos métodos de una clase NO comparten variables de instancia. Un valor de LCOM elevado es una señal de alerta de que la clase está asumiendo demasiadas responsabilidades y viola el Principio de Responsabilidad Única (SRP).

Yegor destaca la utilidad de LCOM4, una variante basada en grafos. Si el valor de LCOM4 es superior a 1, indica que la clase se puede dividir físicamente en dos o más partes independientes sin alterar la lógica. Para concluir, recomienda el uso de herramientas como "jpeek" para automatizar este análisis y evitar que los objetos se conviertan en "God Objects".

## Ideas Clave
- "La cohesión es el pegamento que mantiene unida la lógica interna; si el pegamento falla, el módulo carece de sentido."
- "LCOM4 es una prueba irrefutable: si es mayor que 1, tu clase es en realidad un conjunto de clases fragmentadas."
- "Una alta cohesión es la principal defensa contra los 'God Objects' y el código espagueti."
- "Las métricas de calidad no son opcionales si se quiere gestionar la deuda técnica de forma profesional."

## Relevancia: 5/5
Fundamental para arquitectos de software y desarrolladores senior que buscan profesionalizar su enfoque hacia el diseño orientado a objetos.
