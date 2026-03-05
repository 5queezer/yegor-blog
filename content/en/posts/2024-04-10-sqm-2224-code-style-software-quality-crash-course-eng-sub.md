---
title: "SQM 22/24: Code Style [software quality crash course]"
date: 2024-04-10T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/hPZGoEAXwY0/maxresdefault.jpg"
  alt: "SQM 22/24: Code Style [software quality crash course]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=hPZGoEAXwY0](https://www.youtube.com/watch?v=hPZGoEAXwY0)

## Summary
In this lecture from his "Software Quality Management" series, Yegor Bugayenko argues that code style is a fundamental metric for software maintainability rather than a subjective matter of aesthetics. He traces the evolution of code style from early foundational works like Brian Kernighan’s *The Elements of Programming Style* (1974) to modern empirical research. The core thesis is that "beautiful" code is objectively superior because it minimizes cognitive load for maintainers. 

Bugayenko advocates for the total elimination of individual "creativity" in formatting. He insists that a professional codebase should look as if it were written by a single person. To achieve this, he promotes the use of strict, automated "quality gates" using tools like Checkstyle or RuboCop. His stance is uncompromising: style enforcement must be binary—if the code violates even a single rule, the build must fail. This discipline transforms style from a matter of "good taste" into a rigorous engineering standard that prevents technical debt and improves long-term project viability.

## Key Insights
- "Code style is not about beauty; it is strictly about maintainability and reducing the cost of change."
- "The build must fail if the style is not perfect. There is no middle ground in automated enforcement."
- "The goal of a style guide is to make the entire codebase look like it was written by one person, not a team of individual artists."
- "If a human or an AI cannot easily interpret the structure of your code, the style has failed its primary purpose."

## Relevance: 5/5
This lecture is essential for senior engineers and team leads. It provides the philosophical and practical framework for enforcing consistency in large teams, which is critical for scaling software development.
