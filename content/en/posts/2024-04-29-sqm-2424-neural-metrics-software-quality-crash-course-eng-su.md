---
title: "SQM 24/24: Neural Metrics [Software Quality Crash Course]"
date: 2024-04-29T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/6Rog8QhuXTY/maxresdefault.jpg"
  alt: "SQM 24/24: Neural Metrics [Software Quality Crash Course]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=6Rog8QhuXTY](https://www.youtube.com/watch?v=6Rog8QhuXTY)

## Summary
In the final lecture of his Software Quality Metrics (SQM) course, Yegor Bugayenko explores the transition from traditional, rule-based metrics to "Neural Metrics" driven by Machine Learning (ML) and Large Language Models (LLMs). While classic metrics like Cyclomatic Complexity or LCOM rely on deterministic formulas, neural metrics focus on pattern recognition and semantic understanding. 

Key topics include "Neural Software Analysis," where models are trained on vast code repositories to identify code smells and "semantic clones" that look different but function identically. Yegor highlights "DeepBugs," a method that detects bugs by identifying "surprising" variable names or argument mismatches that deviate from learned norms. He also discusses "code2vec," which transforms code into mathematical vectors via Abstract Syntax Tree (AST) paths to predict method names or functionality. Finally, the lecture addresses the role of LLMs in modern static analysis, suggesting they are most effective at filtering "false positives" and explaining complex warnings, though they remain "black boxes" compared to interpretable traditional metrics.

## Key Insights
- **From Rules to Patterns:** We are moving away from rigid "If-Then" rules toward probabilistic pattern recognition that understands semantic intent.
- **The Ground Truth Dilemma:** The accuracy of neural metrics is entirely dependent on the quality of training data; if trained on poor code, the model will normalize bad practices.
- **Accuracy vs. Interpretability:** Neural metrics often provide higher predictive accuracy for bugs but lack the transparency and "why" provided by traditional mathematical formulas.
- **LLMs as Noise Filters:** Current LLMs excel at reducing the noise in static analysis by identifying which warnings are relevant to the human developer.

## Relevance: 5/5
This lecture is highly relevant as it connects traditional software engineering rigor with the cutting-edge application of AI in code quality and maintenance.
