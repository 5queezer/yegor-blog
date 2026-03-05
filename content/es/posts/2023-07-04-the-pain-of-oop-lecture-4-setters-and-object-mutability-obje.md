---
title: "El Dolor de la POO Lección #4: Setters y mutabilidad de objetos"
date: 2023-07-04T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
  - "oop"
  - "ai"
cover:
  image: "https://img.youtube.com/vi/h0jf9E1tjf4/maxresdefault.jpg"
  alt: "El Dolor de la POO Lección #4: Setters y mutabilidad de objetos"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=h0jf9E1tjf4](https://www.youtube.com/watch?v=h0jf9E1tjf4)

## Resumen
En la cuarta lección de la serie "The Pain of OOP", Yegor Bugayenko lanza una crítica mordaz al uso de setters y al concepto de mutabilidad de objetos. Su argumento central es que los setters transforman los objetos en simples "bolsas de datos" pasivas, despojándolos de su autonomía y violando el principio fundamental de encapsulación. En la programación pura orientada a objetos, un objeto debe ser una entidad autosuficiente que gestione su propio estado y lógica. Al usar setters, permitimos que procedimientos externos manipulen las partes internas del objeto, lo que convierte de hecho el código orientado a objetos en código procedimental donde la lógica está dispersa por toda la aplicación.

Yegor destaca tres problemas críticos causados por la mutabilidad. Primero, la pérdida de identidad: si los campos de un objeto cambian constantemente, resulta difícil asegurar que represente la misma entidad de negocio. Segundo, la inmensa dificultad en la depuración, ya que el estado de un objeto puede alterarse en cualquier momento desde cualquier parte del programa, dificultando el rastreo del origen de los errores. Tercero, la falta de seguridad de hilos inherente; los objetos mutables requieren complejos mecanismos de bloqueo en entornos multihilo. La única solución arquitectónicamente sólida propuesta es la inmutabilidad total. Los objetos deben recibir todos los datos necesarios a través del constructor, y cualquier "cambio" debe dar lugar a la creación de una nueva instancia. Este enfoque hace que el software sea predecible, simplifica las pruebas y obliga a los desarrolladores a pensar en términos de comportamientos del mundo real en lugar de manipulaciones técnicas de campos.

## Ideas Clave
1. "Los setters convierten a los objetos en simples bolsas de datos."
2. "Un objeto debe ser una entidad viva, no un contenedor pasivo."
3. "La mutabilidad es la principal fuente de problemas y errores en la arquitectura de software."
4. "En un mundo verdaderamente orientado a objetos, todos los objetos deberían ser inmutables por defecto."

## Relevancia: 5/5
Esta lección es fundamental para entender la filosofía de "Elegant Objects". Desafía los estándares tradicionales de la industria (como Java Beans) y ofrece un enfoque radical para construir sistemas mantenibles.
