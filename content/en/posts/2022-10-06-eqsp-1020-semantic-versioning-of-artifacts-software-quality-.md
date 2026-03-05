---
title: "EQSP 10/20: Semantic Versioning of Artifacts [software quality crash course]"
date: 2022-10-06T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/xGjjRVmeCWA/maxresdefault.jpg"
  alt: "EQSP 10/20: Semantic Versioning of Artifacts [software quality crash course]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=xGjjRVmeCWA](https://www.youtube.com/watch?v=xGjjRVmeCWA)

## Summary
Yegor Bugayenko argues that software versioning is not just a numbering scheme but a strict contract between developers and users. While the industry standard is Semantic Versioning (MAJOR.MINOR.PATCH), the lecture highlights that developers rarely read release notes; instead, they "upgrade and see if it breaks." To manage this reality, Yegor emphasizes the **immutability of artifacts**. Once a package (JAR, Gem, etc.) is published to a central repository like Maven Central, it must never be changed or deleted. 

A major point of the lecture is the distinction between volatile source control (GitHub) and stable artifact repositories. GitHub is "fluent" and unreliable for production dependencies, whereas package managers provide the stability required for professional builds. Yegor also critiques "outdated" 1980s practices like manual changelogs and the duplication of version information in multiple files, which he views as a primary source of synchronization bugs. Instead, he advocates for automated processes, executable documentation (like Rust’s doctests), and the use of live version badges as a single source of truth.

## Key Insights
* "Duplication of information is the source of the majority of troubles in programming."
* "GitHub is a very volatile source of information; we should not rely on it. We can completely rely on Maven Central 100%."
* "Releases must be immutable... no matter what the author thinks or believes later, the version that was published must stay there forever."
* Manual release notes are obsolete; the source of truth should be automated and integrated into the build process.

## Relevance: 5/5
Essential for understanding CI/CD, library maintenance, and the "Elegant Objects" philosophy of strict, automated quality control.
