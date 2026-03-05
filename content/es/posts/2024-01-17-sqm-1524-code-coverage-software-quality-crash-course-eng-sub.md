---
title: "SQM 15/24: Cobertura de Código [curso intensivo de calidad de software]"
date: 2024-01-17T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/pJrXQ5rptig/maxresdefault.jpg"
  alt: "SQM 15/24: Cobertura de Código [curso intensivo de calidad de software]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=pJrXQ5rptig](https://www.youtube.com/watch?v=pJrXQ5rptig)

## Resumen
La lección aborda la Cobertura de Código no solo como un informe técnico, sino como una métrica fundamental para la gestión disciplinada de la calidad del software. Yegor define cuatro niveles de rigor: cobertura de sentencias, de ramas, de condiciones y de rutas. Además, recorre la historia de la métrica desde sus inicios en los años 60 hasta su aplicación en estándares industriales modernos como la ISO 26262 y las políticas internas de empresas como Google.

El punto central de la lección es la postura radical de Yegor: la cobertura debe ser del 100% o no sirve de nada. Argumenta que permitir un umbral del 80% es, en la práctica, "legalizar" que una quinta parte del código sea basura no verificada. Para él, la cobertura es una herramienta de mando; debe integrarse en el flujo de CI/CD como un filtro severo que detenga cualquier compilación si la métrica disminuye. Finalmente, advierte sobre los "Line Hitters" (pruebas que ejecutan código sin validaciones reales), subrayando que una alta cobertura indica ejecución pero no necesariamente calidad. Por ello, concluye que la cobertura de código debe complementarse con Pruebas de Mutación para evaluar la efectividad real de los tests.

## Ideas Clave
* "La Cobertura de Código es una métrica de tu ignorancia. Muestra la parte del código que no controlas en absoluto."
* "Una alta cobertura no garantiza la ausencia de errores, pero una baja cobertura garantiza su presencia."
* "Si aceptas un 80% de cobertura, autorizas oficialmente a tus programadores a escribir un 20% de código de baja calidad, no verificado y potencialmente peligroso."
* "La calidad no se mejora con ruegos; se mejora midiendo y obligando a cumplir las cifras."

## Relevancia: 5/5
Muy relevante para líderes técnicos y gerentes de proyectos que buscan establecer criterios objetivos y automatizados para mantener la integridad del código a largo plazo.
