---
title: "EQSP 4/20: Creando GitHub Actions Personalizadas, con un Ejemplo [curso intensivo de calidad de software]"
date: 2022-09-07T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/7oKqqgpKjIM/maxresdefault.jpg"
  alt: "EQSP 4/20: Creando GitHub Actions Personalizadas, con un Ejemplo [curso intensivo de calidad de software]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=7oKqqgpKjIM](https://www.youtube.com/watch?v=7oKqqgpKjIM)

## Resumen
En esta lección, Yegor Bugayenko ofrece una guía práctica para construir GitHub Actions personalizadas, una habilidad crucial para los equipos que buscan automatizar los controles de calidad del software más allá de las soluciones estándar. Yegor sostiene que el desarrollo profesional exige "ser dueño" de tu pila de automatización para imponer leyes específicas en el proyecto. Distingue entre las acciones basadas en JavaScript y las basadas en Docker, abogando firmemente por estas últimas. Las acciones de Docker empaquetan todo el entorno de ejecución (SO, dependencias y herramientas), asegurando que la acción se ejecute de forma idéntica independientemente de la configuración del corredor de GitHub.

El recorrido técnico se centra en tres archivos principales: `action.yml` (el manifiesto que define las entradas y la lógica), un `Dockerfile` (la definición del entorno) y un script de entrada (normalmente `entry.sh`). Yegor demuestra cómo envolver una herramienta de línea de comandos en un contenedor y configurarla para analizar el código dentro del directorio `/github/workspace`. El objetivo final es crear un mecanismo de "error rápido" (fail-fast), donde cualquier violación de los estándares de calidad resulte inmediatamente en un estado de compilación fallido en una Pull Request. Al alejarse de las revisiones humanas subjetivas y optar por scripts objetivos y automatizados, los equipos pueden mantener un nivel de calidad mucho más alto y consistente.

## Ideas Clave
- **Automatizar la "Ley":** Los estándares de calidad nunca deben ser simples sugerencias; deben implementarse como scripts que interrumpan la compilación si se violan.
- **Consistencia del Entorno:** Las acciones basadas en Docker son superiores a las de JavaScript porque eliminan los problemas de "funciona en mi máquina" al estandarizar el entorno del corredor.
- **Retroalimentación Objetiva:** El propósito principal de las acciones personalizadas es proporcionar retroalimentación inmediata, objetiva y no negociable a los desarrolladores a través del pipeline de CI/CD.
- **Independencia:** Confiar únicamente en acciones de terceros es un riesgo; los equipos profesionales deben construir y mantener sus propios componentes de automatización para los filtros de calidad críticos.

## Relevancia: 5/5
Muy relevante para ingenieros de software y profesionales de DevOps. Conecta el uso básico de CI/CD con la automatización avanzada, centrándose en la filosofía de "fallo rápido" esencial para mantener bases de código de alta calidad.
