---
title: "The Pain of OOP, Lecture #6: NULL references"
date: 2023-08-09T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
  - "oop"
  - "ai"
cover:
  image: "https://img.youtube.com/vi/cTyIF20Kmz4/maxresdefault.jpg"
  alt: "The Pain of OOP, Lecture #6: NULL references"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=cTyIF20Kmz4](https://www.youtube.com/watch?v=cTyIF20Kmz4)

## Summary
In this lecture, Yegor Bugayenko explores the destructive nature of NULL references in object-oriented programming, famously referred to as the "billion-dollar mistake." He argues that NULL is a procedural relic from the C era that treats objects as memory pointers rather than autonomous, behavior-driven entities. According to Yegor, when a method returns NULL, it breaks the object's contract and forces the caller to engage in "defensive programming"—the constant use of `if (x != null)` checks.

The core problem with NULL is that it is not an object; it has no behavior and cannot respond to messages. This lack of polymorphism causes encapsulation to leak, as the logic of handling "nothingness" is offloaded to the user of the object. Yegor advocates for the "Fail Fast" principle: if an object cannot fulfill its role, it should throw an exception immediately or return a "Null Object" (an implementation of the interface that does nothing). He maintains that a clean OOP design should never allow NULL as an argument or return value, ensuring that every reference always points to a valid, predictable object.

## Key Insights
- NULL is not an object; it is a technical pointer that has no place in the conceptual world of OOP.
- Every NULL check is a sign of architectural failure and a violation of the "Tell, Don't Ask" principle.
- Returning NULL is a betrayal of the method's contract, shifting the responsibility for error handling to the caller.
- Using the Null Object pattern or throwing specific exceptions keeps the code declarative and robust.

## Relevance: 5/5
This lecture is essential for understanding strict OOP principles and improving code maintainability by eliminating one of the most common sources of runtime errors.
