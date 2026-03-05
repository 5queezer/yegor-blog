---
title: "SQM 1/24: Líneas de Código [Curso Intensivo de Calidad de Software]"
date: 2023-09-27T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/q9Gr2xguP5I/maxresdefault.jpg"
  alt: "SQM 1/24: Líneas de Código [Curso Intensivo de Calidad de Software]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=q9Gr2xguP5I](https://www.youtube.com/watch?v=q9Gr2xguP5I)

## Resumen
En esta lección, Yegor Bugayenko explora el papel fundamental de las métricas en la ingeniería de software, basándose en el axioma de gestión: "Solo puedes controlar lo que puedes medir". Distingue entre el "Ingeniero", que resuelve problemas aislados, y el "Científico", que busca verdades generalizables y medibles. El núcleo de la discusión se centra en las Líneas de Código (LoC). Aunque Bill Gates criticó famosamente las LoC como medida de progreso —comparándolo con medir el progreso de la construcción de un avión por su peso—, Yegor argumenta que las LoC siguen siendo una métrica vital si se ven correctamente. En lugar de progreso, las LoC deben verse como una medida de la "carga de mantenimiento" y la complejidad.

La lección introduce las "Non-Commenting Source Statements" (NCSS) para filtrar el ruido como comentarios y espacios en blanco. Sin embargo, Yegor propone una alternativa más dinámica: Hits-of-Code (HoC). A diferencia de las LoC estáticas, HoC rastrea cada modificación en Git, asegurando que la métrica siempre aumente y refleje el esfuerzo real invertido, incluso cuando se elimina código. Además, aborda los "olores de código" (code smells), señalando específicamente las líneas vacías dentro de los métodos como un signo de lógica fragmentada. Finalmente, Yegor aboga por un enfoque de "sufrimiento" en el análisis estático, donde los desarrolladores corrigen manualmente las violaciones de estilo en lugar de usar formateadores automáticos, argumentando que esta fricción es necesaria para el aprendizaje a largo plazo.

## Ideas Clave
- "Medir el progreso de la programación por líneas de código es como medir el progreso de la construcción de un avión por su peso." (Bill Gates, citado por Yegor)
- "Solo puedes controlar lo que puedes medir; sin métricas, la calidad del software es solo una opinión."
- "Hits-of-Code (HoC) es superior a LoC porque captura la historia del esfuerzo y los 'puntos calientes' de complejidad."
- "Las líneas vacías dentro de un método son un olor de código; si necesitas separar bloques de código, tu método está haciendo demasiado."

## Relevancia: 5/5
Esta lección es muy relevante para líderes de equipo y arquitectos, ya que recupera una métrica controvertida (LoC) como herramienta para la estimación de costos y la gestión del mantenimiento.
