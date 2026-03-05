---
title: "SQM 8/24: TCC and LCC [Software Quality Crash Course]"
date: 2023-12-02T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/JOKxjpAglFU/maxresdefault.jpg"
  alt: "SQM 8/24: TCC and LCC [Software Quality Crash Course]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=JOKxjpAglFU](https://www.youtube.com/watch?v=JOKxjpAglFU)

## Summary
In this lecture of the Software Quality Management (SQM) series, Yegor Bugayenko explores the formal measurement of class cohesion through two specific metrics: Tight Class Cohesion (TCC) and Loose Class Cohesion (LCC), as defined by Bieman and Kang. Cohesion is presented as the "cement" of a well-designed module, representing how closely the methods of a class work together toward a single, central purpose.

The lecture breaks down the technical definitions: TCC measures the ratio of method pairs that are "directly connected" (sharing at least one common instance variable) to the total possible pairs. LCC expands this to include "indirectly connected" pairs (methods linked through a chain of shared variables). Yegor emphasizes that a TCC value below 0.5 often indicates a class that should be split, as it likely handles multiple unrelated responsibilities.

A significant portion of the talk is dedicated to the relationship between inheritance and cohesion. Yegor argues that implementation inheritance often forces classes to include "dead" or irrelevant code, thereby lowering cohesion. He advocates for composition over inheritance to maintain high TCC/LCC scores and ensure that objects remain focused, encapsulated entities rather than mere containers for code reuse.

## Key Insights
- "Cohesion is the cement of a well-designed module; it is what keeps the object as a single, focused entity."
- "If your Tight Class Cohesion (TCC) is below 0.5, your class is likely a 'blob' that needs to be refactored into smaller components."
- "Inheritance is often just a procedural trick for code reuse that destroys the internal cohesion of objects."
- "The difference between TCC and LCC reveals how fragmented the internal logic of your class truly is."

## Relevance: 5/5
This lecture provides objective, mathematical metrics for a concept (cohesion) that is often treated as purely subjective, making it essential for senior developers and architects.
