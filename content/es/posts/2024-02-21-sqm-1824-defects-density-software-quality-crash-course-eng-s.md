---
title: "SQM 18/24: Densidad de defectos"
date: 2024-02-21T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/M-yHXzROVno/maxresdefault.jpg"
  alt: "SQM 18/24: Densidad de defectos"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=M-yHXzROVno](https://www.youtube.com/watch?v=M-yHXzROVno)

## Resumen
En esta lección del curso de Gestión de Calidad de Software (SQM), Yegor Bugayenko profundiza en la métrica de "Densidad de Defectos" y cuestiona las creencias populares sobre el tamaño y la complejidad del código. La densidad de defectos se calcula como el número de errores confirmados dividido por el tamaño del software (generalmente en miles de líneas de código o KLOC). La charla se apoya en una investigación de Yamashita et al., replicada por el equipo de Bugayenko, que analiza cómo los umbrales de tamaño afectan la calidad real.

El punto más controvertido es el desafío al mito de que "lo más pequeño es mejor". Aunque las buenas prácticas suelen dictar que los archivos pequeños son preferibles, los datos indican que los archivos grandes suelen tener una densidad de defectos menor. Bugayenko explica que, al dividir un archivo complejo en múltiples piezas pequeñas para cumplir con reglas estéticas de código limpio, la complejidad no se elimina; simplemente se desplaza de la lógica interna del archivo a las interacciones entre los nuevos módulos. Estas interacciones suelen ser más difíciles de rastrear y son una fuente común de errores de integración. La conclusión es que los umbrales rígidos de líneas de código o complejidad ciclomática no son predictores fiables de calidad, y que el refactorizado debe centrarse en la claridad sistémica más que en métricas aisladas.

## Ideas Clave
- "La densidad de defectos nos permite entender la calidad no por el total de errores, sino por su frecuencia en relación al volumen de código."
- "Dividir archivos grandes en muchos pequeños no destruye la complejidad, solo la mueve de las tripas del código a las conexiones entre archivos."
- "Sorprendentemente, la investigación sugiere que los componentes de mayor tamaño pueden ser menos propensos a errores relativos que los fragmentados."
- "Los umbrales de tamaño y complejidad son indicadores engañosos que a menudo fallan al predecir la ubicación de los defectos."

## Relevancia: 5/5
Vital para arquitectos de software, ya que ofrece una visión pragmática basada en datos frente al idealismo de las reglas de estilo de código.
