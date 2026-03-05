---
title: "EQSP 5-6/20: Dependency Management | Maven, Bundler, and Npm [software quality crash course]"
date: 2022-10-13T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/U5yI1mw1tJk/maxresdefault.jpg"
  alt: "EQSP 5-6/20: Dependency Management | Maven, Bundler, and Npm [software quality crash course]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=U5yI1mw1tJk](https://www.youtube.com/watch?v=U5yI1mw1tJk)

## Summary
In this lecture from the Software Quality Crash Course (EQSP), Yegor Bugayenko explores the critical challenges of dependency management in modern software development. He argues that managing dependencies is not merely about importing external libraries, but rather a rigorous discipline of risk and stability control. The core issue developers face is "Dependency Hell," primarily driven by unpredictable transitive dependencies and version conflicts. Bugayenko compares three major package managers: Maven (Java), Bundler (Ruby), and Npm (Node.js). While Maven is the industry standard despite its verbose XML, Bundler is praised for pioneering strict dependency locking via `Gemfile.lock`, ensuring reproducible builds. Npm, conversely, is critiqued for encouraging massive dependency trees that introduce significant security and stability risks. The lecture emphasizes key principles for robust dependency management: strictly locking all versions (avoiding flexible ranges like `^` or `~`), minimizing the total number of dependencies, maintaining transitive transparency, and systematically checking for vulnerabilities. Ultimately, the ideal project minimizes external dependencies to reduce security risks and improve long-term maintainability.

## Key Insights
- "Managing dependencies is a discipline of controlling risks, not just a convenience for developers."
- "The ideal project has zero dependencies; every new library introduces a potential vulnerability."
- "Strict version locking is non-negotiable for reproducible builds—avoid flexible version ranges."
- "Transitive dependencies are the root cause of dependency hell; you must control what your libraries bring with them."

## Relevance: 5/5
This lecture provides essential, highly relevant principles for software engineering and architectural stability, addressing common pitfalls in dependency management that every development team faces.
