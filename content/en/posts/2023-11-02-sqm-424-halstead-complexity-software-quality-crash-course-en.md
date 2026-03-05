---
title: "SQM 4/24: Halstead Complexity [software quality crash course]"
date: 2023-11-02T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/YsGzjv0hgcc/maxresdefault.jpg"
  alt: "SQM 4/24: Halstead Complexity [software quality crash course]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=YsGzjv0hgcc](https://www.youtube.com/watch?v=YsGzjv0hgcc)

## Summary
In this lecture, Yegor Bugayenko explores the concept of **Halstead Complexity**, a foundational metric in "Software Science" introduced by Maurice Halstead in 1977. Unlike Cyclomatic Complexity, which focuses on the control flow and branching of a program (e.g., `if` and `while` statements), Halstead’s approach is based on counting the fundamental building blocks of code: **operators** (keywords, symbols, function calls) and **operands** (variables, constants).

The lecture details the four basic metrics: distinct operators ($n_1$), distinct operands ($n_2$), total operators ($N_1$), and total operands ($N_2$). From these, more complex indicators are derived, most notably **Volume ($V$)**, **Difficulty ($D$)**, and **Effort ($E$)**. Yegor emphasizes that **Effort ($E = D \times V$)** is the most critical takeaway for software engineers, as it attempts to quantify the mental energy and time required for a person to understand or implement a specific algorithm.

Yegor frames these metrics within the context of maintainability and the "cost of code." He argues that while Halstead's work is decades old and sometimes criticized for its empirical claims, it provides a rigorous mathematical framework for understanding why "dense" code is harder to maintain. By measuring the vocabulary and density of a program, teams can identify "effort-heavy" modules that are likely to become bottlenecks for future development and debugging.

## Key Insights
* **Code as Information:** Programming isn't just about logic; it's about the density of information. Halstead metrics treat code as a stream of symbols that must be processed by the human brain.
* **The "Effort" Metric:** The most valuable aspect of Halstead's theory is the quantification of "mental effort," which directly correlates to the time spent by a developer on a task.
* **Volume vs. Difficulty:** A program can have a small volume but high difficulty if it uses a large variety of operators in a complex way, making it harder to read than a longer but simpler piece of code.
* **Scientific Foundation:** Halstead attempted to turn software engineering into a "hard science" by applying information theory to source code.

## Relevance: 4/5
Extremely relevant for understanding the cost of maintenance and the psychological aspect of code readability. It provides a quantitative basis for discussions about code cleanlines and technical debt.
