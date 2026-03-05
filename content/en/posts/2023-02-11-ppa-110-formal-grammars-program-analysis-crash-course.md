---
title: "PPA 1/10: Formal Grammars [program analysis crash course]"
date: 2023-02-11T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/rsoPqA1CYmE/maxresdefault.jpg"
  alt: "PPA 1/10: Formal Grammars [program analysis crash course]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=rsoPqA1CYmE](https://www.youtube.com/watch?v=rsoPqA1CYmE)

## Summary
In this inaugural lecture of the Program Analysis Crash Course, Yegor Bugayenko introduces formal grammars as the essential foundation for software analysis. The session focuses on the "front-end" of the analysis pipeline: the process of transforming raw source code from a simple stream of characters into a structured mathematical model. Bugayenko emphasizes that before any meaningful analysis of a program's behavior (semantics) can occur, a rigorous definition of its structure (syntax) is required.

The lecture explores the history and significance of Backus-Naur Form (BNF), tracing its origins to the late 1950s and the development of ALGOL 60. This historical shift from informal textual descriptions to formal notations allowed for the creation of unambiguous language specifications. The transformation process is detailed in two main phases: Lexical Analysis, which groups characters into "Terminals" (tokens like keywords and identifiers), and Syntax Analysis, which organizes these tokens into a "Parse Tree" or "Abstract Syntax Tree" (AST) using "Non-terminals" (syntactic placeholders). Formalization is presented as a prerequisite for removing ambiguity, enabling computers to perform complex tasks such as static bug checking, code optimization, and formal verification. Ultimately, formal grammars serve as the gateway that turns raw text into a data structure suitable for automated reasoning and further analysis steps in the course.

## Key Insights
* "Formal grammars are the mathematical tool used to remove ambiguity from language definitions."
* "You cannot analyze what a program does (semantics) until you have strictly defined what it looks like (syntax)."
* "Lexical analysis turns characters into terminals; syntax analysis turns terminals into a tree structure."
* "The introduction of BNF transformed programming languages from informal sets of instructions into mathematically provable entities."

## Relevance: 5/5
This is foundational knowledge for anyone building compilers, static analysis tools, or working with domain-specific languages (DSLs).
