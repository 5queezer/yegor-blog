---
title: "SQM 9/24: CAMC and NHD [software quality crash course]"
date: 2023-12-07T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/oCxJ_YSSAGo/maxresdefault.jpg"
  alt: "SQM 9/24: CAMC and NHD [software quality crash course]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=oCxJ_YSSAGo](https://www.youtube.com/watch?v=oCxJ_YSSAGo)

## Summary
In this lecture of the Software Quality Management series, Yegor Bugayenko explores two key structural metrics for measuring class cohesion: Cohesion Among Methods in Class (CAMC) and Normalized Hamming Distance (NHD). The session begins with a historical reflection on the Rational Unified Process (RUP), contrasting its heavy, document-driven discipline with modern Agile practices. Bugayenko argues that while RUP was perhaps too rigid, its focus on architecture and interfaces is something modern development often lacks.

The core of the lecture is dedicated to the mathematical evaluation of cohesion. CAMC measures how much the parameter types overlap across all methods in a class; a value of 1.0 indicates that all methods use the same set of types, suggesting a highly focused class. NHD is presented as a more sophisticated alternative that uses Hamming distance to measure the "similarity" between method signatures. It is more sensitive to internal clustering, helping identify classes that should be split.

Bugayenko ties these metrics to the Interface Segregation Principle (ISP) from SOLID. He critiques the Java standard library, specifically the `InputStream` class, as a "fat interface" that forces implementations to provide methods like `mark()` and `reset()` even when they aren't supported. This lack of cohesion leads to fragile code and violations of the Liskov Substitution Principle.

## Key Insights
- "A class with low cohesion is essentially multiple classes trapped in a single container, waiting to be liberated."
- "Metrics like CAMC and NHD aren't just numbers; they are mathematical evidence of violations of the Interface Segregation Principle."
- "The Java InputStream is a classic example of a 'fat interface'—it forces unrelated responsibilities onto every implementation, leading to UnsupportedOperationExceptions."
- "Decoupling is only possible when we depend on stable, cohesive abstractions rather than bloated concrete implementations."

## Relevance: 5/5
Essential for developers interested in objective code quality, SOLID principles, and moving beyond "gut feelings" about class design.
