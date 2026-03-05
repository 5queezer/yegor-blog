---
title: "SQM 21/24: Compilaciones (Builds) [curso intensivo de calidad de software]"
date: 2024-04-03T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/QQUda0fAcxE/maxresdefault.jpg"
  alt: "SQM 21/24: Compilaciones (Builds) [curso intensivo de calidad de software]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=QQUda0fAcxE](https://www.youtube.com/watch?v=QQUda0fAcxE)

## Resumen
En esta lección, Yegor Bugayenko explora la evolución histórica y las métricas técnicas de las compilaciones (builds) de software dentro del contexto de la Gestión de Calidad de Software (SQM). Traza el concepto desde los hitos de principios de los 90, como el "Daily Build and Smoke Test" de Microsoft, pasando por el auge de Extreme Programming (XP) en 1998, hasta la formalización de la Integración Continua (CI) por Martin Fowler y la Entrega Continua (CD) por Jez Humble.

Una parte importante de la lección se dedica al análisis de las métricas de compilación y la distribución de los tiempos de ejecución. Yegor destaca un "punto de dolor" crítico en la industria: los **tests inestables (flaky tests)**. Argumenta que las pruebas no deterministas —aquellas que fallan y luego pasan con un simple reinicio— son una gran amenaza para la calidad del software porque destruyen la confianza del equipo en el proceso de CI. Si los desarrolladores dejan de tomar en serio los fallos del build, la CI deja de funcionar como una puerta de calidad efectiva. La clase también cubre la CI a gran escala y enfatiza la importancia de medir el "Tiempo de reparación" y el "Ratio de inestabilidad" para mantener un entorno de desarrollo profesional.

## Ideas Clave
- "Un build no es solo un paso técnico; es una declaración formal de que el código cumple con los estándares de calidad del proyecto."
- "El mayor enemigo de un proceso de CI saludable es el botón de 'reintentar'. Los tests inestables destruyen la confianza del desarrollador en la automatización."
- "La Integración Continua no es una herramienta como Jenkins; es la práctica de integrar el trabajo varias veces al día."
- "Los fallos de compilación deben ocurrir rápido. El desperdicio de tiempo más caro es un build que falla después de ejecutarse durante una hora."

## Relevancia: 5/5
Altamente relevante para ingenieros de software y gestores de equipos. Explica por qué la automatización de builds es el pilar fundamental de la disciplina técnica y la calidad.
