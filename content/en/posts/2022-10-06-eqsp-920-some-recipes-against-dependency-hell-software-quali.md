---
title: "EQSP 9/20: Some Recipes Against Dependency Hell"
date: 2022-10-06T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
  - "ai"
cover:
  image: "https://img.youtube.com/vi/_NU0IYv8ZJo/maxresdefault.jpg"
  alt: "EQSP 9/20: Some Recipes Against Dependency Hell"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=_NU0IYv8ZJo](https://www.youtube.com/watch?v=_NU0IYv8ZJo)

## Summary
In this lecture, Yegor Bugayenko addresses the notorious "Dependency Hell," a state where conflicting requirements for shared libraries make a system unstable or impossible to build. He argues that the root cause is often a misplaced trust in third-party developers' adherence to Semantic Versioning (SemVer). Bugayenko categorizes dependencies into two groups: those we trust to maintain backward compatibility (where dynamic ranges like `^` or `~` are acceptable) and those we don't (where versions must be strictly pinned).

A central theme is the "Fail Fast" principle. He recommends using build-time tools, such as the Maven Enforcer Plugin, to detect version conflicts early. Instead of letting the package manager silently resolve a conflict with a random version, the build should crash, forcing the developer to explicitly choose the correct version through transitive resolution. Furthermore, he emphasizes that every new dependency is a liability that increases the attack surface and complexity. Developers should audit dependency trees (`npm list` or `mvn dependency:tree`) before integration. Finally, Bugayenko advocates for automated release pipelines where every artifact is traceable to a specific Git tag, ensuring reproducibility and consistency across environments. This disciplined approach shifts dependency management from a source of chaos into a controlled architectural decision.

## Key Insights
- "Treat every new dependency as a potential liability."
- "The build should fail immediately rather than allowing non-deterministic behavior."
- "Your versioning strategy should be dictated by your trust in the dependency's maintainers."
- Explicitly resolve transitive conflicts rather than letting the build tool "guess" which version to use.

## Relevance: 5/5
Essential for understanding modern build systems, architectural stability, and supply chain security in software engineering.
