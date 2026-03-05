---
title: "The Pain of OOP Lecture #2: Static methods and attributes"
date: 2023-06-19T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
  - "oop"
  - "ai"
cover:
  image: "https://img.youtube.com/vi/lELJSj9mWbI/maxresdefault.jpg"
  alt: "The Pain of OOP Lecture #2: Static methods and attributes"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=lELJSj9mWbI](https://www.youtube.com/watch?v=lELJSj9mWbI)

## Summary
In this lecture, Yegor Bugayenko presents a provocative critique of static methods and attributes, labeling them as a "cancer" that fundamentally undermines Object-Oriented Programming (OOP). His primary argument is that static members transform expressive, object-oriented designs into rigid, procedural scripts. By attaching logic to a class rather than an instance, developers create "hard-coded" dependencies that are impossible to intercept, mock, or replace during unit testing without specialized tools. 

Yegor further distinguishes between "eager" (imperative) and "lazy" (declarative) programming. He argues that static methods (like `Math.sqrt(x)`) are imperative commands that execute immediately, whereas true objects should be declarative representations of values that perform calculations only when absolutely necessary. This "laziness" allows for better composition and flexibility. Finally, he attacks the concept of "Utility Classes" (e.g., `StringUtils`), describing them as "garbage bins" for logic that lacks a proper home. These classes possess no identity and violate the Single Responsibility Principle, leading to high coupling and low cohesion. To achieve "pure" OOP, Yegor advocates for replacing every static method with a dedicated class and every static attribute with encapsulated object state.

## Key Insights
- "Static methods are a cancer; they turn your object-oriented code into procedural garbage."
- "An object should be a 'lazy' representative of a result, not an 'eager' executor of a command."
- "Utility classes are just namespaces for functions; they are not objects and have no place in a clean architecture."
- "If you can't mock it, you've failed at OOP. Static methods are the primary reason for untestable code."

## Relevance: 5/5
This lecture is highly relevant for software architects and developers seeking to understand the "Elegant Objects" philosophy. It challenges industry norms (like the Singleton pattern and Utility classes) and provides a rigorous, albeit controversial, framework for improving code testability and maintainability.
