---
title: "SQM 21/24: Builds [software quality crash course]"
date: 2024-04-03T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/QQUda0fAcxE/maxresdefault.jpg"
  alt: "SQM 21/24: Builds [software quality crash course]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=QQUda0fAcxE](https://www.youtube.com/watch?v=QQUda0fAcxE)

## Summary
In this lecture, Yegor Bugayenko explores the historical evolution and technical metrics of software builds within the context of Software Quality Management (SQM). He traces the concept from early 1990s milestones, such as Microsoft’s "Daily Build and Smoke Test," through the rise of Extreme Programming (XP) in 1998, to the formalization of Continuous Integration (CI) by Martin Fowler and Continuous Delivery (CD) by Jez Humble.

A significant portion of the lecture is dedicated to analyzing build metrics and the distribution of build times. Yegor highlights a critical industry "pain point": **flaky tests**. He argues that non-deterministic tests—those that fail and then pass upon a simple restart—are a major threat to software quality because they destroy the team's trust in the CI process. If developers stop taking build failures seriously, the CI ceases to function as an effective quality gate. The lecture also covers CI at scale, referencing research on how large organizations manage thousands of builds daily, and emphasizes the importance of measuring the "Time to Fix" and the "Flakiness Ratio" to maintain a professional development environment.

## Key Insights
- "A build is not just a technical step; it is a formal statement that the code meets the project's quality standards."
- "The biggest enemy of a healthy CI process is the 're-run' button. Flaky tests destroy the developer's trust in the automation."
- "Continuous Integration is not a tool like Jenkins or GitHub Actions; it is a practice of integrating work multiple times a day."
- "Failed builds should happen fast. The most expensive waste of time is a build that fails after running for an hour."

## Relevance: 5/5
This lecture is highly relevant for lead developers and architects. It moves beyond "how to use a tool" and explains the "why" behind build automation as a cornerstone of software quality and team discipline.
