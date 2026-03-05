---
title: "SQM 15/24: Code Coverage [software quality crash course]"
date: 2024-01-17T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/pJrXQ5rptig/maxresdefault.jpg"
  alt: "SQM 15/24: Code Coverage [software quality crash course]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=pJrXQ5rptig](https://www.youtube.com/watch?v=pJrXQ5rptig)

## Summary
In this lecture, Yegor Bugayenko explores Code Coverage as a vital metric for software quality management, rather than just a technical curiosity. He defines four primary types of coverage: Statement, Branch, Condition, and Path coverage, explaining how each level adds more rigor to the testing process. The lecture provides a rich historical context, tracing the metric's evolution from academic papers in the 1960s to modern industrial standards like ISO 26262 for safety-critical systems and Google’s internal testing policies.

Central to the lecture is Yegor’s uncompromising "100% or nothing" philosophy. He argues that accepting a threshold lower than 100% (such as the common 80% target) essentially "legalizes" the presence of unverified and potentially dangerous code. For Yegor, coverage is a management tool: it must be integrated into CI/CD pipelines as a strict "Quality Gate." If the coverage percentage drops by even a fraction, the build should fail automatically. He concludes by warning against "Line Hitters"—tests that execute lines of code without performing meaningful assertions—noting that while high coverage is a necessary condition for quality, it is insufficient without Mutation Coverage to verify the actual effectiveness of the test suite.

## Key Insights
* "Code Coverage is a metric of your ignorance. It shows the part of the code you don't control at all."
* "High coverage doesn't guarantee the absence of bugs, but low coverage guarantees their presence."
* "If you agree to 80% coverage, you officially allow your programmers to write 20% of low-quality, unverified, and potentially dangerous code."
* "A test that just increases the coverage number but checks nothing is a crime against the project."

## Relevance: 5/5
This lecture is highly relevant for anyone in software engineering or management, as it challenges common industry compromises and provides a disciplined framework for using metrics to enforce code quality.
