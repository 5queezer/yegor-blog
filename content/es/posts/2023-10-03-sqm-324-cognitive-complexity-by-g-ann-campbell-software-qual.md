---
title: "SQM 3/24: Complejidad Cognitiva por G. Ann Campbell [curso intensivo de calidad de software]"
date: 2023-10-03T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/oRUux3w4rsc/maxresdefault.jpg"
  alt: "SQM 3/24: Complejidad Cognitiva por G. Ann Campbell [curso intensivo de calidad de software]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=oRUux3w4rsc](https://www.youtube.com/watch?v=oRUux3w4rsc)

## Resumen
En esta lección de su serie sobre métricas de calidad de software, Yegor Bugayenko analiza las limitaciones de la complejidad ciclomática (CC) tradicional y presenta la complejidad cognitiva (CoCo) como una alternativa más orientada al ser humano. El argumento central es que, aunque la CC de Thomas McCabe es un modelo matemático sólido para medir la testabilidad, no refleja fielmente la dificultad que tiene un desarrollador para comprender y mantener el código.

Bugayenko detalla las tres reglas fundamentales de la complejidad cognitiva propuestas por G. Ann Campbell de SonarSource. Primero, se ignora el "azúcar sintáctico": las características modernas del lenguaje que condensan la lógica sin añadir carga mental. Segundo, se incrementa la puntuación por cada ruptura en el flujo lineal de ejecución (como sentencias `if`, `for` o `catch`). Tercero, y más crítico, se aplica una "penalización por anidamiento". A diferencia de la CC, la CoCo aumenta el peso de una instrucción según su profundidad. Un `if` anidado en tres niveles es mucho más "costoso" que uno en el nivel superior, reflejando el esfuerzo mental necesario para rastrear el estado.

La lección también explora la validación científica de estas métricas. Yegor menciona el uso de cascos de EEG para medir la actividad cerebral real al leer código, demostrando que el anidamiento correlaciona con una mayor carga cognitiva. Finalmente, aborda el "análisis social de código", enfatizando que una métrica útil debe predecir resultados del mundo real, como la frecuencia de errores y la facilidad con la que un nuevo miembro del equipo puede entender el sistema.

## Ideas Clave
- "La complejidad ciclomática mide el esfuerzo de prueba, mientras que la complejidad cognitiva mide el esfuerzo de comprensión."
- "El anidamiento es el principal enemigo de la legibilidad; cada nivel de indentación añade una capa de estado mental que el desarrollador debe mantener."
- "Las métricas modernas deben validarse biológicamente, utilizando herramientas como el EEG para confirmar qué estructuras agotan realmente el cerebro."
- "Una buena métrica funciona como una herramienta predictiva para la gestión de equipos, identificando qué módulos serán más propensos a errores en el futuro."

## Relevancia: 5/5
Fundamental para ingenieros de software y líderes técnicos que buscan reducir la carga cognitiva de sus equipos y mejorar la mantenibilidad a largo plazo.
