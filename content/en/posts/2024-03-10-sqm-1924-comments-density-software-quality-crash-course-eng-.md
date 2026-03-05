---
title: "SQM 19/24: Comments Density [software quality crash course]"
date: 2024-03-10T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/4_SNhBeyato/maxresdefault.jpg"
  alt: "SQM 19/24: Comments Density [software quality crash course]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=4_SNhBeyato](https://www.youtube.com/watch?v=4_SNhBeyato)

## Summary
In this lecture from the Software Quality Metrics (SQM) course, Yegor Bugayenko discusses "Comments Density" as a metric for evaluating codebase health. The core premise is that the ratio of comments to code is an important indicator, but only if we distinguish between different types of comments. Bugayenko draws a strict line between API documentation (like Javadoc or Doxygen) and inline comments placed inside method bodies. 

He argues that class-level and method-level documentation is mandatory and highly beneficial, as it defines the "what" and "why" of the software components, establishing clear contracts for users of the API. Consequently, a high density of API documentation is a sign of a high-quality, maintainable project. 

Conversely, inline comments are considered a severe code smell. If a developer feels compelled to write a comment explaining *how* a specific block of code works, it means the code itself is too complex or poorly named. The solution is not to add a comment, but to refactor the code—usually by extracting smaller, well-named methods or objects that are self-explanatory. Furthermore, comments are not executable and often fall out of sync with the actual code, leading to misleading "lies" in the repository. Ultimately, Bugayenko advocates for maximizing architectural documentation while driving inline comment density to absolute zero.

## Key Insights
- "Inline comments are a code smell; if you have to explain how your code works, you should refactor it instead."
- "There is a strict difference between API documentation (the contract) and internal comments (the implementation)."
- "Code never lies, but comments easily become outdated and turn into lies that confuse future developers."
- "A high-quality codebase maximizes the density of API documentation while keeping inline comment density at zero."

## Relevance: 5/5
This topic is highly relevant for software engineers and team leads, as it establishes clear rules for code maintainability, refactoring, and documentation practices within object-oriented programming.
