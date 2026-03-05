---
title: "El dolor de la POO, Lección #8: Herencia"
date: 2023-08-22T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
  - "oop"
  - "ai"
cover:
  image: "https://img.youtube.com/vi/m0OEOoGgIuM/maxresdefault.jpg"
  alt: "El dolor de la POO, Lección #8: Herencia"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=m0OEOoGgIuM](https://www.youtube.com/watch?v=m0OEOoGgIuM)

## Resumen
En esta lección, Yegor Bugayenko analiza uno de los temas más controvertidos de la Programación Orientada a Objetos: la herencia. Establece una distinción tajante entre el "subtipado" (interfaces) y la "herencia de implementación" (la palabra clave `extends`). Mientras que el subtipado es elogiado como la base del polimorfismo y del Principio de Sustitución de Liskov (LSP), la herencia de implementación es condenada como un "truco" procedimental para la reutilización de código que destruye el encapsulamiento.

Bugayenko argumenta que la herencia crea un acoplamiento fuerte entre un padre y sus hijos, lo que conduce al problema de la "Clase Base Frágil", donde los cambios en una clase base rompen inesperadamente las subclases. Critica el uso de modificadores `protected`, afirmando que violan el principio de "caja negra" de los objetos. La lección también toca las trampas de la sobrecarga de métodos y la herencia múltiple. Como solución, aboga por la "Composición sobre la Herencia", sugiriendo que los objetos deben encapsular y delegar el comportamiento en lugar de heredarlo. Este enfoque da como resultado bases de código más pequeñas, mantenibles y desacopladas.

## Ideas Clave
- "La herencia de implementación no se trata de pensamiento orientado a objetos; es un atajo procedimental para la reutilización perezosa de código."
- "En el momento en que usas el modificador `protected`, has admitido que tu encapsulamiento está roto."
- "Los objetos deben ser unidades de comportamiento independientes, no bolsas de datos con detalles de implementación compartidos."
- "Un verdadero arquitecto de POO usa interfaces para definir tipos y composición para reutilizar la lógica."

## Relevancia: 5/5
Esta lección es muy relevante, ya que desafía las prácticas estándar de la industria y profundiza en principios arquitectónicos que impactan directamente en la mantenibilidad y escalabilidad del software.
