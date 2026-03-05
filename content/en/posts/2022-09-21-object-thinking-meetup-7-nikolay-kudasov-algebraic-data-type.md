---
title: "Object Thinking Meetup #7: Nikolay Kudasov / Algebraic Data Types"
date: 2022-09-21T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
  - "oop"
  - "ai"
cover:
  image: "https://img.youtube.com/vi/ERIDMfy4rCg/maxresdefault.jpg"
  alt: "Object Thinking Meetup #7: Nikolay Kudasov / Algebraic Data Types"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=ERIDMfy4rCg](https://www.youtube.com/watch?v=ERIDMfy4rCg)

## Summary
In this meetup, Nikolay Kudasov, a specialist in functional programming from Innopolis University, explores the mathematical foundations and practical applications of Algebraic Data Types (ADTs). The core of the discussion revolves around the "algebra" of types, where data structures are built using two primary operations: Product types (AND) and Sum types (OR). Product types, such as classes or structs, are common in almost all languages, representing a combination of fields. However, Kudasov emphasizes that Sum types (tagged unions or variants) are often the "missing piece" in traditional Object-Oriented Programming (OOP) like Java or C++.

Kudasov explains that ADTs allow developers to "make illegal states unrepresentable." By using Sum types, a programmer can define a variable that is strictly either a 'Success' containing data or an 'Error' containing a message, preventing the common OOP pitfall of having both fields present but one being null. The talk also addresses the "Expression Problem," comparing how ADTs and OOP handle extensibility: while OOP makes it easy to add new data types (subclasses) but hard to add new operations (interface methods), ADTs make it easy to add new operations but require a complete overview of all data variants. This mathematical approach to modeling leads to more robust, self-documenting code and leverages the compiler to enforce business logic through exhaustive pattern matching.

## Key Insights
- "The goal of a good type system is to make illegal states unrepresentable in your code."
- "Product types represent 'AND' (this and that), while Sum types represent 'OR' (either this or that). Most bugs happen because we use AND when we meant OR."
- "In traditional OOP, we often simulate Sum types with inheritance, but we lose the ability for the compiler to check if we've handled every possible case."
- "ADTs are a way to bring mathematical rigor to domain modeling, turning runtime errors into compile-time certainties."

## Relevance: 5/5
Extremely high for software architects and developers. ADTs are a fundamental tool for reducing complexity and improving type safety in modern systems.
