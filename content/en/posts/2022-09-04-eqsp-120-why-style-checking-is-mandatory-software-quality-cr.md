---
title: "Why Style Checking is Mandatory?"
date: 2022-09-04T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/ZeraaVNW1mo/maxresdefault.jpg"
  alt: "Why Style Checking is Mandatory?"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=ZeraaVNW1mo](https://www.youtube.com/watch?v=ZeraaVNW1mo)

## Summary
In this lecture, Yegor Bugayenko argues that automated style checking is not a matter of aesthetics, but a fundamental pillar of professional software development and team discipline. He posits that style checkers act as an impartial "judge" that eliminates subjective conflicts during code reviews. Without automation, reviews often devolve into personal arguments over formatting, which wastes expensive human time and creates friction between developers. By delegating these "cosmetic" decisions to a tool (like Checkstyle or RuboCop), the team moves from debating opinions to following a project-wide law.

Yegor further explains that a developer’s attention to style is a "litmus test" for their overall professional discipline. If a programmer is indifferent to messy formatting or inconsistent naming, they are likely to be equally negligent regarding deeper architectural issues or memory management. Quality cannot be achieved through meetings or "asking nicely"; it must be enforced by the build system. The rule is simple: if the style check fails, the build fails, and the code cannot be merged. This creates a "robot-led" workflow where humans focus on logic and "why" the code exists, while machines handle the "how" it looks. Ultimately, style checking is a tool for building a system that forces quality rather than one that merely hopes for it.

## Key Insights
- "A style checker is like a judge for us; it is no longer my opinion versus your opinion, it is the tool's decision."
- "If a programmer doesn't pay attention to the style of the code, they will not pay attention to the quality of the code."
- "Don't blame people for bad code, blame the system that allowed it to be merged."
- "Human reviewers should focus on logic and architecture; let the robots handle the spaces and brackets."

## Relevance: 5/5
This is a foundational concept for team management and CI/CD pipelines, emphasizing that automation is the only way to scale quality.
