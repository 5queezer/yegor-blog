---
title: "SQM 1/24: Lines of Code [Software Quality Crash Course]"
date: 2023-09-27T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/q9Gr2xguP5I/maxresdefault.jpg"
  alt: "SQM 1/24: Lines of Code [Software Quality Crash Course]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=q9Gr2xguP5I](https://www.youtube.com/watch?v=q9Gr2xguP5I)

## Summary
In this lecture, Yegor Bugayenko explores the fundamental role of metrics in software engineering, grounded in the management axiom: "You can only control what you can measure." He distinguishes between the "Engineer," who solves isolated problems, and the "Scientist," who seeks generalized, measurable truths. The core of the discussion focuses on Lines of Code (LoC). While famously criticized by Bill Gates as a poor measure of progress—likening it to measuring aircraft construction by weight—Yegor argues that LoC remains a vital metric when viewed correctly. Instead of progress, LoC should be seen as a measure of the "maintenance burden" and complexity. 

The lecture introduces Non-Commenting Source Statements (NCSS) to filter out noise like comments and whitespace. However, Yegor proposes a more dynamic alternative: Hits-of-Code (HoC). Unlike static LoC, HoC tracks every modification in Git, ensuring the metric always increments and reflects the true effort invested, even when code is deleted or refactored. Furthermore, he addresses code "smells," specifically targeting empty lines within methods as a sign of fragmented logic; a method should be cohesive enough to require no internal separation. Finally, Yegor advocates for a "suffering" approach to static analysis, where developers manually fix style violations rather than using auto-formatters, arguing that this friction is necessary for long-term learning and architectural discipline.

## Key Insights
- "Measuring programming progress by lines of code is like measuring aircraft building progress by weight." (Bill Gates, cited by Yegor)
- "You can only control what you can measure; without metrics, software quality is just an opinion."
- "Hits-of-Code (HoC) is superior to LoC because it captures the history of effort and the 'hotspots' of complexity."
- "Empty lines inside a method are a code smell; if you need to separate blocks of code, your method is doing too much."

## Relevance: 5/5
This lecture is highly relevant for team leads and architects as it reclaims a controversial metric (LoC) as a tool for cost estimation and maintenance management while introducing more modern alternatives like HoC.
