---
title: "The Pain of OOP, Lecture #8: Inheritance"
date: 2023-08-22T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
  - "oop"
  - "ai"
cover:
  image: "https://img.youtube.com/vi/m0OEOoGgIuM/maxresdefault.jpg"
  alt: "The Pain of OOP, Lecture #8: Inheritance"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=m0OEOoGgIuM](https://www.youtube.com/watch?v=m0OEOoGgIuM)

## Summary
In this lecture, Yegor Bugayenko discusses one of the most controversial topics in Object-Oriented Programming: inheritance. He makes a sharp distinction between "subtyping" (interfaces) and "implementation inheritance" (the `extends` keyword). While subtyping is praised as the foundation of polymorphism and the Liskov Substitution Principle (LSP), implementation inheritance is condemned as a procedural "hack" for code reuse that destroys encapsulation.

Bugayenko argues that inheritance creates tight coupling between a parent and its children, leading to the "Fragile Base Class" problem—where changes in a base class unexpectedly break subclasses. He critiques the use of `protected` modifiers, stating they violate the "black box" principle of objects. The lecture also touches on the pitfalls of method overloading and multiple inheritance. As a solution, he advocates for "Composition over Inheritance," suggesting that objects should encapsulate and delegate behavior rather than inheriting it. This approach leads to smaller, more maintainable, and decoupled codebases.

## Key Insights
- "Implementation inheritance is not about object thinking; it's a procedural shortcut for lazy code reuse."
- "The moment you use the `protected` modifier, you have admitted that your encapsulation is broken."
- "Objects should be independent behavioral units, not data bags with shared implementation details."
- "A true OOP architect uses interfaces to define types and composition to reuse logic."

## Relevance: 5/5
This lecture is highly relevant as it challenges industry-standard practices and provides a deep dive into architectural principles that directly impact software maintainability and scalability.
