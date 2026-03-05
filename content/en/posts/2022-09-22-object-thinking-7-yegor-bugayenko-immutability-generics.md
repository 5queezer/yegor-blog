---
title: "Object Thinking #7: Yegor Bugayenko / Immutability + Generics"
date: 2022-09-22T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
  - "oop"
cover:
  image: "https://img.youtube.com/vi/C6CQWzOKEJs/maxresdefault.jpg"
  alt: "Object Thinking #7: Yegor Bugayenko / Immutability + Generics"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=C6CQWzOKEJs](https://www.youtube.com/watch?v=C6CQWzOKEJs)

## Summary
In this episode of the "Object Thinking" series, Yegor Bugayenko explores the intersection of strict object-oriented principles with real-world library design, specifically focusing on his Java library **xsline**. The core of the discussion centers on how to build a transformation pipeline (XSL) that remains entirely **immutable** and **declarative**. 

Yegor introduces two primary metaphors: the **Shift** (a single transformation) and the **Train** (a pipeline of shifts). He argues vehemently against mutable state, replacing standard procedural methods like `add()` with a functional `with()` method. This method returns a new instance of the pipeline, ensuring thread safety and architectural clarity.

A significant portion of the video addresses the challenge of type safety when a pipeline needs to accept different inputs (e.g., an XSL file path as a `String` versus a pre-compiled `Shift` object). Yegor demonstrates how **Generics** can be used to "evolve" the type of a fluent API. By using a `Temporary` interface and a `back()` method, he allows the developer to switch contexts (e.g., from a `Train<String>` back to a `Train<Shift>`) without breaking the interface-only method rule. This approach ensures that the resulting code looks like a static declaration of "what" the pipeline is, rather than a sequence of "how" it is built.

## Key Insights
- **"Objects are not bags of data; they are self-sufficient entities that must be immutable to be reliable."**
- **"The transition from `Train<String>` to `Train<Shift>` via a `back()` method allows for a fluent API that respects strict type safety."**
- **"A class should never have public methods that are not defined in an interface; if it does, the design is leaked."**
- **"Declarative programming is superior because it describes the 'what' (the result) rather than the 'how' (the procedure)."**

## Relevance: 5/5
This session is highly relevant for senior engineers and architects. it provides a masterclass in applying theoretical OOP constraints (immutability, interface segregation) to solve complex API design problems using Java Generics.
