---
title: "SQM 2/24: Complejidad Ciclomática de Thomas J. McCabe"
date: 2023-09-30T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/Cvv0Olx4Bpw/maxresdefault.jpg"
  alt: "SQM 2/24: Complejidad Ciclomática de Thomas J. McCabe"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=Cvv0Olx4Bpw](https://www.youtube.com/watch?v=Cvv0Olx4Bpw)

## Resumen
Yegor Bugayenko ofrece una lección profunda sobre el trabajo fundamental de Thomas J. McCabe de 1976 respecto a la Complejidad Ciclomática (CC). Presenta la complejidad no como un simple efecto secundario técnico, sino como una elección deliberada que refleja la profesionalidad del desarrollador y su respeto por quienes leerán el código después. Utilizando la "métrica del dolor de ojos" como punto de partida, Yegor argumenta que si el código es difícil de comprender, es intrínsecamente arriesgado y costoso de mantener. La CC se define técnicamente como el número de caminos linealmente independientes a través del flujo de control de un programa, calculado mediante la fórmula $V(G) = E - N + 2$.

Una parte significativa de la charla aborda la tensión entre la CC y las líneas de código (LoC). Aunque ambas métricas suelen estar correlacionadas, Yegor destaca que la CC se enfoca específicamente en la densidad lógica. Cita evidencia de que una CC elevada es un indicador principal de la densidad de defectos y de la dificultad para realizar pruebas. Siguiendo las directrices originales de McCabe, aboga por un umbral estricto (generalmente de 10), por encima del cual las funciones deben ser refactorizadas. La conclusión más práctica es la vinculación directa con las pruebas: el valor de la CC es igual al número mínimo de casos de prueba necesarios para lograr una cobertura completa de las ramas. Yegor concluye que la "buena" ingeniería de software es el arte de resolver requisitos complejos con código simple y de baja complejidad, apoyándose en controles de calidad automatizados en CI/CD para evitar la deuda técnica.

## Ideas Clave
* "La complejidad es una elección que hace el programador; no es algo impuesto por los requisitos".
* "La complejidad ciclomática representa el número mínimo de pruebas que debes escribir para cubrir todos los caminos".
* "Escribir código complejo es una falta de respeto hacia los futuros mantenedores y el equipo".
* "La fórmula $V(G) = E - N + 2$ es una forma matemática de cuantificar el riesgo y la mantenibilidad".

## Relevancia: 5/5
La complejidad ciclomática es una piedra angular de las métricas de calidad de software modernas, esencial para la estrategia de pruebas y el diseño orientado a objetos.
