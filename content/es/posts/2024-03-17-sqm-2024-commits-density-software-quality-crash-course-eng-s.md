---
title: "SQM 20/24: Densidad de Commits"
date: 2024-03-17T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/BrG3HiuYC5U/maxresdefault.jpg"
  alt: "SQM 20/24: Densidad de Commits"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=BrG3HiuYC5U](https://www.youtube.com/watch?v=BrG3HiuYC5U)

## Resumen
En esta clase del curso de Métricas de Calidad de Software (SQM), Yegor Bugayenko explora el concepto de "Densidad de Commits" como una métrica crucial para evaluar la disciplina en el desarrollo de software. Define esta métrica de dos maneras: densidad temporal (commits por día) y densidad estructural (commits por cada mil líneas de código alterado). Bugayenko argumenta que una mayor densidad de commits se correlaciona directamente con una mayor calidad del software.

En lugar de realizar cambios masivos y de golpe ("big bang"), los desarrolladores deben dividir su trabajo en commits pequeños y frecuentes. Este enfoque ofrece varias ventajas importantes. En primer lugar, mejora significativamente la trazabilidad, lo que facilita descubrir exactamente cuándo y por qué se introdujo un error utilizando herramientas como `git bisect`. En segundo lugar, los cambios más pequeños son mucho más fáciles de revisar a fondo por otros compañeros. Los commits grandes a menudo agrupan cambios no relacionados, abrumando a los revisores y haciendo que las reversiones (rollbacks) parciales sean casi imposibles. Bugayenko enfatiza que los commits frecuentes son la base de una Integración Continua (CI) efectiva, asegurando que el código permanezca estable y minimizando los conflictos de fusión.

## Ideas Clave
- "Una mayor densidad de commits es un indicador directo de una fuerte disciplina de ingeniería y produce una mayor calidad de código."
- "Los commits pequeños y frecuentes hacen que las revisiones de código sean útiles y evitan la fusión de defectos ocultos."
- "Los commits masivos son muy arriesgados; agrupan cambios no relacionados y hacen imposibles las reversiones parciales."
- "La integración frecuente reduce los conflictos de fusión y mantiene el proyecto en un estado continuo de preparación."

## Relevancia: 5/5
Extremadamente relevante para la ingeniería de software y la gestión de equipos. Enfatiza la disciplina práctica de control de versiones, impactando directamente en la calidad de la revisión de código, la efectividad de CI/CD y la mantenibilidad general del proyecto.
