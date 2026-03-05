---
title: "EQSP 12/20: Lanzamiento de cambios en bases de datos"
date: 2022-10-06T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
  - "infrastructure"
cover:
  image: "https://img.youtube.com/vi/qtTG1kRLzCY/maxresdefault.jpg"
  alt: "EQSP 12/20: Lanzamiento de cambios en bases de datos"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=qtTG1kRLzCY](https://www.youtube.com/watch?v=qtTG1kRLzCY)

## Resumen
En esta lección de su curso intensivo sobre calidad de software, Yegor Bugayenko defiende un enfoque estrictamente automatizado para la gestión de bases de datos, tratándolas como activos fundamentales del código de la aplicación. Su tesis central es que las intervenciones manuales en las bases de datos de producción son una señal de falta de profesionalismo y la principal fuente de inestabilidad. Según Bugayenko, cada cambio debe encapsularse en scripts de migración versionados (por ejemplo, 001.sql, 002.sql) almacenados en el repositorio de código fuente junto con la lógica de negocio.

Bugayenko enfatiza el uso de herramientas como Liquibase o Flyway para gestionar estas transiciones. Estas herramientas mantienen un registro histórico dentro de la propia base de datos, garantizando que solo se ejecuten los scripts nuevos durante el despliegue. El flujo de trabajo propuesto es tajante: la canalización (pipeline) de CI/CD es la única entidad con autoridad para modificar el esquema de producción. Los desarrolladores nunca deben tener acceso directo; su función es proponer cambios mediante Merge Requests, que luego son revisados por un arquitecto y aplicados automáticamente. Este enfoque elimina la deriva de configuración y asegura que el entorno sea reproducible. Al quitar el poder manual a los individuos y otorgárselo a los procesos automatizados, los equipos pueden lograr la consistencia necesaria para sistemas de software escalables y de alta calidad.

## Ideas Clave
- "La base de datos no es solo un almacén; es una parte viva del código de tu aplicación y debe versionarse como tal."
- "Si un programador tiene acceso manual a la base de datos de producción, no tienes un proceso de calidad, tienes una receta para el desastre."
- "La automatización es la única forma de quitarle la autoridad al error humano y dársela a la arquitectura del sistema."
- "Herramientas como Liquibase no son opcionales; son los guardianes de la integridad estructural de tu proyecto."

## Relevancia: 5/5
Es fundamental para ingenieros de software y arquitectos que buscan implementar flujos de CI/CD robustos y mantener estándares de calidad estrictos en aplicaciones con estado.
