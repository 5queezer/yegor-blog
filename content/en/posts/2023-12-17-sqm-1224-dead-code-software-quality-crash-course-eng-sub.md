---
title: "SQM 12/24: Dead Code [software quality crash course] [eng sub]"
date: 2023-12-17T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/zN0gX9m6a2k/maxresdefault.jpg"
  alt: "SQM 12/24: Dead Code [software quality crash course] [eng sub]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=zN0gX9m6a2k](https://www.youtube.com/watch?v=zN0gX9m6a2k)

## Summary
In his lecture "SQM 12/24: Dead Code," part of the Software Quality Metrics crash course, Yegor Bugayenko addresses the pervasive issue of dead code and its detrimental impact on software maintainability. Dead code—code that is either never executed or whose results are completely unused—is categorized as a severe "bad smell" in object-oriented programming. Bugayenko emphasizes that its presence artificially inflates cognitive load for developers, making refactoring significantly more difficult and accelerating "bit rot." He explains how static analysis tools and modern compilers handle Dead Code Elimination (DCE), but argues that developers must actively prune their codebases rather than relying solely on automated tools to clean up after them.

A major, and perhaps controversial, segment of the lecture pivots to repository architecture, specifically comparing Monolithic repositories (Monorepos) with Polyrepos ("Manyrepos"). While acknowledging that tech giants like Google and Facebook successfully utilize monorepos to reduce integration overhead, Bugayenko strongly critiques this approach for the majority of teams. He argues that monorepos inevitably lead to compromised code quality, blurred boundaries, and poor encapsulation. Instead, he advocates for the Manyrepo strategy. By breaking projects into smaller, decoupled repositories, teams can achieve faster independent builds, enforce stricter encapsulation, maintain cleaner metrics, and simplify the testing pipeline. Finally, he introduces the concept of code "volatility"—measuring how frequently files change—to identify stagnant areas that may conceal dead code.

## Key Insights
- "Dead code is not just harmless text; it is a liability that actively increases the cognitive load and slows down future refactoring."
- "While monorepos might solve integration headaches, they often do so at the fatal cost of encapsulation and code quality."
- "Code that doesn't change is code that rots. High volatility is a sign of life, whereas stagnant code often masks dead or irrelevant logic."
- "Do not rely exclusively on the compiler's Dead Code Elimination; keeping the codebase strictly pruned is the developer's direct responsibility."

## Relevance: 5/5
This lecture is highly relevant to software engineering and team management. It directly tackles the daily challenges of codebase maintenance, refactoring, and high-level architectural decisions (Monorepo vs. Manyrepo) that dictate a team's long-term velocity and code quality.
