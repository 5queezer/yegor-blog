---
title: "PPA 10/10: Code Analysis With Machine Learning [program analysis crash course]"
date: 2023-05-19T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/6Z1EFTJ7Kdo/maxresdefault.jpg"
  alt: "PPA 10/10: Code Analysis With Machine Learning [program analysis crash course]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=6Z1EFTJ7Kdo](https://www.youtube.com/watch?v=6Z1EFTJ7Kdo)

## Summary
In this final installment of the Program Analysis series, Yegor Bugayenko explores the emerging field of "Big Code," which applies Machine Learning (ML) techniques to software engineering. The lecture contrasts traditional static analysis, which relies on expert-defined rules and formal logic, with probabilistic models trained on massive datasets from platforms like GitHub. Bugayenko explains that because code is a human-generated artifact, it possesses "naturalness"—repetitive patterns and statistical regularities similar to human language. This makes it possible to use ML for tasks that are difficult to hard-code, such as predicting meaningful variable names, detecting subtle logic bugs, and automating code reviews.

A significant portion of the talk is dedicated to code representation. Bugayenko describes how code is transformed into a format machines can understand, moving beyond simple text tokens to structural representations like Abstract Syntax Trees (ASTs) and Control Flow Graphs (CFGs). He highlights "Code2Vec" as a pivotal technology that uses path-based embeddings to represent the semantics of a code snippet as a mathematical vector. However, he remains critical of the "black box" nature of current ML models. Unlike traditional linters that provide a clear rationale for a warning (e.g., "variable not initialized"), ML models often struggle with explainability, offering a probability of an error without a logical justification. This lack of interpretability remains the primary barrier to replacing deterministic analysis tools with AI-driven ones in production environments.

## Key Insights
- "Code is natural; it has the same statistical properties as human language, which makes it an ideal candidate for probabilistic machine learning models."
- "The shift from manually crafted heuristics to 'Big Code' allows us to find patterns in software that no human expert could ever document in a set of rules."
- "The fundamental problem with ML in program analysis is the lack of explainability; a developer needs to know 'why' a piece of code is flagged as a bug, not just that it probably is."
- "We are moving from a world of deterministic correctness to a world of probabilistic suggestions, where the goal is to augment human intuition with global data."

## Relevance: 5/5
This lecture is highly relevant as it bridges the gap between formal computer science and modern AI, providing a realistic look at how LLMs and ML tools actually perceive and process source code.
