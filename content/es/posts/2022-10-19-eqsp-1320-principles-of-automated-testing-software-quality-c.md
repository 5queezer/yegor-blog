---
title: "EQSP 13/20: Principios de las pruebas automatizadas"
date: 2022-10-19T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
  - "testing"
cover:
  image: "https://img.youtube.com/vi/hzrzq5HAhvM/maxresdefault.jpg"
  alt: "EQSP 13/20: Principios de las pruebas automatizadas"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=hzrzq5HAhvM](https://www.youtube.com/watch?v=hzrzq5HAhvM)

## Resumen
En esta lección, Yegor Bugayenko explora la filosofía fundamental y la necesidad técnica de las pruebas automatizadas dentro de un marco de calidad de software. Sostiene que las pruebas automatizadas no son solo una herramienta para detectar errores, sino un mecanismo vital para aumentar la velocidad de desarrollo y eliminar lo que él llama "Desarrollo impulsado por el miedo" (Fear-Driven Development). Cuando los desarrolladores carecen de una suite de pruebas robusta, temen modificar el código, lo que conduce al estancamiento y a la deuda técnica.

El núcleo del enfoque de Bugayenko es el concepto de "Red de Seguridad". Una suite integral de pruebas automatizadas permite a los desarrolladores realizar cambios audaces con la confianza de que cualquier regresión será detectada de inmediato. Distingue claramente entre las Pruebas Unitarias —que deben ser extremadamente rápidas y proporcionar retroalimentación instantánea— y las Pruebas de Integración, que cubren el comportamiento del sistema de manera más amplia pero son naturalmente más lentas.

Un principio crítico enfatizado es el ciclo obligatorio de reproducción de errores: nunca se debe corregir un error hasta que se haya escrito una prueba automatizada que lo reproduzca. Si el código está roto pero las pruebas pasan, el fallo reside en la propia estrategia de pruebas. Al tratar las pruebas como ciudadanos de primera clase del código fuente, los equipos aseguran que, una vez corregido un error, este no vuelva a aparecer. En última instancia, el objetivo de la automatización es crear un entorno determinista donde la calidad sea un subproducto medible del proceso de desarrollo.

## Ideas Clave
- "Si tienes un error pero tus pruebas pasan, el problema no está en el código, sino en tus pruebas."
- "Las pruebas manuales son un desperdicio del potencial humano; si una máquina puede revisarlo, una máquina debe revisarlo."
- "El objetivo de las pruebas automatizadas es eliminar el miedo, permitiendo que los desarrolladores sean productivamente 'descuidados'."
- "Una corrección de errores sin una prueba que los reproduzca es solo un parche temporal que eventualmente volverá a fallar."

## Relevancia: 5/5
Esta lección es esencial para comprender cómo las pruebas automatizadas se integran con CI/CD, la productividad del equipo y la mantenibilidad a largo plazo.
