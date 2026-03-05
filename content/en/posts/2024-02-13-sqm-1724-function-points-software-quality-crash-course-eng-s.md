---
title: "SQM 17/24: Function Points [software quality crash course]"
date: 2024-02-13T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/xt01nxxfAB0/maxresdefault.jpg"
  alt: "SQM 17/24: Function Points [software quality crash course]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=xt01nxxfAB0](https://www.youtube.com/watch?v=xt01nxxfAB0)

## Summary
In this lecture, Yegor Bugayenko explores Function Point Analysis (FPA) as a superior alternative to the traditional "Lines of Code" (LOC) metric for measuring software size. He begins by addressing the "productivity paradox" inherent in LOC: a developer using a low-level language like Assembly appears more productive than one using a high-level language, even if they deliver the same functionality. To solve this, Allan Albrecht of IBM introduced Function Points in 1979, shifting the focus from the implementation process to the business utility provided to the user.

Yegor details the five core components of Unadjusted Function Points (UFP): Internal Logical Files (ILF) and External Interface Files (EIF) represent data at rest, while External Inputs (EI), External Outputs (EO), and External Inquiries (EQ) represent data in motion. These elements are identified through models like Entity-Relationship diagrams and Data Flow Diagrams. The count is further refined using 14 General System Characteristics—such as performance and reusability—to produce Adjusted Function Points (AFP).

The lecture emphasizes that FPA is technology-agnostic, allowing for fair benchmarking across different programming stacks. While counting Function Points is more complex and often requires specialists or adherence to IFPUG standards, it provides a rigorous foundation for project estimation models like COCOMO-II. Yegor concludes that understanding software size through functional utility is essential for professional software management and cost prediction, as it measures what the system actually *does* for the user rather than how many characters were typed.

## Key Insights
* "Function Points move the focus from implementation (how many lines did I write?) to utility (how much functionality did the user get?)"
* "The productivity paradox: using LOC as a metric makes developers in inefficient languages look like heroes."
* "Software should be measured by the value it provides to the business, making the specific programming language irrelevant to the size of the requirement."
* "The five components (ILF, EIF, EI, EO, EQ) provide a standardized vocabulary for describing any information system's boundaries."

## Relevance: 5/5
This lecture is fundamental for anyone in software engineering management or lead roles. It provides the mathematical basis for objective productivity measurement and professional cost estimation.
