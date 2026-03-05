---
title: "EQSP 3/20: CI y DevOps con GitHub Actions [curso intensivo de calidad de software]"
date: 2022-09-06T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/c2_h7CMzUgA/maxresdefault.jpg"
  alt: "EQSP 3/20: CI y DevOps con GitHub Actions [curso intensivo de calidad de software]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=c2_h7CMzUgA](https://www.youtube.com/watch?v=c2_h7CMzUgA)

## Resumen
En esta lección de su "Curso Intensivo de Calidad de Software", Yegor Bugayenko explora los aspectos prácticos y filosóficos de la Integración Continua (CI) y DevOps, utilizando específicamente GitHub Actions. Redefine la CI no simplemente como un conjunto de pruebas, sino como un "mecanismo de protección" diseñado para mantener el código de baja calidad fuera del repositorio principal. El núcleo de su enfoque es el principio de "Master de solo lectura": los desarrolladores nunca deben realizar "push" directamente a la rama principal. En su lugar, todos los cambios deben pasar por una canalización rigurosa y automatizada que incluye pruebas unitarias (Maven), comprobaciones de estilo (Xcop), métricas de calidad (Kulis) y escaneo de seguridad (Snyk).

Bugayenko destaca el uso de GitHub Actions por su configuración basada en YAML e infraestructura gratuita para proyectos de código abierto. Demuestra funciones avanzadas como las construcciones matriciales (matrix builds) para realizar pruebas en diferentes versiones de JDK simultáneamente. Una parte significativa de la conferencia está dedicada a "Rulor", un chatbot personalizado que gestiona el proceso de fusión (merge). Al usar comandos como `@rulor merge`, el bot crea un entorno aislado, realiza la fusión localmente, ejecuta todas las comprobaciones y solo publica en master si todo es correcto. Esto traslada la responsabilidad de la calidad del programador individual al "sistema", asegurando que si un error llega a producción, se vea como un fallo de la canalización y no de la persona.

## Ideas Clave
- "La calidad ocurre cuando eliminas las partes malas de forma intencionada y explícita".
- "El Master es sagrado: nunca hagas push directamente; deja que los robots lo protejan".
- "Culpa al sistema, no a la persona: si un error llega a master, tu pipeline de CI ha fallado".
- "Cada línea de código debe estar vinculada a un ticket; sin intención no hay código".

## Relevancia: 5/5
Extremadamente alta para la ingeniería de software moderna. Proporciona un modelo para construir canalizaciones de entrega de alta integridad y fomentar una cultura de responsabilidad automatizada.
