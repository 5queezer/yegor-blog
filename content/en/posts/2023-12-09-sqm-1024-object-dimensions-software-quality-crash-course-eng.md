---
title: "SQM 10/24: Object Dimensions [Software Quality Management]"
date: 2023-12-09T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
  - "oop"
cover:
  image: "https://img.youtube.com/vi/jdEFoz-OQ44/maxresdefault.jpg"
  alt: "SQM 10/24: Object Dimensions [Software Quality Management]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=jdEFoz-OQ44](https://www.youtube.com/watch?v=jdEFoz-OQ44)

## Summary
In this lecture, Yegor Bugayenko shifts the focus from simple code volume (LoC) to the structural "dimensions" of software quality: Encapsulation, Inheritance, Polymorphism, and Complexity. The core of the presentation revolves around the MOOD (Metrics for Object-Oriented Design) and C&K (Chidamber & Kemerer) metric suites, which provide a mathematical framework for evaluating design integrity.

Bugayenko explains that metrics like Method Hiding Factor (MHF) and Attribute Hiding Factor (AHF) are essential ratios for measuring encapsulation; a low AHF suggests that a class is exposing its internal state, violating the fundamental principles of OOP. He also delves into inheritance metrics (MIF and AIF), noting that while inheritance promotes reuse, an excessively high inheritance factor can lead to the "fragile base class" problem.

Furthermore, structural metrics such as Depth of Inheritance Tree (DIT) and Number of Children (NOC) are discussed to highlight how a class's position in a hierarchy affects its maintainability and risk profile. The lecture concludes by emphasizing that these metrics should be normalized and used to identify "critical points of failure" rather than just counting lines. For Bugayenko, a high Response For a Class (RFC) is a clear warning sign of high coupling and debugging difficulty.

## Key Insights
- "Lines of code is a poor proxy for quality; true object-oriented quality is measured through encapsulation and inheritance ratios."
- "If your Attribute Hiding Factor (AHF) is low, you aren't doing OOP; you are doing procedural programming with data structures."
- "Inheritance is a double-edged sword: high reuse (MIF) is good, but it increases the risk of the 'fragile base class' syndrome."
- "Response For a Class (RFC) is the most critical complexity metric—if an object knows too many ways to react, it becomes impossible to test."

## Relevance: 5/5
This lecture is highly relevant for senior engineers and architects who need objective, quantitative ways to measure technical debt and design quality.
