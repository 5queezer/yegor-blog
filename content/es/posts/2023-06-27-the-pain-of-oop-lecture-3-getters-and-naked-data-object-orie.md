---
title: "El dolor de la POO, Lección #3: Getters y datos desnudos"
date: 2023-06-27T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
  - "oop"
  - "ai"
cover:
  image: "https://img.youtube.com/vi/2YyVmIQQ23w/maxresdefault.jpg"
  alt: "El dolor de la POO, Lección #3: Getters y datos desnudos"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=2YyVmIQQ23w](https://www.youtube.com/watch?v=2YyVmIQQ23w)

## Resumen
En esta lección, Yegor Bugayenko aborda uno de los problemas más comunes en el desarrollo de software moderno: el uso de getters. Sostiene que los métodos que comienzan con `get...` transforman un objeto de ser un actor activo a un contenedor pasivo de información, o "datos desnudos". La tesis central es que la verdadera encapsulación no consiste solo en hacer que los campos sean privados, sino en ocultar la estructura misma de los datos. Si un objeto permite que sus interioridades se extraigan, deja de ser un objeto para convertirse en una estructura de datos.

Yegor critica los IDE modernos y librerías como Lombok por facilitar excesivamente la generación de getters, lo que fomenta la creación de "modelos anémicos". En estos modelos, los objetos carecen de lógica propia, obligando a que la lógica de negocio se traslade a servicios externos, lo que supone un regreso a la programación procedimental. Se centra especialmente en los Objetos de Transferencia de Datos (DTO), a los que califica como "el mal absoluto" porque fingen ser objetos sin poseer ninguna de sus cualidades reales.

La alternativa propuesta es el principio "Tell, Don't Ask" (Dile, no preguntes). En lugar de recuperar datos de un objeto para tomar una decisión externa, se debe ordenar al objeto que realice la tarea basándose en su propio estado interno. Además, Yegor argumenta en contra del prefijo `get`, que refuerza el pensamiento procedimental. Sugiere usar nombres basados en sustantivos (por ejemplo, `weight()` en lugar de `getWeight()`) para indicar una interacción con una entidad viva. La lección concluye con una crítica al framework Spring, ilustrando cómo su dependencia en "beans" y getters/setters convierte a Java en un lenguaje procedimental similar a COBOL o C.

## Ideas Clave
*   "Un getter es una forma de desnudar a un objeto y mostrar sus datos desnudos al mundo".
*   "Un objeto no es un cubo de datos; es un organismo vivo con su propio comportamiento".
*   "Los DTO son el mal absoluto en la POO porque obligan al resto del sistema a ser procedimental".
*   "La encapsulación no consiste en ocultar campos, sino en ocultar el hecho de que existen datos dentro del objeto".

## Relevancia: 5/5
Altamente relevante para ingenieros de software que deseen profundizar en el diseño orientado a objetos y evitar arquitecturas frágiles basadas en servicios externos y modelos de datos pasivos.
