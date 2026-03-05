---
title: "SQM 3/24: Cognitive Complexity by G. Ann Campbell [software quality crash course]"
date: 2023-10-03T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/oRUux3w4rsc/maxresdefault.jpg"
  alt: "SQM 3/24: Cognitive Complexity by G. Ann Campbell [software quality crash course]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=oRUux3w4rsc](https://www.youtube.com/watch?v=oRUux3w4rsc)

## Summary
In this lecture from his "Software Quality Metrics" series, Yegor Bugayenko explores the limitations of traditional Cyclomatic Complexity (CC) and presents Cognitive Complexity (CoCo) as a more human-centric alternative. The core thesis is that while Thomas McCabe’s Cyclomatic Complexity is a robust mathematical model for determining testability (i.e., the number of paths requiring unit tests), it fails to account for how difficult code is for a developer to actually understand and maintain.

Bugayenko details the three fundamental rules of Cognitive Complexity proposed by G. Ann Campbell of SonarSource. First, the metric ignores "syntactic sugar"—modern language features like method chaining or null-coalescing operators that condense logic without adding mental strain. Second, it increments for every break in the linear, top-to-bottom flow of execution (such as `if`, `for`, and `catch` statements). Third, and most importantly, it applies a "nesting penalty." Unlike CC, which treats nested structures linearly, CoCo increases the weight of a statement based on its depth. An `if` statement nested three levels deep is significantly more "expensive" than one at the top level, reflecting the increased mental effort required to track state.

The lecture also delves into the scientific validation of these metrics. Yegor discusses the use of EEG (electroencephalogram) headsets to measure actual brain activity while developers read code, proving that nesting correlates with higher cognitive load. Finally, he touches on "social code analysis," emphasizing that the ultimate goal of a metric is to predict real-world outcomes like bug frequency and maintenance costs within a team.

## Key Insights
- "Cyclomatic complexity measures the effort to test code, whereas cognitive complexity measures the effort to understand it."
- "Nesting is the primary enemy of readability; every level of indentation adds a layer of mental state a developer must maintain."
- "Modern metrics must be validated biologically—using tools like EEG to confirm that what we call 'complex' actually taxes the human brain."
- "A good metric is a predictive tool for team management, identifying which parts of the codebase will become future 'bug magnets'."

## Relevance: 5/5
This is highly relevant for software architects and team leads who need objective ways to enforce maintainability and prevent the accumulation of technical debt.
