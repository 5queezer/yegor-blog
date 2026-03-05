---
title: "Object Thinking Meetup #7: Nikolay Kudasov / Tipos de Datos Algebraicos"
date: 2022-09-21T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
  - "oop"
  - "ai"
cover:
  image: "https://img.youtube.com/vi/ERIDMfy4rCg/maxresdefault.jpg"
  alt: "Object Thinking Meetup #7: Nikolay Kudasov / Tipos de Datos Algebraicos"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=ERIDMfy4rCg](https://www.youtube.com/watch?v=ERIDMfy4rCg)

## Resumen
En este encuentro, Nikolay Kudasov analiza los fundamentos matemáticos y la aplicación práctica de los Tipos de Datos Algebraicos (ADTs). Explica que los ADTs se basan en dos operaciones fundamentales: los tipos Producto (clases o estructuras que combinan múltiples valores) y los tipos Suma (uniones etiquetadas que permiten elegir entre varias opciones). Kudasov destaca que, mientras los tipos Producto son comunes en la programación orientada a objetos (OOP) tradicional, los tipos Suma han sido históricamente ignorados en lenguajes como Java o C++, lo que obliga a los desarrolladores a usar patrones menos seguros como el uso de valores nulos o herencia compleja.

El punto central de la charla es cómo los ADTs permiten "hacer que los estados ilegales sean irrepresentables". Al definir estructuras de datos precisas, el compilador puede garantizar que todas las variantes de un proceso (como 'Cargando', 'Éxito' o 'Error') se manejen de forma exhaustiva mediante el ajuste de patrones (pattern matching). También se discute el "Problema de la Expresión", comparando la extensibilidad de los ADTs frente a la OOP: la OOP facilita añadir nuevos datos (subclases), mientras que los ADTs facilitan añadir nuevas operaciones sobre datos existentes. Kudasov argumenta que adoptar un enfoque algebraico reduce drásticamente los errores en tiempo de ejecución y mejora la claridad del diseño del software.

## Ideas Clave
- "El objetivo de un sistema de tipos robusto es que sea imposible representar un estado inválido en el código."
- "Los tipos Producto son una conjunción (Y), los tipos Suma son una disyunción (O). La mayoría de los bugs ocurren por usar 'Y' cuando la lógica dictaba un 'O'."
- "En OOP tradicional, simulamos los tipos Suma con herencia, pero perdemos la capacidad del compilador para verificar si hemos cubierto todos los casos posibles."
- "Los ADTs transforman la lógica de negocio en una estructura matemática que el compilador puede validar."

## Relevancia: 5/5
Fundamental para ingenieros de software. Los ADTs son la base de la seguridad de tipos moderna en lenguajes como Rust, Swift y Scala.
