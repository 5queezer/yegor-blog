---
title: "El dolor de la POO, Lección #5: El sufijo -ER es malvado"
date: 2023-07-10T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
  - "oop"
  - "ai"
cover:
  image: "https://img.youtube.com/vi/6GMiosTLUTc/maxresdefault.jpg"
  alt: "El dolor de la POO, Lección #5: El sufijo -ER es malvado"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=6GMiosTLUTc](https://www.youtube.com/watch?v=6GMiosTLUTc)

## Resumen
En esta influyente lección de la serie "The Pain of OOP", Yegor Bugayenko presenta una crítica feroz contra una de las convenciones de nomenclatura más comunes en la ingeniería de software: el uso del sufijo "-er" (por ejemplo, Manager, Controller, Helper, Validator, Parser). Bugayenko sostiene que estos nombres no son una simple cuestión de estilo, sino indicadores claros de un pensamiento procedimental disfrazado de Programación Orientada a Objetos (POO). Según su filosofía "Elegant Objects", un objeto real debe definirse por "lo que es" (un sustantivo) y no por "lo que hace" (un verbo disfrazado de sustantivo). Al crear un `UserManager`, el programador está admitiendo que ha diseñado una estructura de datos pasiva y un "titiritero" externo para manipularla, lo que destruye la encapsulación y fomenta el "Modelo de Dominio Anémico".

La lección subraya la importancia del antropomorfismo: tratar a los objetos como organismos vivos con autonomía y dignidad, en lugar de verlos como herramientas o esclavos a los que se les ordenan tareas. Bugayenko propone que, en lugar de usar un `FileSaver` para realizar una acción, deberíamos diseñar un objeto `SavedFile` o simplemente un objeto `File` que represente la entidad de forma integral. Al eliminar el sufijo "-er", los desarrolladores se ven obligados a reconsiderar la identidad y responsabilidad de sus clases, lo que resulta en un código más pequeño, cohesivo y declarativo. Este cambio de paradigma, que pasa de una arquitectura de "jefe-esclavo" a un ecosistema de entidades autónomas, es para Yegor la única vía para producir software mantenible y de alta calidad. Además, desafía el uso excesivo de capas de "Servicio" y clases de "Utilidad", calificándolas como "cubos de basura" procedimentales.

## Ideas Clave
- Los objetos no son herramientas ni cubos de funciones; son organismos vivos con identidad propia.
- Si nombras a una clase "Manager", estás confesando que no sabes qué es el objeto ni cuál es su verdadera razón de ser.
- El sufijo "-er" es un síntoma de descomposición procedimental donde la lógica se separa de los datos, violando la encapsulación.
- Debemos descomponer los sistemas basándonos en entidades (sustantivos) y no en acciones (verbos). Es preferible un `ValidatedUser` que un `UserValidator`.

## Relevancia: 5/5
Esta lección es fundamental para desarrolladores que buscan mejorar su diseño arquitectónico y comprender las raíces filosóficas del código orientado a objetos de alta calidad.
