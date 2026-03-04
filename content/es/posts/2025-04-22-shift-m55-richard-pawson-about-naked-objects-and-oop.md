---
title: "Shift-M/55: Richard Pawson sobre Naked Objects y OOP"
date: 2025-04-22T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
  - "oop"
cover:
  image: "https://img.youtube.com/vi/x6LKw-iQHZQ/maxresdefault.jpg"
  alt: "Shift-M/55: Richard Pawson sobre Naked Objects y OOP"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=x6LKw-iQHZQ](https://www.youtube.com/watch?v=x6LKw-iQHZQ)

## Resumen
En esta entrevista del podcast Shift-M, Yegor Bugayenko conversa con Richard Pawson, creador del patrón arquitectónico "Naked Objects" (Objetos Desnudos). La charla explora la esencia de la programación orientada a objetos (OOP) y cómo el patrón de Pawson busca restaurar sus principios originales. Naked Objects se basa en encapsular toda la lógica de negocio en los objetos de dominio, permitiendo que la interfaz de usuario (UI) se genere automáticamente a partir de ellos, ofreciendo una representación directa 1:1 al usuario.

Pawson destaca que su enfoque no busca la escalabilidad de rendimiento (como el tráfico web masivo), sino la escalabilidad de la complejidad. Pone como ejemplo un sistema gubernamental en Irlanda con más de 5,000 clases de dominio, donde la automatización de la UI permitió manejar reglas de negocio extremadamente complejas que de otro modo habrían sido inmanejables.

El autor critica el estado actual de la OOP, donde los desarrolladores suelen usar objetos solo como estructuras de datos pasivas (DTOs) manipuladas por servicios externos. Pawson aboga por objetos "ricos" en comportamiento, similares a la visión original de Smalltalk. Finalmente, diferencia entre aplicaciones "Soberanas" (herramientas internas para expertos) y "Transitorias" (sitios web de consumo), señalando que Naked Objects brilla especialmente en las primeras.

## Ideas Clave
- "Naked Objects no se trata de simplificar el código, sino de permitir que la arquitectura escale frente a una complejidad de negocio masiva."
- "Debemos tratar al usuario como un profesional capaz de manipular objetos directamente, no como alguien que solo sigue pasos en un asistente."
- "La UI generada automáticamente elimina la necesidad de capas de traducción que suelen corromper el modelo de dominio."
- "El objetivo es que el software hable el mismo lenguaje que el experto en el negocio, sin intermediarios técnicos innecesarios."

## Relevancia: 5/5
Es una pieza fundamental para entender arquitecturas alternativas al MVC tradicional, especialmente útil para quienes diseñan sistemas empresariales complejos y buscan maximizar la cohesión del modelo.
