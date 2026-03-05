---
title: "OSBP 5/8: Setting Guidelines [open source crash course]"
date: 2024-04-17T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/mWi2S5FJiJ4/maxresdefault.jpg"
  alt: "OSBP 5/8: Setting Guidelines [open source crash course]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=mWi2S5FJiJ4](https://www.youtube.com/watch?v=mWi2S5FJiJ4)

## Summary
In this lecture, Yegor Bugayenko emphasizes that a successful open-source project relies on strict discipline and automated enforcement rather than social agreements. He outlines five core recommendations for repository management. First, every project must have a **License** (preferably MIT) to be legally open source. Second, the **README.md** must follow the "10-second rule," being visually attractive with badges and providing a clear problem statement and a 3-line "quick start."

Third, the **master branch must be read-only**; all changes, even from the owner, should go through Pull Requests to ensure validation. Fourth, Yegor expresses skepticism toward standard **Codes of Conduct**, suggesting that technical quality and clear contribution rules are more important than social "fluff." Finally, the most critical point is the **automation of guidelines**. Instead of writing long coding style documents, maintainers should set up GitHub Actions (linters, static analyzers, test coverage) to automatically reject any PR that doesn't meet the standards. This "management by robots" reduces conflict and saves the maintainer's time.

## Key Insights
- "The more protective you are of your master branch, the better for the health of your repository."
- "Don't waste time explaining rules in documents; if a rule matters, make it a failing build check."
- "A README is your storefront: if I don't understand what the project does in 10 seconds, I'm leaving."

## Relevance: 5/5
Essential for anyone leading a team or an open-source project, focusing on the intersection of technical discipline and workflow automation.
