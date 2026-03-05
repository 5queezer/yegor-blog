---
title: "EQSP 3/20: CI and DevOps with GitHub Actions [software quality crash course]"
date: 2022-09-06T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/c2_h7CMzUgA/maxresdefault.jpg"
  alt: "EQSP 3/20: CI and DevOps with GitHub Actions [software quality crash course]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=c2_h7CMzUgA](https://www.youtube.com/watch?v=c2_h7CMzUgA)

## Summary
In this lecture from his "Software Quality Crash Course," Yegor Bugayenko explores the practical and philosophical aspects of Continuous Integration (CI) and DevOps, specifically using GitHub Actions. He redefines CI not merely as a set of tests, but as a "protection mechanism" designed to keep low-quality code out of the main repository. The core of his approach is the "Read-Only Master" principle: developers should never push directly to the master branch. Instead, all changes must pass through a rigorous, automated pipeline that includes unit tests (Maven), style checks (Xcop), quality metrics (Kulis), and security scanning (Snyk).

Bugayenko emphasizes the use of GitHub Actions for its YAML-based configuration and free infrastructure for open-source projects. He demonstrates advanced features like matrix builds to test across different JDK versions simultaneously. A significant portion of the lecture is dedicated to "Rulor," a custom chatbot that manages the merging process. By using commands like `@rulor merge`, the bot creates an isolated environment, performs the merge locally, runs the entire suite of checks, and only pushes to master if everything passes. This shifts the responsibility for quality from the individual programmer to the "system," ensuring that if a bug reaches production, it is viewed as a failure of the pipeline rather than the person.

## Key Insights
- "Quality happens when you intentionally and explicitly remove the bad parts."
- "Master is sacred: never push directly to the main branch; let the robots protect it."
- "Blame the system, not the person: if a bug reaches master, your CI pipeline has failed."
- "Every line of code must be linked to a ticket; no intent means no code."

## Relevance: 5/5
Extremely high relevance for modern software engineering. It provides a blueprint for building high-integrity delivery pipelines and fostering a culture of automated accountability.
