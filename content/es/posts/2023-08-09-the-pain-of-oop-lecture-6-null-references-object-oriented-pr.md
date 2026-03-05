---
title: "El dolor de la POO, Lección #6: Referencias NULL"
date: 2023-08-09T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
  - "oop"
  - "ai"
cover:
  image: "https://img.youtube.com/vi/cTyIF20Kmz4/maxresdefault.jpg"
  alt: "El dolor de la POO, Lección #6: Referencias NULL"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=cTyIF20Kmz4](https://www.youtube.com/watch?v=cTyIF20Kmz4)

## Resumen
En esta lección, Yegor Bugayenko analiza el impacto negativo de las referencias NULL en la programación orientada a objetos, calificándolas como el "error de los mil millones de dólares". Sostiene que NULL es un vestigio de la programación procedimental que trata a los objetos como simples punteros de memoria en lugar de entidades autónomas con comportamiento. Para Yegor, cuando un método devuelve NULL, rompe el contrato con el cliente y lo obliga a practicar la "programación defensiva", saturando el código con validaciones `if (x != null)`.

El problema fundamental es que NULL no es un objeto; carece de comportamiento y no puede responder a mensajes. Esto rompe el polimorfismo y provoca que la encapsulación se debilite, ya que la lógica para manejar la "ausencia de datos" se traslada al usuario del objeto. Yegor propone el principio "Fail Fast" (fallar rápido): si un objeto no puede cumplir su función, debe lanzar una excepción de inmediato o devolver un "Objeto Nulo" (una implementación de la interfaz que no hace nada). Su postura es radical: un diseño puro de POO nunca debe aceptar ni devolver NULL.

## Ideas Clave
- NULL no es un objeto; es un puntero técnico que no pertenece al modelo conceptual de la POO.
- Cada comprobación de NULL es un síntoma de un fallo arquitectónico y una violación del principio "Tell, Don't Ask".
- Devolver NULL es una traición al contrato del método, delegando la gestión de errores al llamador de forma inapropiada.
- El uso del patrón Null Object o el lanzamiento de excepciones mantiene el código declarativo y robusto.

## Relevancia: 5/5
Es una lección crítica para desarrolladores que buscan profesionalizar su diseño de software y eliminar la fuente principal de errores en tiempo de ejecución.
