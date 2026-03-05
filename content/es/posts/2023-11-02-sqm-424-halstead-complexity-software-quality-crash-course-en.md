---
title: "SQM 4/24: Complejidad de Halstead [curso intensivo de calidad de software]"
date: 2023-11-02T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/YsGzjv0hgcc/maxresdefault.jpg"
  alt: "SQM 4/24: Complejidad de Halstead [curso intensivo de calidad de software]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=YsGzjv0hgcc](https://www.youtube.com/watch?v=YsGzjv0hgcc)

## Resumen
En esta lección, Yegor Bugayenko explora el concepto de **Complejidad de Halstead**, una métrica fundamental en la "Ciencia del Software" introducida por Maurice Halstead en 1977. A diferencia de la Complejidad Ciclomática, que se centra en el flujo de control y las ramificaciones, el enfoque de Halstead se basa en contar los componentes básicos del código: **operadores** (palabras clave, símbolos, llamadas a funciones) y **operandos** (variables, constantes).

La clase detalla las cuatro métricas básicas: operadores distintos ($n_1$), operandos distintos ($n_2$), operadores totales ($N_1$) y operandos totales ($N_2$). A partir de estos, se derivan indicadores más complejos, principalmente el **Volumen ($V$)**, la **Dificultad ($D$)** y el **Esfuerzo ($E$)**. Bugayenko enfatiza que el **Esfuerzo ($E = D \times V$)** es la conclusión más crítica para los ingenieros de software, ya que intenta cuantificar la energía mental y el tiempo necesarios para que una persona comprenda o implemente un algoritmo específico.

Yegor enmarca estas métricas dentro del contexto de la mantenibilidad y el "costo del código". Sostiene que, aunque el trabajo de Halstead tiene décadas de antigüedad, proporciona un marco matemático riguroso para entender por qué el código "denso" es más difícil de mantener. Al medir el vocabulario y la densidad de un programa, los equipos pueden identificar módulos que requieren un alto esfuerzo y que probablemente se conviertan en cuellos de botella para el desarrollo futuro.

## Ideas Clave
* **El código como información:** Programar no es solo lógica; es densidad de información. Las métricas de Halstead tratan el código como un flujo de símbolos que el cerebro humano debe procesar.
* **La métrica de "Esfuerzo":** El aspecto más valioso de la teoría de Halstead es la cuantificación del "esfuerzo mental", que se correlaciona directamente con el tiempo dedicado por un desarrollador.
* **Volumen vs. Dificultad:** Un programa puede tener un volumen pequeño pero una dificultad alta si utiliza una gran variedad de operadores de forma compleja, lo que lo hace más difícil de leer que un código más largo pero simple.
* **Fundamentación Científica:** Halstead intentó convertir la ingeniería de software en una "ciencia exacta" aplicando la teoría de la información al código fuente.

## Relevancia: 4/5
Extremadamente relevante para comprender los costos de mantenimiento y el aspecto psicológico de la legibilidad del código en el desarrollo profesional.
