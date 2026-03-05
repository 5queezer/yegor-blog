---
title: "SQM 20/24: Commits Density"
date: 2024-03-17T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/BrG3HiuYC5U/maxresdefault.jpg"
  alt: "SQM 20/24: Commits Density"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=BrG3HiuYC5U](https://www.youtube.com/watch?v=BrG3HiuYC5U)

## Summary
In this lecture from the Software Quality Metrics (SQM) course, Yegor Bugayenko explores the concept of "Commits Density" as a crucial metric for evaluating software development discipline. He defines this metric in two ways: temporal density (commits per unit of time, such as per day) and structural density (commits relative to the volume of code changed, such as per thousand lines of code). Bugayenko argues that higher commit density directly correlates with higher software quality.

Instead of making massive "big bang" changes, developers should break their work down into small, frequent commits. This approach offers several major advantages. First, it significantly improves traceability, making it much easier to pinpoint exactly when and why a bug was introduced (for instance, by using `git bisect`). Second, smaller changes are much easier and faster for peers to review thoroughly. Large commits often bundle unrelated changes, overwhelming reviewers and making rollbacks or partial reverts nearly impossible. Bugayenko emphasizes that high commit density is a prerequisite for effective Continuous Integration (CI), ensuring the codebase remains in a releasable state while minimizing painful merge conflicts.

## Key Insights
- "Higher commit density is a direct indicator of strong engineering discipline and leads to higher code quality."
- "Small, frequent commits make peer reviews meaningful and prevent the merging of hidden defects."
- "Massive 'big bang' commits are highly risky; they bundle unrelated changes and make partial rollbacks impossible."
- "Frequent integration reduces merge conflicts and keeps the project in a continuous state of readiness."

## Relevance: 5/5
Extremely relevant for software engineering and team management. It emphasizes practical version control discipline, directly impacting code review quality, CI/CD effectiveness, and overall project maintainability.
