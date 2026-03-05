---
title: "SQM 14/24: Technical Debt [Software Quality Crash Course]"
date: 2024-01-03T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/pvZDcytPU3w/maxresdefault.jpg"
  alt: "SQM 14/24: Technical Debt [Software Quality Crash Course]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=pvZDcytPU3w](https://www.youtube.com/watch?v=pvZDcytPU3w)

## Summary
In this lecture from his Software Quality Management (SQM) course, Yegor Bugayenko presents a disciplined and architectural perspective on "Technical Debt." The core of his argument lies in a strict binary distinction: code is either "Technical Debt" or "Technical Mess." Debt is a strategic, intentional choice to bypass quality standards temporarily to meet a specific business milestone, provided it is formally tracked in a task management system. In contrast, "Mess" is simply low-quality code that exists because of developer negligence or lack of process, which remains undocumented and invisible.

Drawing heavily on Ward Cunningham’s original metaphor, Yegor explains that technical debt functions like a financial loan. It allows a team to "buy time" in the present, but it comes with mandatory "interest" payments. These interest payments manifest as the increased effort and time required to implement every subsequent feature due to the complexity and fragility of the compromised code. He warns that if this debt is not systematically repaid through refactoring, the interest can eventually exceed the team's capacity to deliver new value, leading to "technical bankruptcy."

To manage this, Yegor advocates for Puzzle Driven Development (PDD). He argues that traditional `// TODO` comments are ineffective because they are passive and often ignored. PDD requires developers to leave structured "puzzles" in the code that are automatically converted into tracked GitHub issues. This ensures that the debt is visible to management and can be prioritized alongside new features. Ultimately, the lecture emphasizes that managing debt is a process-level responsibility, where the architect acts as a financial officer deciding which "loans" are worth taking to ensure long-term project viability.

## Key Insights
1. "If it is not in the task tracker, it is not technical debt; it is just a technical mess."
2. "Technical debt is a conscious trade-off where you borrow productivity from the future to gain speed today."
3. "The interest on technical debt is a tax you pay on every single new line of code you write in a cluttered system."
4. "Puzzle Driven Development (PDD) turns the passive hope of refactoring into an active, tracked, and manageable task."

## Relevance: 5/5
This content is essential for senior developers and architects who need to balance business pressure with long-term maintainability. It provides a formal framework for discussing quality with non-technical stakeholders.
