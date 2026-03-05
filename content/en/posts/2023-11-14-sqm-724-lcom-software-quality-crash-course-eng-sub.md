---
title: "SQM 7/24: LCOM [software quality crash course]"
date: 2023-11-14T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/74YigDo8_BE/maxresdefault.jpg"
  alt: "SQM 7/24: LCOM [software quality crash course]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=74YigDo8_BE](https://www.youtube.com/watch?v=74YigDo8_BE)

## Summary
In this lecture, Yegor Bugayenko explores the concept of Cohesion, focusing specifically on the LCOM (Lack of Cohesion of Methods) metric. He begins by contrasting Cohesion (internal strength of a module) with Coupling (external dependency strength), noting that the ideal software architecture strives for high cohesion and low coupling. A non-cohesive class is compared to a "junk drawer" where unrelated logic is stored together, making it difficult to maintain and test.

The core of the talk reviews the historical hierarchy of cohesion, from the worst (Coincidental) to the best (Functional). Yegor then dives into the technical details of the LCOM metric introduced by Chidamber and Kemerer. He explains how LCOM measures the degree to which methods in a class share instance variables. A high LCOM value acts as a "code smell," indicating that the class likely violates the Single Responsibility Principle (SRP) and should be split. 

Finally, the lecture covers variants like LCOM4, which uses a graph-based approach to identify "connected components" within a class. If LCOM4 is greater than 1, it provides a mathematical proof that the class can be physically split into independent pieces. Yegor emphasizes the use of automated tools like "jpeek" to visualize and enforce these metrics in real-world projects.

## Key Insights
- "Cohesion is the glue that holds the internal parts of a module together; if the glue is weak, the module falls apart conceptually."
- "LCOM4 is the most practical version: if the value is greater than one, your class is literally two or more classes hiding in one file."
- "High cohesion is not just a 'good to have' feature; it is the primary defense against the 'God Object' anti-pattern."
- "A class with low cohesion is a burden for testers and a nightmare for future maintainers."

## Relevance: 5/5
This is a fundamental lecture for any software engineer interested in object-oriented design, as it provides a mathematical basis for the Single Responsibility Principle.
