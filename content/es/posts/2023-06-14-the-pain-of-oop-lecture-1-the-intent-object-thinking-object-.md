---
title: "El dolor de la POO Lección #1: El pensamiento de objeto de intención"
date: 2023-06-14T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
  - "oop"
  - "ai"
cover:
  image: "https://img.youtube.com/vi/8FPU_N3LxqA/maxresdefault.jpg"
  alt: "El dolor de la POO Lección #1: El pensamiento de objeto de intención"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=8FPU_N3LxqA](https://www.youtube.com/watch?v=8FPU_N3LxqA)

## Resumen
Yegor Bugayenko sostiene que la Programación Orientada a Objetos (POO) actual es una desviación "monstruosa" de su propósito original, resultando a menudo en sistemas más complejos que el código procedimental tradicional. La tesis principal es que los programadores han fallado en adoptar el "pensamiento de objetos", prefiriendo en su lugar el "pensamiento algorítmico" envuelto en clases.

Para Yegor, un objeto debe ser una abstracción de una entidad real que oculta sus datos y solo expone comportamiento. Critica duramente el uso de métodos estáticos, "getters" y "setters", argumentando que estos rompen la encapsulación al permitir que los datos escapen del objeto. La lección propone que los objetos deben ser tratados como organismos vivos y autosuficientes. En lugar de extraer datos de un objeto para procesarlos externamente (enfoque algorítmico), debemos pedirle al objeto que realice la acción por sí mismo (enfoque declarativo). El objetivo final es construir sistemas mediante la composición de objetos pequeños y atómicos que se comunican entre sí, eliminando la necesidad de lógica centralizada y compleja.

## Ideas Clave
1. "Un objeto es una composición de abstracciones que ocultan datos y exponen comportamiento."
2. "Los datos nunca deben escapar del objeto; los 'getters' son una señal de un diseño fallido."
3. "Debemos dejar de pensar en 'cómo' se hace algo (algoritmos) y empezar a pensar en 'qué' es el objeto (composición)."

## Relevancia: 5/5
Es fundamental para entender las críticas arquitectónicas a los marcos de trabajo modernos y mejorar la mantenibilidad del software a largo plazo.
