---
title: "First Signs of High Quality in Software Engineering"
date: 2023-04-13T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/5PLqi79uA0s/maxresdefault.jpg"
  alt: "First Signs of High Quality in Software Engineering"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=5PLqi79uA0s](https://www.youtube.com/watch?v=5PLqi79uA0s)

## Summary
In this lecture, Yegor Bugayenko outlines the foundational indicators of high quality within a software engineering project. He argues that quality is not merely the absence of bugs, but the presence of a rigorous, disciplined process. A primary sign of quality is the transformation of code review into a professional "battlefield" where the author and reviewer act as opponents. The reviewer's goal is to find flaws, while the author must defend their solution using objective standards. Subjective opinions, such as "I don't like this approach," are dismissed; every critique must reference a documented rule, standard, or automated metric.

Responsibility is another cornerstone of high quality. Bugayenko insists on a clear shift: before a merge, the author is solely accountable for failures; however, once the code is integrated into the main branch, it becomes the property and responsibility of the entire team, specifically the reviewer who approved it. Furthermore, high quality is impossible without total automation. If code style or basic errors are checked manually rather than through linters and CI pipelines, the process is flawed. He advocates for a "Read-only Master" policy where no one, regardless of seniority, can bypass automated checks. Finally, Bugayenko warns against "heroism." In a high-quality project, there are no indispensable heroes saving the day at midnight; instead, success is the result of consistent, almost boring adherence to strict protocols and automated constraints.

## Key Insights
* "Reviewers should be opponents, not friends; their job is to stop bad code from entering the system."
* "Before the merge, it is your fault; after the merge, it is our fault."
* "Quality is a boring, repetitive discipline, not a series of heroic acts."
* "Subjective opinions have no place in code review; if there is no written rule, there is no valid comment."

## Relevance: 5/5
This video is highly relevant for anyone looking to transition from "coding" to professional software engineering, emphasizing the structural and cultural shifts necessary for long-term project stability.
