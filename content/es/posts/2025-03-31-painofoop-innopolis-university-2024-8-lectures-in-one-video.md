---
title: "El Dolor de la POO, Universidad Innopolis, 2024, 8 conferencias en un video"
date: 2025-03-31T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
  - "oop"
  - "ai"
cover:
  image: "https://img.youtube.com/vi/awB08yeXfZM/maxresdefault.jpg"
  alt: "El Dolor de la POO, Universidad Innopolis, 2024, 8 conferencias en un video"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=awB08yeXfZM](https://www.youtube.com/watch?v=awB08yeXfZM)

## Resumen
El curso "Pain of OOP" (El Dolor de la POO) de Yegor Bugayenko en la Universidad Innopolis desmantela sistemáticamente las prácticas convencionales de la Programación Orientada a Objetos. Argumenta que el software empresarial moderno es, en su mayoría, programación procedimental disfrazada de POO. A lo largo de ocho exhaustivas conferencias, Bugayenko critica hábitos profundamente arraigados: el uso de getters y setters, métodos estáticos, referencias nulas y frameworks ORM. En su lugar, defiende el concepto de "Objetos Elegantes" (Elegant Objects), un paradigma mucho más estricto donde los objetos son tratados como entidades vivas y activas, y no como simples contenedores de datos pasivos.

El curso profundiza en reglas prácticas para un diseño verdaderamente orientado a objetos. Bugayenko promueve la inmutabilidad estricta, argumentando que los objetos cuyo estado cambia son inherentemente impredecibles. Exige la erradicación absoluta de la referencia `null`, recomendando el uso de "Objetos Nulos" (Null Objects). Además, los constructores deben estar completamente libres de código lógico; su único trabajo es asignar variables, retrasando cualquier computación real hasta que se invoque un método específico. La verdadera encapsulación es un tema central: Bugayenko explica que exponer el estado interno a través de DTOs (Objetos de Transferencia de Datos) destruye la cohesión del objeto.

También critica las prácticas de prueba modernas, atacando los frameworks de "mocking" y recomendando el uso de objetos "fake" que implementan las mismas interfaces. Se favorece fuertemente la composición sobre la herencia, y el uso extensivo de interfaces y decoradores se presenta como la forma correcta de extender el comportamiento. El "dolor" del título se refiere a la dificultad de desaprender estos estándares industriales tóxicos, pero la recompensa final es una arquitectura de software altamente mantenible, cohesiva y resiliente.

## Ideas Clave
- "Los getters y setters despojan a los objetos de su dignidad, convirtiéndolos en meras bolsas de datos."
- "Los métodos estáticos son un virus procedimental en el mundo orientado a objetos."
- "Los constructores deben estar libres de código; un objeto debe instanciarse rápidamente y trabajar solo cuando se llaman sus métodos."
- "Null no es un objeto; devolver o aceptar null es una violación de la confianza entre objetos."

## Relevancia: 5/5
Esta serie de conferencias es altamente relevante ya que desafía fundamentalmente las prácticas estándar de la ingeniería de software y ofrece una alternativa estricta y cohesiva para diseñar sistemas robustos orientados a objetos.
