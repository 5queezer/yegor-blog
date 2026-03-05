---
title: "The Pain of OOP, Lecture #7: Reflection and Type Casting"
date: 2023-08-14T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
  - "oop"
  - "ai"
cover:
  image: "https://img.youtube.com/vi/vYw_GcDkPQA/maxresdefault.jpg"
  alt: "The Pain of OOP, Lecture #7: Reflection and Type Casting"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=vYw_GcDkPQA](https://www.youtube.com/watch?v=vYw_GcDkPQA)

## Summary
In this lecture, Yegor Bugayenko argues that reflection and type casting are fundamental "anti-patterns" in object-oriented programming because they violate the core principle of encapsulation and lead to unmaintainable, tightly coupled code. Bugayenko posits that type casting (e.g., `instanceof` checks) is a sign of poor design, describing it as "discriminating" against an object based on its class rather than interacting with its behavior. When you cast an object, you force the client to have intimate knowledge of the implementation, which breaks the abstraction. If the internal type changes, every place where a cast occurs must also change, spreading fragility throughout the codebase.

Furthermore, he views reflection as a "hack" that bypasses the compiler’s safety mechanisms. Reflection allows for "magic" behaviors—like accessing private fields or instantiating classes via strings—which creates dependencies that are invisible to the compiler, making the code nearly impossible to refactor safely. He is particularly critical of reflection-heavy frameworks and annotations, arguing they turn self-sufficient objects into passive data structures manipulated by external logic. Bugayenko advocates for strict adherence to polymorphism, where the client is "blind" to the implementation. He suggests replacing reflection-based Dependency Injection (DI) containers with manual constructor injection and avoiding any logic that "peeks" inside an object. Ultimately, he argues that while these tools offer short-term flexibility, they create a "mess of spaghetti code" that sacrifices long-term maintainability.

## Key Insights
- "Casting is discrimination by type; in true OOP, we should only care about behavior, not the name on the object's passport."
- "Reflection is a hack that makes your code invisible to the compiler and impossible to refactor safely."
- "An object should be a black box; the moment you 'peek' inside via reflection, you've lost the benefits of encapsulation."
- "Frameworks that rely on 'magic' through annotations turn active, intelligent objects into passive data holders manipulated by external forces."

## Relevance: 5/5
This lecture is highly relevant for any developer aiming to understand deep architectural principles, clean code, and the long-term consequences of "magic" in modern frameworks.
