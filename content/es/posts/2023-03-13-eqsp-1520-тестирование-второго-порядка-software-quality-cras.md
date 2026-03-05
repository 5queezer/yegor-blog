---
title: "EQSP 15/20: Pruebas de segundo orden [curso intensivo de calidad de software]"
date: 2023-03-13T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
  - "testing"
cover:
  image: "https://img.youtube.com/vi/O6cl3X8gOzs/maxresdefault.jpg"
  alt: "EQSP 15/20: Pruebas de segundo orden [curso intensivo de calidad de software]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=O6cl3X8gOzs](https://www.youtube.com/watch?v=O6cl3X8gOzs)

## Resumen
En esta lección de su curso sobre calidad de software, Yegor Bugayenko presenta el concepto de "Pruebas de Segundo Orden". Mientras que las pruebas tradicionales (primer orden) verifican si el código funciona, las de segundo orden se encargan de verificar la calidad y eficacia de las propias pruebas. La premisa es simple: si no probamos nuestros tests, no podemos confiar en los resultados que nos entregan.

Yegor describe varios mecanismos clave para implementar este control. Primero, propone un "Control de Cobertura" extremo: la compilación (build) debe fallar automáticamente si el porcentaje de cobertura de código disminuye, aunque sea un 0.1%. Esto garantiza que cada nueva funcionalidad esté respaldada por pruebas. En segundo lugar, destaca las "Pruebas de Mutación" como la herramienta definitiva. Mediante el uso de herramientas como PITest, se introducen errores deliberados en el código fuente; si las pruebas no fallan ante estos cambios, significa que los tests son inútiles o superficiales.

La lección también aborda las "Pruebas Estructurales" para validar reglas arquitectónicas (por ejemplo, asegurar que todas las clases sean `final` mediante ArchUnit) y las "Pruebas basadas en Propiedades" (Property-based Testing) para descubrir casos borde usando datos aleatorios. Finalmente, insiste en la higiene de las pruebas: un test nunca debe depender de recursos externos como internet o bases de datos globales, ya que esto introduce indeterminismo. El objetivo final es convertir la garantía de calidad en un proceso riguroso, matemático y completamente automatizado que no dependa del juicio subjetivo del programador.

## Ideas Clave
1. "Las pruebas de segundo orden responden a la pregunta: '¿Qué tan buenos son nuestros tests?'"
2. "Las pruebas de mutación son la única forma de demostrar matemáticamente que un test realmente está verificando la lógica."
3. "El build debe fallar si la cobertura baja un 0.1%; la cobertura es un mecanismo que solo debe subir o mantenerse."
4. "Un test que depende de internet no es un test; es una lotería que acabará destruyendo la confianza en tu CI."

## Relevancia: 5/5
Muy alta para ingenieros de software y líderes técnicos. Proporciona una visión avanzada y herramientas prácticas para elevar el estándar de calidad en proyectos complejos de forma objetiva.
