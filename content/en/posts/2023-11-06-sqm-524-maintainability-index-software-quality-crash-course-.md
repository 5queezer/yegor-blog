---
title: "SQM 5/24: Maintainability Index"
date: 2023-11-06T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
  - "ai"
cover:
  image: "https://img.youtube.com/vi/xnSnPfVkmkM/maxresdefault.jpg"
  alt: "SQM 5/24: Maintainability Index"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=xnSnPfVkmkM](https://www.youtube.com/watch?v=xnSnPfVkmkM)

## Summary
In this lecture from the Software Quality Management (SQM) series, Yegor Bugayenko explores the **Maintainability Index (MI)**, a metric designed to quantify how easy it is to support and evolve a software system. The session begins by grounding the topic in the foundational theories of Fred Brooks (essential vs. accidental complexity) and Ward Cunningham’s concept of technical debt. Bugayenko explains that MI was developed in the early 1990s by Paul Oman and Jack Hagemeister to move software evaluation from subjective "feelings" to objective data.

The original MI formula is a polynomial calculation involving three key variables: **Halstead Volume** (information content), **McCabe’s Cyclomatic Complexity** (logic paths), and **Lines of Code (LOC)**. A fourth optional variable, comment density, is sometimes included. Bugayenko highlights how Microsoft popularized a normalized version of this index (0 to 100) within Visual Studio, where scores below 10 indicate "red" or problematic code. However, the lecture takes a critical turn by discussing researchers like Arie van Deursen, who argue that MI can be "harmful." Because the metric is heavily weighted by LOC, it can be easily "gamed"—for example, by removing comments or shortening names to artificially inflate the score without actually improving the code's quality or readability. Ultimately, Bugayenko suggests using MI as a "smoke test": it can signal when something is wrong, but it should never be the sole arbiter of architectural health.

## Key Insights
*   "The Maintainability Index is an attempt to reduce the human feeling of 'messy code' into a single, objective mathematical number."
*   "Because MI is so dependent on Lines of Code, it is easy to 'game' the metric without actually making the software better."
*   "Use the Maintainability Index as a 'smoke test'—it can tell you that there is fire, but it cannot tell you that the house is perfectly built."

## Relevance: 4/5
This lecture is highly relevant for team leads and architects who need to measure technical debt but must understand the limitations of automated quality metrics.
