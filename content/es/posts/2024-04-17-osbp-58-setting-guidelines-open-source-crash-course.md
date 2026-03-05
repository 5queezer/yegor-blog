---
title: "OSBP 5/8: Establecimiento de Directrices [curso intensivo de código abierto]"
date: 2024-04-17T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/mWi2S5FJiJ4/maxresdefault.jpg"
  alt: "OSBP 5/8: Establecimiento de Directrices [curso intensivo de código abierto]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=mWi2S5FJiJ4](https://www.youtube.com/watch?v=mWi2S5FJiJ4)

## Resumen
Yegor Bugayenko presenta una guía práctica sobre cómo establecer la disciplina necesaria en un repositorio de código abierto para que sea sostenible y profesional. Su enfoque se centra en la "gestión defensiva". Primero, insiste en la obligatoriedad de una **licencia** (recomienda MIT) para otorgar validez legal al proyecto. Segundo, destaca la importancia del **README.md**, el cual debe captar la atención en 10 segundos, mostrar "badges" de estado y ofrecer un inicio rápido de no más de tres líneas.

Una de las reglas más estrictas de Yegor es que la **rama principal (master) sea de solo lectura**. Nadie debe hacer "push" directo; todo debe pasar por Pull Requests. Además, critica los "Códigos de Conducta" tradicionales, prefiriendo directrices técnicas claras. El punto culminante es la **automatización mediante GitHub Actions**. Bugayenko sostiene que no se debe perder tiempo discutiendo estilos de código en documentos; en su lugar, se deben configurar herramientas automáticas que rechacen cualquier contribución que no cumpla con los estándares de calidad, delegando la autoridad en los "robots".

## Ideas Clave
- "Trata a los contribuyentes como si pudieran romper tu código: sé defensivo."
- "Si una regla de estilo es importante, debe ser un error de compilación, no una sugerencia en un PDF."
- "El README es la cara de tu proyecto; si no es atractivo, nadie lo usará."

## Relevancia: 5/5
Muy relevante para la gestión de equipos de ingeniería y la implementación de flujos de trabajo de Integración Continua (CI).
