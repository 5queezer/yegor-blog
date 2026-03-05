---
title: "SQM 5/24: Índice de Mantenibilidad"
date: 2023-11-06T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
  - "ai"
cover:
  image: "https://img.youtube.com/vi/xnSnPfVkmkM/maxresdefault.jpg"
  alt: "SQM 5/24: Índice de Mantenibilidad"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=xnSnPfVkmkM](https://www.youtube.com/watch?v=xnSnPfVkmkM)

## Resumen
En esta lección de la serie Software Quality Management (SQM), Yegor Bugayenko analiza el **Índice de Mantenibilidad (MI)**, una métrica diseñada para cuantificar qué tan fácil es mantener y evolucionar un sistema de software. La sesión comienza fundamentando el tema en las teorías de Fred Brooks (complejidad esencial vs. accidental) y el concepto de deuda técnica de Ward Cunningham. Bugayenko explica que el MI fue desarrollado a principios de los años 90 por Paul Oman y Jack Hagemeister para trasladar la evaluación de software de "sentimientos" subjetivos a datos objetivos.

La fórmula original del MI es un cálculo polinómico que involucra tres variables clave: el **Volumen de Halstead** (contenido de información), la **Complejidad Ciclomática de McCabe** (rutas lógicas) y las **Líneas de Código (LOC)**. Bugayenko destaca cómo Microsoft popularizó una versión normalizada de este índice (de 0 a 100) en Visual Studio. Sin embargo, la lección toma un tono crítico al discutir investigadores como Arie van Deursen, quienes sostienen que el MI puede ser "dañino". Debido a que la métrica depende mucho de las líneas de código, es fácil de "manipular"; por ejemplo, eliminando comentarios para inflar la puntuación sin mejorar realmente la calidad o legibilidad. Bugayenko sugiere usar el MI como una "prueba de humo": puede señalar que algo anda mal, pero no debe ser el único juez de la salud arquitectónica.

## Ideas Clave
*   "El Índice de Mantenibilidad es un intento de reducir la sensación humana de 'código desordenado' a un único número matemático objetivo".
*   "Como el MI depende tanto de las líneas de código, es fácil 'engañar' a la métrica sin mejorar realmente el software".
*   "Use el Índice de Mantenibilidad como una 'prueba de humo': puede decirte que hay fuego, pero no que la casa esté perfectamente construida".

## Relevancia: 4/5
Esta lección es muy relevante para líderes de equipo y arquitectos que necesitan medir la deuda técnica pero deben comprender las limitaciones de las métricas de calidad automáticas.
