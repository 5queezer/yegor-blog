---
title: "SQM 8/24: TCC y LCC [Curso Intensivo de Calidad de Software]"
date: 2023-12-02T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/JOKxjpAglFU/maxresdefault.jpg"
  alt: "SQM 8/24: TCC y LCC [Curso Intensivo de Calidad de Software]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=JOKxjpAglFU](https://www.youtube.com/watch?v=JOKxjpAglFU)

## Resumen
En esta lección, Yegor Bugayenko profundiza en la medición formal de la cohesión de clases utilizando las métricas Tight Class Cohesion (TCC) y Loose Class Cohesion (LCC). La cohesión se define como el "cemento" que mantiene unidos los componentes de un módulo, asegurando que una clase tenga un propósito único y claro. El video se basa en el modelo de Bieman y Kang para transformar un concepto abstracto en datos cuantificables.

La TCC mide la proporción de pares de métodos que están "directamente conectados" a través del uso compartido de variables de instancia. La LCC, por su parte, incluye conexiones indirectas, proporcionando una visión más amplia de la conectividad interna. Yegor explica que un valor de TCC inferior a 0.5 es una señal de alerta que indica que la clase probablemente debería dividirse en fragmentos más pequeños y especializados.

Bugayenko también lanza una fuerte crítica contra la herencia de implementación. Argumenta que la herencia suele violar la cohesión al introducir dependencias innecesarias y código "muerto" en las subclases. Su recomendación es priorizar la composición sobre la herencia para mantener objetos altamente cohesivos y alineados con los principios de la programación orientada a objetos (POO) pura.

## Ideas Clave
- "La cohesión es el cemento de un módulo bien diseñado; es lo que define si un objeto es realmente una entidad o solo un contenedor."
- "Si tu TCC es menor a 0.5, tu clase está fragmentada y carece de un propósito central único."
- "La herencia es un mecanismo de reutilización de código que, con frecuencia, compromete la integridad del diseño orientado a objetos."
- "TCC y LCC nos permiten diagnosticar la salud de nuestra arquitectura sin depender de la intuición."

## Relevancia: 5/5
Vital para entender cómo evaluar la calidad del diseño de software de manera objetiva, especialmente en sistemas complejos donde la cohesión tiende a degradarse.
