---
title: "OSBP 3/8: Making Changes"
date: 2024-03-27T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/D6CUW9eZ5yk/maxresdefault.jpg"
  alt: "OSBP 3/8: Making Changes"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=D6CUW9eZ5yk](https://www.youtube.com/watch?v=D6CUW9eZ5yk)

## Summary
In the eighth installment of his "Open Source Best Practices" series, Yegor Bugayenko explores the technical and psychological nuances of contributing code to open-source projects. He frames a Pull Request (PR) as a commercial transaction where the contributor serves as the salesperson and the maintainer acts as the customer. The central premise is that for a "sale" to occur, the contributor must minimize friction and cognitive load for the buyer. This leads to the most critical advice of the session: keep your Pull Requests radically small. Bugayenko argues that a one-line PR is often superior to a 500-line submission because massive changes create a "moral dilemma" for maintainers, often leading to procrastination or outright rejection due to the hidden complexity. Small, incremental changes are much easier to verify and merge, significantly accelerating the overall development velocity.

Furthermore, Bugayenko emphasizes the principle of atomicity—one PR should address exactly one isolated issue. Combining multiple fixes into a single submission is a tactical mistake; if a maintainer disagrees with even a single minor point, the entire contribution may be stalled indefinitely. He also introduces the concept of being the "leader" or "boss" of your PR. Once a PR is submitted, the responsibility for its integration lies solely with the author. This involves proactively monitoring CI results, navigating style critiques without taking them personally, and politely following up if the submission is ignored. He suggests that descriptions should focus on the "Why" (the motivation and business value) rather than the "What" (the technical implementation), as the code itself should be self-explanatory to a competent reviewer. By citing academic research from experts like Bram Adams, Caitlin Sadowski, and Marco Ortu, Bugayenko provides a rigorous foundation for these practices, highlighting how PR size and the emotional "valence" of review comments directly impact the success of collaborative software engineering.

## Key Insights
- "A Pull Request is a transaction. You are the salesperson, the maintainer is the customer."
- "Small PRs are merged much faster. Even a one-line PR is perfectly acceptable."
- "You are the leader of the transaction. If the PR fails to merge, it is your failure."
- "Explain the 'Why', not the 'What'. The code itself shows what was changed."

## Relevance: 5/5
Essential for effective collaboration in distributed teams and open-source environments, focusing on reducing reviewer friction and improving merge velocity.
