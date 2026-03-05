---
title: "EQSP 4/20: Making Custom GitHub Actions, by Example [software quality crash course]"
date: 2022-09-07T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/7oKqqgpKjIM/maxresdefault.jpg"
  alt: "EQSP 4/20: Making Custom GitHub Actions, by Example [software quality crash course]"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=7oKqqgpKjIM](https://www.youtube.com/watch?v=7oKqqgpKjIM)

## Summary
In this lecture, Yegor Bugayenko provides a hands-on guide to building custom GitHub Actions, a crucial skill for any team aiming to automate software quality checks beyond standard off-the-shelf solutions. Yegor argues that professional development requires "owning" your automation stack to enforce specific project laws. He distinguishes between JavaScript-based actions and Docker-based actions, strongly advocating for the latter. Docker-based actions package the entire execution environment—OS, dependencies, and tools—ensuring that the action runs identically regardless of the GitHub runner's configuration.

The technical walkthrough focuses on three core files: `action.yml` (the manifest defining inputs and execution logic), a `Dockerfile` (the environment definition), and an entry script (typically `entry.sh`). Yegor demonstrates how to wrap a command-line tool into a container and configure it to analyze code within the `/github/workspace` directory. The ultimate goal is to create a "fail-fast" mechanism where any violation of quality standards immediately results in a failed build status on a Pull Request. By moving away from subjective human reviews and toward objective, automated scripts, teams can maintain a much higher and more consistent level of software quality.

## Key Insights
- **Automate the "Law":** Quality standards should never be mere suggestions; they must be implemented as scripts that fail the build if violated.
- **Environmental Consistency:** Docker-based actions are superior to JavaScript actions because they eliminate "it works on my machine" issues by standardizing the runner's environment.
- **Objective Feedback:** The primary purpose of custom actions is to provide immediate, objective, and non-negotiable feedback to developers through the CI/CD pipeline.
- **Independence:** Relying solely on third-party actions is a risk; professional teams should build and maintain their own automation components for critical quality gates.

## Relevance: 5/5
This is highly relevant for software engineers and DevOps professionals. It bridges the gap between basic CI/CD usage and advanced automation, focusing on the "fail-fast" philosophy essential for maintaining high-quality codebases in a team environment.
