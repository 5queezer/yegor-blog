---
title: "SQM 18/24: Defects Density"
date: 2024-02-21T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/M-yHXzROVno/maxresdefault.jpg"
  alt: "SQM 18/24: Defects Density"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=M-yHXzROVno](https://www.youtube.com/watch?v=M-yHXzROVno)

## Summary
In this lecture from his Software Quality Management (SQM) course, Yegor Bugayenko explores the metric of "Defect Density" and challenges conventional wisdom regarding code size and complexity. Defect density is defined as the number of confirmed bugs divided by the size of the software, typically measured in thousands of lines of code (KLOC). The core of the discussion centers on a research study by Yamashita et al., which Yegor’s team replicated, investigating the relationship between file size, complexity thresholds, and the actual prevalence of bugs.

The most provocative takeaway is the debunking of the "smaller is better" myth. While industry best practices often suggest splitting large files into smaller components to improve quality, the data suggests a paradox: larger files often exhibit a lower defect density than smaller ones. Yegor explains that when a complex module is fragmented into many smaller pieces to satisfy arbitrary line-count limits, the complexity does not vanish. Instead, it shifts from the internal logic of a single file to the interactions and dependencies between the new, smaller files. These inter-file interactions are frequently harder to track and more prone to integration errors, potentially increasing the total bug count. Ultimately, the lecture concludes that rigid thresholds for size or cyclomatic complexity are unreliable predictors of quality, and refactoring should prioritize clarity over meeting metric-based quotas.

## Key Insights
- "Defect density is not just about the number of bugs, but about how many bugs exist relative to the volume of code (KLOC)."
- "Splitting a large file into ten smaller ones doesn't eliminate complexity; it merely moves it from internal logic to the interactions between those files."
- "Counter-intuitively, research shows that larger files often have a lower defect density than their smaller, fragmented counterparts."
- "Size and complexity thresholds are often misleading indicators that fail to accurately predict where the next bug will appear."

## Relevance: 5/5
This lecture is highly relevant for lead developers and architects who often enforce "clean code" rules without considering the architectural trade-offs of over-modularization.
