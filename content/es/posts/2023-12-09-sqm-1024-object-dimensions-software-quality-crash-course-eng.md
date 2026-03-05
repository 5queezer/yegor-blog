---
title: "SQM 10/24: Dimensiones de los Objetos [Curso de calidad de software]"
date: 2023-12-09T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
  - "oop"
cover:
  image: "https://img.youtube.com/vi/jdEFoz-OQ44/maxresdefault.jpg"
  alt: "SQM 10/24: Dimensiones de los Objetos [Curso de calidad de software]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=jdEFoz-OQ44](https://www.youtube.com/watch?v=jdEFoz-OQ44)

## Resumen
En esta sesión, Yegor Bugayenko analiza las "dimensiones" de la calidad del software a través de métricas cuantitativas, alejándose del simple conteo de líneas de código. Se centra en los conjuntos de métricas MOOD (Metrics for Object-Oriented Design) y C&K (Chidamber & Kemerer), explicando cómo medir la Encapsulación, Herencia, Polimorfismo y Complejidad.

Bugayenko destaca que la encapsulación se mide mediante factores de ocultación (MHF y AHF). Un diseño robusto debe tener un AHF cercano a 1, lo que significa que los atributos son privados; lo contrario indica un diseño procedural disfrazado de objetos. En cuanto a la herencia (MIF/AIF), explica que es una herramienta para la reutilización, pero advierte sobre el riesgo de las "clases base frágiles" cuando los factores son excesivamente altos.

También se discuten métricas estructurales como la Profundidad del Árbol de Herencia (DIT) y el Número de Hijos (NOC). Estas métricas permiten identificar clases críticas que, de cambiar, podrían romper gran parte del sistema. Finalmente, se introduce la Respuesta por Clase (RFC) como un indicador clave de acoplamiento: cuantas más respuestas (métodos ejecutables) tenga una clase, más difícil será de depurar y mantener.

## Ideas Clave
- "Las líneas de código son una métrica pobre; la calidad real se mide en los ratios de encapsulación y herencia."
- "Si el factor de ocultación de atributos (AHF) es bajo, no estás haciendo OOP, solo programación procedural con estructuras de datos."
- "La herencia es un arma de doble filo: facilita la reutilización pero puede hacer que el sistema sea rígido y difícil de modificar."
- "El RFC (Respuesta por Clase) es el mejor indicador de complejidad; una clase que 'sabe' demasiado es un foco de errores."

## Relevancia: 5/5
Fundamental para arquitectos de software que buscan formalizar la revisión de código mediante análisis estático y métricas objetivas.
