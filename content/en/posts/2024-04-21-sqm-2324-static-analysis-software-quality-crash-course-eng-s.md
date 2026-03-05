---
title: "SQM 23/24: Static Analysis [software quality crash course]"
date: 2024-04-21T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/QK2XQvYoEpQ/maxresdefault.jpg"
  alt: "SQM 23/24: Static Analysis [software quality crash course]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=QK2XQvYoEpQ](https://www.youtube.com/watch?v=QK2XQvYoEpQ)

## Summary
In this lecture, Yegor Bugayenko explores static analysis as a fundamental pillar of Software Quality Management (SQM). He defines it as the automatic inspection of source code without execution, contrasting it with dynamic analysis (testing). The session traces the evolution of static analysis through three generations: from simple pattern matching and syntax checking (1st gen) to control flow analysis (2nd gen), and finally to complex inter-procedural and global logic analysis (3rd gen).

Yegor categorizes code issues into Style Violations, Code Smells, and actual Bugs. He emphasizes that while style might seem trivial, it impacts long-term maintainability. A significant portion of the lecture is dedicated to the technical challenges of static analysis, specifically the "noise" created by false positives. He references the SARIF standard for integrating various tools into modern CI/CD pipelines.

The most provocative part of the lecture is Yegor’s educational philosophy. He argues that static analysis should be treated as a pedagogical tool. Instead of using "auto-fixers" that silently correct code, developers should be forced to fix violations manually. This manual "suffering" ensures that the developer understands the underlying principle, eventually internalizing better coding habits and moving from "code smells" to "code perfumes."

## Key Insights
* "Static analysis is a training tool; developers should fix warnings manually to actually learn from their mistakes rather than relying on auto-fixers."
* "The goal of shifting left is to identify structural and logical flaws long before the code ever reaches a runtime environment."
* "False positives are the primary enemy of static analysis; if the noise is too high, developers will eventually ignore even the most critical bug reports."
* "We should strive for 'code perfumes'—patterns that are so clean and professional that they serve as the opposite of code smells."

## Relevance: 5/5
This lecture is essential for understanding how to enforce high standards in a team environment and automate the gatekeeping of code quality.
