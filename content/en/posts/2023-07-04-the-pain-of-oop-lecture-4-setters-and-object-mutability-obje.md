---
title: "The Pain of OOP Lecture #4: Setters and Object Mutability"
date: 2023-07-04T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
  - "oop"
  - "ai"
cover:
  image: "https://img.youtube.com/vi/h0jf9E1tjf4/maxresdefault.jpg"
  alt: "The Pain of OOP Lecture #4: Setters and Object Mutability"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=h0jf9E1tjf4](https://www.youtube.com/watch?v=h0jf9E1tjf4)

## Summary
In the fourth lecture of the "The Pain of OOP" series, Yegor Bugayenko delivers a sharp critique of setters and the concept of object mutability. His central argument is that setters transform objects into passive "data bags," stripping them of their autonomy and violating the fundamental principle of encapsulation. In pure object-oriented programming, an object should be a self-sufficient entity that manages its own state and logic. When we use setters, we allow external procedures to manipulate the object's internals, which effectively turns object-oriented code into procedural code where logic is scattered across the entire application.

Yegor highlights three critical issues caused by mutability. First is the loss of identity: if an object's fields are constantly changing, it becomes difficult to ensure it represents the same business entity. Second is the immense difficulty in debugging, as an object's state can be altered at any time from any part of the program, making it hard to track down the source of bugs. Third is the lack of inherent thread safety; mutable objects require complex locking mechanisms in multi-threaded environments. The only architecturally sound solution proposed is full immutability. Objects should receive all necessary data through the constructor, and any "change" should result in the creation of a new instance. This approach makes software predictable, simplifies testing, and forces developers to think in terms of real-world behaviors rather than technical field manipulations.

## Key Insights
1. "Setters turn objects into simple bags of data."
2. "An object must be a living entity, not a passive container."
3. "Mutability is the primary source of problems and bugs in software architecture."
4. "In a truly object-oriented world, all objects should be immutable by default."

## Relevance: 5/5
This lecture is foundational for understanding the "Elegant Objects" philosophy. It challenges mainstream industry standards (like Java Beans) and offers a radical but internally consistent approach to building maintainable and thread-safe systems.
