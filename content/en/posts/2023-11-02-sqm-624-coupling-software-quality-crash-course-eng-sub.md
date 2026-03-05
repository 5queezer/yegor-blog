---
title: "SQM 6/24: Coupling [software quality crash course]"
date: 2023-11-02T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/G0vN6Ah8-js/maxresdefault.jpg"
  alt: "SQM 6/24: Coupling [software quality crash course]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=G0vN6Ah8-js](https://www.youtube.com/watch?v=G0vN6Ah8-js)

## Summary
In this lecture, Yegor Bugayenko explores the concept of Coupling as a fundamental metric for software quality. Coupling measures the degree of interdependence between software modules; the more modules depend on each other, the harder the system is to maintain and change. Yegor traces the origins of this concept back to the 1970s and the work of Constantine and Myers on "Structured Design." 

The core of the discussion revolves around specific metrics: CBO (Coupling Between Objects) and DCC (Direct Class Coupling). Yegor argues that high CBO is a primary indicator of technical debt, as it makes classes fragile and difficult to test in isolation. He also introduces the "Distance of Coupling," a metric describing how far an object "travels" through method calls—the longer the distance, the more dangerous the coupling. The lecture covers various types of coupling, including temporal coupling (where methods must be called in a strict sequence) and hidden coupling (often caused by reflection or global states). The ultimate goal for a software engineer is to minimize the "strength of connection" between modules to ensure architectural stability.

## Key Insights
- "Coupling is the enemy of change; the more your modules know about each other, the less you can move them."
- "The goal of a good architect is to minimize the strength of connection between components."
- "Temporal coupling is a design flaw that should be replaced by immutable objects or proper encapsulation."
- "High CBO (Coupling Between Objects) makes a class a 'hotspot' that is sensitive to changes anywhere in the system."

## Relevance: 5/5
This is a foundational concept in OOP and system design, essential for anyone managing large-scale codebases.
