---
title: "The Pain of OOP, Lecture #3: Getters and naked data"
date: 2023-06-27T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
  - "oop"
  - "ai"
cover:
  image: "https://img.youtube.com/vi/2YyVmIQQ23w/maxresdefault.jpg"
  alt: "The Pain of OOP, Lecture #3: Getters and naked data"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=2YyVmIQQ23w](https://www.youtube.com/watch?v=2YyVmIQQ23w)

## Summary
In this lecture, Yegor Bugayenko addresses one of the most pervasive issues in modern software development: the use of getters. He argues that the presence of `get...` methods transforms an object from an active participant into a passive container of information, or "naked data." The core thesis is that true encapsulation is not merely about making fields private, but about hiding the structure of the data itself. If an object allows its internals to be extracted, it ceases to be an object and effectively becomes a data structure.

Yegor critiques modern IDEs and libraries like Lombok for making getter generation too easy, which encourages the creation of "anemic models." In these models, objects are devoid of logic, forcing business logic into external services—a shift that reverts Object-Oriented Programming back to a procedural style. He specifically targets Data Transfer Objects (DTOs), labeling them as "the ultimate evil" because they masquerade as objects while possessing none of their inherent qualities.

The proposed alternative to getters is the "Tell, Don't Ask" principle. Instead of retrieving data from an object to make a decision, developers should command the object to perform the task based on its internal state. Additionally, Yegor argues against the `get` prefix, which reinforces procedural thinking. He suggests using noun-based method names (e.g., `weight()` instead of `getWeight()`) to signal interaction with a living entity rather than a memory dump. The lecture concludes with a critique of the Spring Framework, illustrating how its reliance on "beans" and getters/setters turns Java into a procedural-like environment reminiscent of older languages like COBOL.

## Key Insights
*   "A getter is a way to undress an object and show its naked data to the world."
*   "An object is not a bucket of data; it is a living organism with its own behavior and responsibilities."
*   "DTOs are the ultimate evil in OOP because they force the rest of the system to be procedural."
*   "Encapsulation is not about hiding fields; it's about hiding the fact that data even exists inside the object."

## Relevance: 5/5
Extremely high relevance for software architects and developers seeking to understand strict Object-Oriented principles and avoid common anti-patterns like anemic domain models.
