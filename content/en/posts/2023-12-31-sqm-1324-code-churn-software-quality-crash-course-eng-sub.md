---
title: "SQM 13/24: Code Churn [software quality crash course]"
date: 2023-12-31T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/dvuyJ5LvHvQ/maxresdefault.jpg"
  alt: "SQM 13/24: Code Churn [software quality crash course]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=dvuyJ5LvHvQ](https://www.youtube.com/watch?v=dvuyJ5LvHvQ)

## Summary
In this lecture, Yegor Bugayenko explores the concept of "Code Churn" as a vital metric for software quality management. Unlike static metrics such as Lines of Code (LoC), which only provide a snapshot of the current project size, Code Churn measures the evolutionary dynamics of the codebase—how much code is added, deleted, or modified over a specific period. Yegor argues that the history of changes is far more revealing than the current state of the code.

A central theme is the research by Nagappan and Ball (2005), which demonstrates that "Relative Code Churn" is a superior predictor of defect density compared to traditional metrics. Files that undergo frequent and massive changes are identified as "hotspots." These areas are statistically more likely to contain bugs, often indicating unstable requirements, architectural flaws, or a lack of developer understanding.

Yegor also introduces his proprietary metric, Hits-of-Code (HoC). He criticizes LoC for failing to account for refactoring; if a developer deletes 1,000 lines of messy code, their LoC contribution appears negative, despite high effort. HoC, by contrast, is the cumulative sum of all changes recorded in Git and always increases, providing a more honest representation of developer productivity and business value. Ultimately, the lecture advocates for using churn data from version control systems to proactively identify risks and manage technical debt.

## Key Insights
- "Quality is not just about how the code looks now; it's about how much it's changing."
- "Hits-of-Code (HoC) shows the business that you actually worked, even if you deleted more code than you added."
- "Files with high relative churn are 'hotspots'—we don't need to wait for bugs to appear to know they are there."
- "A manager's goal should be to reduce the churn rate of unstable modules, not just to increase the feature count."

## Relevance: 5/5
This lecture provides high-value insights for team leads and architects on using empirical data (Git history) to predict risks and justify refactoring to management.
