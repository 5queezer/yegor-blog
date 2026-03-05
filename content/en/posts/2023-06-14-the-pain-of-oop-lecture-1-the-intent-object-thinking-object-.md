---
title: "The Pain of OOP Lecture #1: The Intent object thinking"
date: 2023-06-14T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
  - "oop"
  - "ai"
cover:
  image: "https://img.youtube.com/vi/8FPU_N3LxqA/maxresdefault.jpg"
  alt: "The Pain of OOP Lecture #1: The Intent object thinking"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=8FPU_N3LxqA](https://www.youtube.com/watch?v=8FPU_N3LxqA)

## Summary
In this introductory lecture of his OOP crash course, Yegor Bugayenko argues that modern implementation of Object-Oriented Programming (specifically in languages like Java and C++) has become a "monstrous" deviation from its original intent. He posits that while OOP was designed to manage complexity, it often creates more "spaghetti code" than traditional procedural programming. 

The core of the lecture is a redefinition of what an object should be: a self-sufficient "living organism" that acts as an abstraction of a real-world entity. Yegor emphasizes two critical pillars: data hiding and behavior exposure. He argues that data should never escape an object; the moment you use a "getter" to extract data, you have turned a living object into a passive data structure. The shift required is from "Algorithmic Thinking" (focusing on the step-by-step 'how') to "Object Thinking" (focusing on the declarative 'what'). Instead of writing long procedural scripts, developers should compose systems from small, independent objects that communicate via messages.

## Key Insights
1. "An object is a composition of objects that are abstractions which hide data and expose behavior."
2. "Data should never escape the object; getters and setters are the enemies of true encapsulation."
3. "Object-oriented programming is about building a world of living organisms, not a set of instructions for a CPU to manipulate passive data."
4. "The original intent of OOP was to simplify, but modern 'procedural' habits within classes have made it more complex than C."

## Relevance: 5/5
This lecture provides a fundamental challenge to mainstream software engineering practices, forcing developers to reconsider basic patterns like ORMs, utility classes, and standard data-access methods.
