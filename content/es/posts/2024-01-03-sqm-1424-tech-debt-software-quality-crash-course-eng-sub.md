---
title: "SQM 14/24: Deuda Técnica [Curso Intensivo de Calidad de Software]"
date: 2024-01-03T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/pvZDcytPU3w/maxresdefault.jpg"
  alt: "SQM 14/24: Deuda Técnica [Curso Intensivo de Calidad de Software]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=pvZDcytPU3w](https://www.youtube.com/watch?v=pvZDcytPU3w)

## Resumen
En esta conferencia de su curso de Gestión de Calidad de Software (SQM), Yegor Bugayenko presenta una perspectiva disciplinada sobre la "Deuda Técnica". El núcleo de su argumento radica en una distinción binaria estricta: el código es "Deuda Técnica" o es "Desorden Técnico" (Mess). Según Yegor, la deuda es una elección estratégica e intencional de eludir los estándares de calidad para cumplir con un hito comercial, siempre que esté registrada formalmente en un sistema de seguimiento de tareas. Por el contrario, el "Desorden" es simplemente código de baja calidad que existe por negligencia, permaneciendo indocumentado e invisible.

Yegor utiliza la metáfora de Ward Cunningham para explicar que la deuda técnica funciona como un préstamo financiero. Permite al equipo "comprar tiempo" en el presente, pero conlleva el pago obligatorio de "intereses". Estos intereses se manifiestan como el esfuerzo adicional y el tiempo requerido para implementar cada nueva funcionalidad debido a la fragilidad de la base de código. Advierte que, si esta deuda no se paga sistemáticamente mediante la refactorización, los intereses pueden superar la capacidad del equipo para entregar valor, lo que lleva a la "quiebra técnica".

Para gestionar esto, Yegor aboga por el Puzzle Driven Development (PDD). Argumenta que los comentarios `// TODO` tradicionales son ineficaces porque son pasivos. El PDD requiere que los desarrolladores dejen "puzzles" estructurados en el código que se conviertan automáticamente en problemas (issues) de GitHub. Esto asegura que la deuda sea visible para la gerencia y pueda ser priorizada junto con las nuevas funciones. La conferencia enfatiza que la gestión de la deuda es una responsabilidad a nivel de proceso, donde el arquitecto decide qué "préstamos" vale la pena tomar para asegurar la viabilidad del proyecto a largo plazo.

## Ideas Clave
1. "Si no está en el rastreador de tareas, no es deuda técnica; es simplemente un desorden técnico."
2. "La deuda técnica es un compromiso consciente en el que pides prestada productividad al futuro para ganar velocidad hoy."
3. "El interés de la deuda técnica es un impuesto que pagas por cada nueva línea de código que escribes en un sistema saturado."
4. "El PDD convierte la esperanza pasiva de refactorizar en una tarea activa, rastreada y manejable."

## Relevancia: 5/5
Extremadamente relevante para líderes de equipo y arquitectos, proporcionando un marco formal para discutir la calidad con las partes interesadas del negocio.
