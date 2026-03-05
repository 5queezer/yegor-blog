---
title: "SQM 13/24: Code Churn [curso intensivo de calidad de software]"
date: 2023-12-31T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/dvuyJ5LvHvQ/maxresdefault.jpg"
  alt: "SQM 13/24: Code Churn [curso intensivo de calidad de software]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=dvuyJ5LvHvQ](https://www.youtube.com/watch?v=dvuyJ5LvHvQ)

## Resumen
En esta lección, Yegor Bugayenko explora el concepto de "Code Churn" (rotación de código) como una métrica vital para la gestión de la calidad del software. A diferencia de las métricas estáticas como las Líneas de Código (LoC), que solo muestran el tamaño actual del proyecto, el Code Churn mide la dinámica evolutiva del código: cuánto se añade, elimina o modifica en un periodo determinado. Yegor sostiene que el historial de cambios es mucho más revelador que el estado actual del código.

Un tema central es la investigación de Nagappan y Ball (2005), que demuestra que el "Relative Code Churn" es un predictor superior de la densidad de defectos en comparación con las métricas tradicionales. Los archivos que sufren cambios frecuentes y masivos se identifican como "hotspots" (puntos calientes). Estas áreas tienen estadísticamente más probabilidades de contener errores, lo que a menudo indica requisitos inestables, fallos arquitectónicos o falta de comprensión del desarrollador sobre el módulo.

Yegor también presenta su propia métrica: Hits-of-Code (HoC). Critica el uso de LoC porque no valora el refactorizado; si un desarrollador elimina 1,000 líneas de código desordenado, su contribución parece negativa. El HoC, por el contrario, es la suma acumulativa de todos los cambios registrados en Git y siempre aumenta, proporcionando una representación más honesta de la productividad y el valor empresarial. La lección aboga por usar los datos de rotación para identificar riesgos de forma proactiva.

## Ideas Clave
- "La calidad no se trata solo de cómo se ve el código ahora, sino de cuánto está cambiando".
- "Hits-of-Code (HoC) le muestra a la empresa que realmente trabajaste, incluso si eliminaste más código del que añadiste".
- "Los archivos con un alto nivel de churn relativo son 'hotspots'; no necesitamos esperar a que aparezcan errores para saber que están ahí".
- "El objetivo de un gerente debería ser reducir la tasa de churn de los módulos inestables, no solo aumentar el número de funciones".

## Relevancia: 5/5
Fundamental para ingenieros y gestores que buscan métodos basados en datos para predecir fallos y gestionar el esfuerzo de desarrollo de manera justa.
