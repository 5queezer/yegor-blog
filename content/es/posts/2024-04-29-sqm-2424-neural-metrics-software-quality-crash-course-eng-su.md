---
title: "SQM 24/24: Métricas Neuronales [Curso intensivo de calidad de software]"
date: 2024-04-29T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/6Rog8QhuXTY/maxresdefault.jpg"
  alt: "SQM 24/24: Métricas Neuronales [Curso intensivo de calidad de software]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=6Rog8QhuXTY](https://www.youtube.com/watch?v=6Rog8QhuXTY)

## Resumen
En la vigésima cuarta y última sesión de su curso sobre métricas de calidad de software, Yegor Bugayenko analiza la evolución desde las métricas deterministas (como las líneas de código o la complejidad ciclomática) hacia las "Métricas Neuronales". Estas nuevas herramientas utilizan el aprendizaje automático y los LLM para identificar patrones de calidad que las reglas humanas suelen pasar por alto.

La lección profundiza en el "Análisis Neuronal de Software", explorando cómo se entrenan los modelos para detectar "code smells" y "clones semánticos" basándose en repositorios masivos. Bugayenko destaca proyectos como "DeepBugs", que utiliza el contexto semántico para hallar errores en nombres de variables o argumentos intercambiados, y "code2vec", que representa el código como vectores matemáticos a través de rutas en el Árbol de Sintaxis Abstracta (AST). Finalmente, se discute el papel de los LLM (como ChatGPT) no para reemplazar el análisis estático, sino para actuar como un filtro inteligente que reduce el ruido de los falsos positivos, ayudando a los ingenieros a centrarse en problemas reales.

## Ideas Clave
- **De Reglas a Patrones:** La transición implica dejar de usar fórmulas rígidas para adoptar un reconocimiento de patrones que entiende la "intención" del código.
- **Dependencia de los Datos:** La eficacia de una métrica neuronal depende de la "Verdad Fundamental" (Ground Truth) de sus datos de entrenamiento; si el entrenamiento es deficiente, la métrica fallará.
- **Precisión vs. Explicabilidad:** Aunque los modelos neuronales son más precisos para predecir errores, carecen de la transparencia de las métricas tradicionales.
- **El LLM como Asistente:** Los modelos de lenguaje actuales son excelentes para explicar advertencias de análisis estático y descartar aquellas que no son críticas.

## Relevancia: 5/5
Muy alta para profesionales interesados en la intersección entre la Inteligencia Artificial y la ingeniería de software moderna.
