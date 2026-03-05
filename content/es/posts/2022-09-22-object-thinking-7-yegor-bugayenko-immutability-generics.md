---
title: "Pensamiento de Objetos #7: Yegor Bugayenko / Inmutabilidad + Genéricos"
date: 2022-09-22T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
  - "oop"
cover:
  image: "https://img.youtube.com/vi/C6CQWzOKEJs/maxresdefault.jpg"
  alt: "Pensamiento de Objetos #7: Yegor Bugayenko / Inmutabilidad + Genéricos"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=C6CQWzOKEJs](https://www.youtube.com/watch?v=C6CQWzOKEJs)

## Resumen
En este episodio de la serie "Object Thinking", Yegor Bugayenko discute el diseño arquitectónico de su biblioteca Java **xsline**. El núcleo del debate es cómo mantener los principios estrictos de la Programación Orientada a Objetos (POO), específicamente la **inmutabilidad** y el uso de **interfaces**, al construir sistemas complejos como tuberías (pipelines) de transformación XSL.

Yegor utiliza la metáfora de **Shift** (una transformación individual) y **Train** (el conjunto de transformaciones). Rechaza frontalmente el uso de métodos mutables como `add()`, proponiendo en su lugar el método `with()`, que devuelve una nueva instancia inmutable. Esto garantiza que los objetos no sean simples contenedores de datos, sino entidades autosuficientes y seguras para hilos (thread-safe).

El vídeo profundiza en el uso de **Genéricos** para resolver el problema de la entrada de diversos tipos de datos en una API fluida. Yegor introduce un patrón ingenioso: una interfaz `Temporary` con un método `back()`. Esto permite que un `Train<String>` (que acepta rutas de archivos) "evolucione" de nuevo a un `Train<Shift>` (el tipo base) manteniendo la seguridad de tipos. El objetivo final es lograr un código **declarativo** donde la configuración de la tubería parezca una definición estática en lugar de un procedimiento paso a paso.

## Ideas Clave
- **"Los objetos no son bolsas de datos; deben ser inmutables para ser predecibles y seguros."**
- **"Si una clase tiene métodos públicos que no están en una interfaz, estás exponiendo detalles internos y rompiendo el contrato del objeto."**
- **"Los genéricos permiten que un objeto cambie su estado de tipo durante la configuración sin perder la rigurosidad del compilador."**
- **"La programación declarativa es superior porque se enfoca en el 'qué' es el objeto, no en el 'cómo' se construye."**

## Relevancia: 5/5
Es fundamental para desarrolladores senior que buscan elevar su nivel de diseño de APIs, demostrando cómo los conceptos puristas de POO pueden aplicarse de forma práctica para crear librerías robustas y elegantes.
