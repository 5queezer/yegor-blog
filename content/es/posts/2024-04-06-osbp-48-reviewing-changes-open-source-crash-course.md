---
title: "OSBP 4/8: Revisión de Cambios [curso intensivo de código abierto]"
date: 2024-04-06T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/TJ83ePwyH_A/maxresdefault.jpg"
  alt: "OSBP 4/8: Revisión de Cambios [curso intensivo de código abierto]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=TJ83ePwyH_A](https://www.youtube.com/watch?v=TJ83ePwyH_A)

## Resumen
En esta cuarta entrega de la serie "Mejores Prácticas de Código Abierto", Yegor Bugayenko redefine el papel del revisor de código como un "guardián" y un "oponente" en lugar de un asistente servicial. La filosofía central es que las revisiones de código deben ser rigurosas, estrictas y centradas en mantener la integridad arquitectónica a largo plazo en lugar de simplemente comprobar si el código "funciona". Yegor sostiene que un revisor debe buscar activamente razones para rechazar una Pull Request (PR) para proteger el repositorio de la "putrefacción del código".

Se establecen varias reglas prácticas: Primero, un revisor nunca debe ejecutar el código localmente. La corrección funcional debe estar garantizada por pruebas automatizadas y CI; si un revisor siente la necesidad de ejecutar el código, significa que las pruebas son insuficientes. Segundo, las PR grandes (que abarcan docenas de archivos) deben rechazarse de inmediato porque son imposibles de revisar con eficacia. Los cambios deben ser atómicos y pequeños. Tercero, para las correcciones de errores, una PR es inválida a menos que incluya un "rompecabezas" (un caso de prueba) que falle sin la corrección y pase con ella.

Finalmente, Yegor enfatiza el valor educativo de las revisiones. Un revisor debe plantear los problemas, pero nunca resolverlos personalmente. Al explicar los principios subyacentes y los estándares del repositorio, el revisor actúa como mentor del colaborador, obligándole a mejorar su propio trabajo. Esto construye una cultura de altos estándares donde la calidad nunca se sacrifica por la velocidad.

## Ideas Clave
*   **El revisor como oponente:** El deber principal del revisor es encontrar fallos y rechazar el código, actuando como un filtro para la salud del repositorio.
*   **Confíe en la CI, no en la máquina local:** El tiempo humano es demasiado valioso para las pruebas manuales; la verificación funcional pertenece a la tubería automatizada.
*   **Nada de Pull Requests grandes:** Los cambios pequeños y atómicos son la única forma de garantizar un análisis profundo del código y evitar aprobaciones superficiales.
*   **El requisito del "puzzle":** Cada corrección de error debe ir acompañada de un caso de prueba fallido para demostrar que la solución funciona y evitar regresiones.

## Relevancia: 5/5
Este contenido es esencial para cualquier líder de software. Desafía la cultura de revisión "amigable" pero superficial, proporcionando un modelo para la gestión de equipos de alta calidad y la prevención de la deuda técnica.
