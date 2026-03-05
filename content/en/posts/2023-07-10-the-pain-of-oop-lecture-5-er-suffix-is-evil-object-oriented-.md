---
title: "The Pain of OOP, Lecture #5: -ER Suffix is Evil"
date: 2023-07-10T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
  - "oop"
  - "ai"
cover:
  image: "https://img.youtube.com/vi/6GMiosTLUTc/maxresdefault.jpg"
  alt: "The Pain of OOP, Lecture #5: -ER Suffix is Evil"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=6GMiosTLUTc](https://www.youtube.com/watch?v=6GMiosTLUTc)

## Summary
In this influential lecture from "The Pain of OOP" series, Yegor Bugayenko presents a provocative critique of common naming conventions in software engineering, specifically targeting classes that end with the "-er" suffix (e.g., Manager, Controller, Helper, Validator, Parser). Bugayenko argues that these names are not merely a matter of aesthetics but are clear indicators of procedural thinking masquerading as Object-Oriented Programming (OOP). According to his "Elegant Objects" philosophy, a true object should be defined by "what it is" (a noun) rather than "what it does" (a verb disguised as a noun). When a developer creates a `UserManager`, they are essentially creating a puppet master that treats data as passive objects, which leads to the "Anemic Domain Model" and a total breakdown of encapsulation.

The lecture emphasizes the importance of anthropomorphism—treating objects as living organisms that we respect and interact with, rather than tools or slaves that we command. Bugayenko suggests that instead of using a `FileSaver` to perform an action, we should design a `SavedFile` or a `File` object that knows how to represent itself. By removing the "-er" suffix, developers are forced to rethink the identity and responsibility of their classes, resulting in smaller, more cohesive, and more declarative code. This shift from a "manager-slave" architecture to an ecosystem of autonomous entities is, in Yegor's view, the only way to achieve high-quality, maintainable software. He challenges the industry's obsession with "Service" layers and "Utilities," calling them procedural "garbage bins" that hinder true object decomposition.

## Key Insights
- Objects are not tools or collections of functions; they are living organisms with their own identity and autonomy.
- If you name a class "Manager," you are admitting that you don't know what the object actually is or what its real identity should be.
- The "-er" suffix is a symptom of procedural decomposition, where logic is separated from data, violating the core principle of encapsulation.
- We should decompose systems based on entities (nouns) rather than actions (verbs). Instead of a `UserValidator`, we should have a `ValidatedUser`.

## Relevance: 5/5
This lecture is fundamental for any developer seeking to understand high-level architectural design and the philosophical roots of "clean" object-oriented code.
