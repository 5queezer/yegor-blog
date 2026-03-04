---
title: "Pain of OOP, Innopolis University, 2024, 8 lectures in one video"
date: 2025-03-31T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
  - "oop"
  - "ai"
cover:
  image: "https://img.youtube.com/vi/awB08yeXfZM/maxresdefault.jpg"
  alt: "Pain of OOP, Innopolis University, 2024, 8 lectures in one video"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=awB08yeXfZM](https://www.youtube.com/watch?v=awB08yeXfZM)

## Summary
Yegor Bugayenko's "Pain of OOP" course systematically dismantles mainstream Object-Oriented Programming practices, arguing that modern enterprise software is mostly procedural programming disguised as OOP. Across eight comprehensive lectures, Bugayenko critiques deeply ingrained industry habits: the use of getters and setters, static methods, null references, and ORM frameworks. He advocates for "Elegant Objects," a stricter, purer paradigm where objects are treated as active, living entities rather than passive data containers.

The course dives deep into practical rules for true object-oriented design. Bugayenko champions strict immutability, arguing that objects whose state changes are inherently unpredictable and harder to maintain. He insists on the absolute eradication of `null`, calling for the use of Null Objects or Optional types instead. Furthermore, constructors must be entirely code-free—their only job is to assign variables, delaying any actual computation until a specific method is invoked. True encapsulation is a major theme; Bugayenko explains that exposing internal state through DTOs (Data Transfer Objects) or accessors destroys object cohesion.

He also targets modern testing practices, heavily criticizing mocking frameworks (like Mockito) and instead recommending the use of "fake" objects that implement the same interfaces. Composition is heavily favored over implementation inheritance, and the extensive use of interfaces and decorators is presented as the right way to extend behavior. Ultimately, the "pain" refers to the steep learning curve and discomfort developers face when unlearning toxic industry standards, but the reward is highly maintainable, cohesive, and resilient software architecture.

## Key Insights
- "Getters and setters strip objects of their dignity, turning them into mere data bags."
- "Static methods are a procedural virus in the object-oriented world."
- "Constructors must be code-free; an object should be instantiated fast and do work only when its methods are called."
- "Null is not an object; returning or accepting null is a violation of trust between objects."

## Relevance: 5/5
This lecture series is highly relevant as it fundamentally challenges standard enterprise software engineering practices and offers a strict, cohesive alternative for designing robust object-oriented systems.
