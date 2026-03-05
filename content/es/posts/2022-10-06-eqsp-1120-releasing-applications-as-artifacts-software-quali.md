---
title: "EQSP 11/20: Lanzamiento de aplicaciones como artefactos"
date: 2022-10-06T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/9YeTbqFr85s/maxresdefault.jpg"
  alt: "EQSP 11/20: Lanzamiento de aplicaciones como artefactos"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=9YeTbqFr85s](https://www.youtube.com/watch?v=9YeTbqFr85s)

## Resumen
En esta lección, Yegor Bugayenko explica la distinción crítica entre una biblioteca de software (paquete) y una aplicación completa en el contexto de la gestión de lanzamientos. Mientras que una biblioteca es una dependencia utilizada por otros desarrolladores, una aplicación es un producto final que requiere una estrategia de despliegue más robusta. La tesis central es la "Filosofía del Artefacto": una aplicación debe entregarse como una unidad única, inmutable y con versión, como una imagen de Docker o un archivo "fat JAR". Este enfoque garantiza la independencia del entorno y elimina los riesgos asociados con las transferencias manuales de archivos o errores de configuración.

Yegor enfatiza que el despliegue nunca debe implicar un "git pull" en un servidor de producción. En su lugar, debe ser un "cambio" controlado donde se lanza una nueva versión del artefacto junto con la antigua. Para mantener la integridad de los datos durante esta transición, sugiere un "modo de solo lectura", donde la versión antigua deja de escribir en la base de datos justo antes de que el tráfico se redirija a la nueva versión. Además, todo el proceso debe estar completamente automatizado. Usando herramientas como Rultor, los desarrolladores deben activar los lanzamientos mediante comandos simples en un ticket, dejando el trabajo pesado de probar, etiquetar y desplegar a bots autónomos. Esto elimina el error humano y asegura que el entorno de producción permanezca intacto.

## Ideas Clave
- "Una aplicación no es solo código; es un artefacto único e inmutable que debe contener todo lo que necesita para ejecutarse".
- "Si estás haciendo un 'git pull' en tu servidor de producción, no eres un profesional; eres un aficionado jugando con fuego".
- "El proceso de despliegue es esencialmente un cambio de tráfico entre dos estados inmutables del sistema".
- "El tiempo de inactividad cero no se logra por magia, sino poniendo el sistema en modo de solo lectura durante los segundos críticos de la transición".

## Relevancia: 5/5
Este video es esencial para comprender las prácticas modernas de CI/CD, la cultura DevOps y el cambio de la entrega centrada en el código a la centrada en el artefacto, fundamental para la ingeniería de software escalable.
