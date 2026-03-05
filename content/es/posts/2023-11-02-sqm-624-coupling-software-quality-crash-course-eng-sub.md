---
title: "SQM 6/24: Acoplamiento [curso intensivo de calidad de software]"
date: 2023-11-02T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/G0vN6Ah8-js/maxresdefault.jpg"
  alt: "SQM 6/24: Acoplamiento [curso intensivo de calidad de software]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=G0vN6Ah8-js](https://www.youtube.com/watch?v=G0vN6Ah8-js)

## Resumen
Yegor Bugayenko dedica esta sesión a explicar por qué el acoplamiento (Coupling) es el principal motor de la deuda técnica. El acoplamiento mide qué tan conectados están los módulos de un sistema: cuanto mayor es la interdependencia, más difícil es modificar el código sin romper funcionalidades existentes. Yegor retoma los principios del "Diseño Estructurado" de los años 70 para fundamentar su análisis.

El video profundiza en métricas como CBO (Acoplamiento entre Objetos) y DCC (Acoplamiento Directo de Clases). Yegor introduce un concepto propio: la "distancia de acoplamiento", que evalúa cuánto se propaga un objeto a través de diferentes llamadas en el sistema. También critica el acoplamiento temporal —donde el orden de ejecución es rígido— y el acoplamiento oculto, que ocurre de forma invisible para el compilador (como mediante la reflexión). La conclusión es clara: para lograr una arquitectura estable y fácil de probar, se debe aplicar el principio "Tell, Don't Ask" y reducir al mínimo lo que una clase conoce sobre las demás.

## Ideas Clave
- "El acoplamiento es el enemigo del cambio; si todo está conectado, nada puede moverse de forma segura."
- "El miedo al desacoplamiento a menudo resulta en sistemas monolíticos e inestables."
- "La distancia de acoplamiento debe ser lo más corta posible para evitar que los errores se propaguen."
- "Una clase con un CBO alto es una señal de alerta de que el diseño necesita ser refactorizado en objetos más pequeños."

## Relevancia: 5/5
Es un tema fundamental para la ingeniería de software moderna, especialmente en el contexto de microservicios y diseño modular.
