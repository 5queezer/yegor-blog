---
title: "Los primeros signos de alta calidad en la ingeniería de software"
date: 2023-04-13T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/5PLqi79uA0s/maxresdefault.jpg"
  alt: "Los primeros signos de alta calidad en la ingeniería de software"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=5PLqi79uA0s](https://www.youtube.com/watch?v=5PLqi79uA0s)

## Resumen
En esta lección, Yegor Bugayenko presenta los indicadores fundamentales de la alta calidad en la ingeniería de software. Según Bugayenko, la calidad no es la simple ausencia de errores, sino la existencia de una disciplina férrea y un conflicto institucionalizado. El primer signo es la naturaleza del "Code Review": el revisor y el autor deben actuar como oponentes profesionales. El objetivo del revisor es detectar fallos, mientras que el autor debe demostrar la validez de su código basándose exclusivamente en reglas objetivas. Si una crítica no se fundamenta en un estándar documentado o una métrica automatizada, puede ser ignorada, eliminando así la subjetividad del proceso.

Otro pilar fundamental es la gestión de la responsabilidad. Bugayenko enfatiza que antes de la integración (merge), la culpa de cualquier error recae exclusivamente en el autor; sin embargo, después del merge, la responsabilidad se vuelve colectiva, implicando especialmente al revisor que aprobó el cambio. Además, subraya que la calidad es imposible sin una automatización total (linters, pruebas automáticas) y prohíbe terminantemente las acciones manuales o los privilegios de acceso directo al código principal ("Read-only Master"). Por último, critica el concepto de "heroísmo" en el desarrollo. En un proyecto de alta calidad, no se necesitan héroes que trabajen de noche para arreglar desastres; en su lugar, se requiere una adherencia constante y casi aburrida a los protocolos establecidos. La calidad es el resultado de procesos que eliminan el factor humano y la improvisación.

## Ideas Clave
* "Los revisores deben ser oponentes, no amigos; su trabajo es detener el código mediocre."
* "Antes del merge es tu culpa; después del merge es nuestra culpa."
* "La calidad es una disciplina aburrida y repetitiva, no una serie de actos heroicos."
* "Las opiniones subjetivas no tienen lugar en el code review; si no hay una regla escrita, no hay comentario válido."

## Relevancia: 5/5
Esencial para líderes de equipo y arquitectos que buscan implementar procesos de desarrollo robustos y predecibles basados en la responsabilidad técnica.
