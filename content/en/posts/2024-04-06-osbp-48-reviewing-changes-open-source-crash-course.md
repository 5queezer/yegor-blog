---
title: "OSBP 4/8: Reviewing Changes [open source crash course]"
date: 2024-04-06T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/TJ83ePwyH_A/maxresdefault.jpg"
  alt: "OSBP 4/8: Reviewing Changes [open source crash course]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=TJ83ePwyH_A](https://www.youtube.com/watch?v=TJ83ePwyH_A)

## Summary
In this fourth installment of the "Open Source Best Practices" series, Yegor Bugayenko redefines the role of a code reviewer as a "gatekeeper" and an "opponent" rather than a helpful assistant. The core philosophy is that code reviews should be rigorous, strict, and focused on maintaining long-term architectural integrity rather than just checking if the code "works." Yegor argues that a reviewer should actively look for reasons to reject a Pull Request (PR) to protect the repository from "code rot" and "broken windows."

Several practical rules are established: First, a reviewer should never run the code locally. Functional correctness must be guaranteed by automated tests and CI; if a reviewer feels the need to run the code, it means the tests are insufficient. Second, large PRs (spanning dozens of files) should be rejected immediately because they are impossible to review effectively. Changes must be atomic and small. Third, for bug fixes, a PR is invalid unless it includes a "puzzle"—a test case that fails without the fix and passes with it. This ensures the bug is truly understood and permanently resolved. 

Finally, Yegor emphasizes the educational value of reviews. A reviewer should raise issues but never resolve them personally. By explaining the underlying principles and repository standards, the reviewer mentors the contributor, forcing them to improve their own work. This builds a culture of high standards where quality is never sacrificed for speed.

## Key Insights
*   **Reviewer as Opponent:** The reviewer’s primary duty is to find flaws and reject the code, acting as a filter for the repository's health.
*   **Trust the CI, Not the Local Machine:** Human time is too valuable for manual testing; functional verification belongs to the automated pipeline.
*   **No Large Pull Requests:** Small, atomic changes are the only way to ensure deep, meaningful code analysis and avoid superficial approvals.
*   **The "Puzzle" Requirement:** Every bug fix must be accompanied by a failing test case to prove the fix works and prevent regressions.

## Relevance: 5/5
This content is essential for any software lead or maintainer. It challenges the "friendly" but superficial review culture, providing a blueprint for high-quality, scalable team management and technical debt prevention.
