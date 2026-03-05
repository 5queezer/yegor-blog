---
title: "SQM 2/24: Cyclomatic Complexity by Thomas J. McCabe"
date: 2023-09-30T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/Cvv0Olx4Bpw/maxresdefault.jpg"
  alt: "SQM 2/24: Cyclomatic Complexity by Thomas J. McCabe"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=Cvv0Olx4Bpw](https://www.youtube.com/watch?v=Cvv0Olx4Bpw)

## Summary
Yegor Bugayenko delivers a compelling lecture on Thomas J. McCabe’s 1976 seminal work regarding Cyclomatic Complexity (CC). He frames complexity not merely as a technical side effect, but as a deliberate choice that reflects a developer's professionalism and respect for future maintainers. Using the "eye pain metric" as a humorous starting point, Yegor argues that if code is difficult to read, it is inherently risky and expensive to maintain. The core of the session defines CC as the number of linearly independent paths through a program's source code, calculated using the graph-theory-based formula $V(G) = E - N + 2$.

A significant portion of the talk addresses the tension between CC and Lines of Code (LoC). While the two metrics are statistically correlated, Yegor highlights that CC specifically targets logical density. He cites empirical evidence showing that high CC is a leading indicator of defect density and testing difficulty. Following McCabe’s original guidelines, Yegor advocates for a strict threshold—typically a CC of 10—above which functions must be refactored or justified. The most practical takeaway is the link to testing: CC equals the minimum number of test cases required for complete branch coverage. Yegor concludes that "good" software engineering is the art of solving complex requirements with simple, low-CC code, facilitated by automated quality gates in modern CI/CD pipelines to prevent technical debt.

## Key Insights
* "Complexity is a choice that a programmer makes; it is not forced upon you by the requirements."
* "Cyclomatic complexity is the minimum number of tests you need to write to cover all paths."
* "Writing complex code is a sign of disrespect toward future maintainers and the team."
* "The formula $V(G) = E - N + 2$ is a mathematical way to quantify risk and maintainability in your logic."

## Relevance: 5/5
Cyclomatic complexity is a fundamental metric for code quality, testing strategy, and risk management in software engineering and OOP.
