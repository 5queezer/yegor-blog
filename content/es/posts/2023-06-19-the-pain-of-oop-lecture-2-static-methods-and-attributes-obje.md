---
title: "El dolor de la POO Lección #2: Métodos y atributos estáticos"
date: 2023-06-19T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
  - "oop"
  - "ai"
cover:
  image: "https://img.youtube.com/vi/lELJSj9mWbI/maxresdefault.jpg"
  alt: "El dolor de la POO Lección #2: Métodos y atributos estáticos"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=lELJSj9mWbI](https://www.youtube.com/watch?v=lELJSj9mWbI)

## Resumen
En esta lección, Yegor Bugayenko presenta una crítica provocadora de los métodos y atributos estáticos, calificándolos como un "cáncer" que socava fundamentalmente la Programación Orientada a Objetos (POO). Su argumento principal es que los miembros estáticos transforman los diseños orientados a objetos en guiones procedimentales rígidos. Al vincular la lógica a una clase en lugar de a una instancia, los desarrolladores crean dependencias "acopladas" que son imposibles de interceptar, simular (mock) o reemplazar durante las pruebas unitarias sin herramientas especializadas.

Yegor distingue además entre la programación "eager" (imperativa) y "lazy" (declarativa). Sostiene que los métodos estáticos (como `Math.sqrt(x)`) son comandos imperativos que se ejecutan de inmediato, mientras que los objetos reales deberían ser representaciones declarativas de valores que realizan cálculos solo cuando es absolutamente necesario. Esta "pereza" permite una mejor composición y flexibilidad. Finalmente, ataca el concepto de "Clases de Utilidad" (por ejemplo, `StringUtils`), describiéndolas como "cubos de basura" para la lógica que carece de un hogar adecuado. Estas clases no poseen identidad y violan el Principio de Responsabilidad Única, lo que conduce a un alto acoplamiento y una baja cohesión. Para lograr una POO "pura", Yegor aboga por reemplazar cada método estático con una clase dedicada y cada atributo estático con un estado de objeto encapsulado.

## Ideas Clave
- "Los métodos estáticos son un cáncer; convierten tu código orientado a objetos en basura procedimental."
- "Un objeto debe ser un representante 'perezoso' de un resultado, no un ejecutor 'ansioso' de un comando."
- "Las clases de utilidad son solo espacios de nombres para funciones; no son objetos y no tienen lugar en una arquitectura limpia."
- "Si no puedes simularlo (mock), has fallado en la POO. Los métodos estáticos son la razón principal del código difícil de probar."

## Relevancia: 5/5
Esta lección es altamente relevante para arquitectos de software y desarrolladores que buscan comprender la filosofía de "Objetos Elegantes". Desafía las normas de la industria (como el patrón Singleton y las clases de utilidad) y proporciona un marco riguroso, aunque controvertido, para mejorar la capacidad de prueba y el mantenimiento del código.
