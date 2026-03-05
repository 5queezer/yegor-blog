---
title: "SQM 9/24: CAMC y NHD [curso intensivo de calidad de software]"
date: 2023-12-07T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/oCxJ_YSSAGo/maxresdefault.jpg"
  alt: "SQM 9/24: CAMC y NHD [curso intensivo de calidad de software]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=oCxJ_YSSAGo](https://www.youtube.com/watch?v=oCxJ_YSSAGo)

## Resumen
Yegor Bugayenko dedica esta sesión a profundizar en la cohesión de clases a través de dos métricas fundamentales: CAMC (Cohesión entre Métodos de una Clase) y NHD (Distancia de Hamming Normalizada). La charla inicia con una crítica al Rational Unified Process (RUP), destacando cómo su enfoque riguroso en la documentación y fases de elaboración contrasta con la falta de disciplina arquitectónica en algunos entornos ágiles actuales.

El punto central es el uso de matrices de parámetros para evaluar la calidad del diseño. La métrica CAMC analiza la superposición de tipos de parámetros en las firmas de los métodos; cuanto mayor es la superposición, más cohesiva se considera la clase. Por otro lado, NHD ofrece una visión más precisa al medir la "distancia" estructural entre métodos, permitiendo detectar si una clase contiene grupos de funcionalidad que no tienen relación entre sí.

Bugayenko conecta estas métricas con el Principio de Segregación de Interfaces (ISP). Utiliza la clase `InputStream` de Java como ejemplo negativo de una "interfaz gorda" que obliga a las implementaciones a cargar con métodos irrelevantes (como `mark` o `reset`), reduciendo la cohesión y aumentando la fragilidad del sistema.

## Ideas Clave
- "La cohesión no es una sensación subjetiva; se puede calcular basándose en la intersección de los tipos de datos que manejan los métodos."
- "Una interfaz gorda es un fracaso del diseño que obliga al cliente a depender de métodos que nunca utilizará."
- "NHD es superior a CAMC porque identifica agrupamientos internos, lo que nos indica exactamente por dónde dividir una clase."
- "El desacoplamiento real requiere interfaces pequeñas y específicas, no abstracciones genéricas que intentan hacerlo todo."

## Relevancia: 5/5
Fundamental para entender la aplicación práctica de SOLID y cómo usar métricas estáticas para guiar la refactorización de código.
