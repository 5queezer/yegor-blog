---
title: "I23: A. S. Medvednikov | The V Programming Language - simple, fast, safe, compiled, Open Source"
date: 2024-05-28T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/xMGNlUZQ-6w/maxresdefault.jpg"
  alt: "I23: A. S. Medvednikov | The V Programming Language - simple, fast, safe, compiled, Open Source"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=xMGNlUZQ-6w](https://www.youtube.com/watch?v=xMGNlUZQ-6w)

## Summary
In this interview, Yegor Bugayenko talks with Alexander Medvednikov, the creator of the V programming language (vlang). Alexander explains that V was born out of a practical need for a language that is as simple as Go but as fast and safe as Rust, specifically for developing his high-performance messaging client, "Volt." A central theme is V's extreme compilation speed—claiming over a million lines per second—achieved through a tiny, self-bootstrapping compiler that avoids heavy dependencies like LLVM by default, instead translating to C or directly to machine code.

The discussion covers technical innovations such as V’s memory management, which aims for a middle ground between manual control and garbage collection using compile-time analysis (autofree). Alexander emphasizes safety features like the absence of null pointers, the lack of global variables, and mandatory immutability by default. They also address the skepticism from the developer community regarding V’s ambitious claims, which Alexander counters by pointing to the growing ecosystem and functional real-world applications. The conversation highlights a philosophy of radical simplicity: providing only one way to solve a problem and keeping the language's core small enough to be understood by a single developer.

## Key Insights
- "V is designed to be a language without legacy; it takes the best from Go, Rust, and Oberon but removes the complexity."
- "Compiling at 1.2 million lines per second isn't just a gimmick; it fundamentally changes the developer's feedback loop."
- "Safety shouldn't be an academic exercise; it's about preventing common mistakes like null dereferencing and global state corruption through strict language rules."

## Relevance: 5/5
Extremely relevant for engineers interested in language design, compiler performance, and the trade-offs between safety and simplicity in system programming.
