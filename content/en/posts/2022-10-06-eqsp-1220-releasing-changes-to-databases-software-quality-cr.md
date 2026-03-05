---
title: "EQSP 12/20: Releasing Changes to Databases"
date: 2022-10-06T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
  - "infrastructure"
cover:
  image: "https://img.youtube.com/vi/qtTG1kRLzCY/maxresdefault.jpg"
  alt: "EQSP 12/20: Releasing Changes to Databases"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=qtTG1kRLzCY](https://www.youtube.com/watch?v=qtTG1kRLzCY)

## Summary
In this lecture of his software quality crash course, Yegor Bugayenko argues for a strict, automated approach to database management, treating the database schema and data as core application assets rather than external entities. The central thesis is that manual interventions in production databases are a hallmark of low professionalism and a primary source of technical debt and instability. Instead, every change must be encapsulated in versioned migration scripts (e.g., 001.sql, 002.sql) that are stored in the source code repository alongside the application logic.

Yegor emphasizes the use of industry-standard tools like Liquibase or Flyway to manage these transitions. These tools maintain a historical record within the database itself, ensuring that only new, unapplied scripts are executed during deployment. The workflow he proposes is uncompromising: the CI/CD pipeline is the only entity with the authority to modify the production schema. Developers should never have direct access to production; their role is to propose changes via Merge Requests, which are then reviewed by an architect and applied automatically. This "Expand/Contract" mindset ensures that the database evolves incrementally, preventing configuration drift and making the entire environment reproducible. By stripping manual power from individuals and vesting it in automated processes, teams can achieve the consistency required for high-quality, scalable software systems.

## Key Insights
- "The database is not just a storage; it is a living part of your application code and must be versioned as such."
- "If a programmer has manual access to the production database, you don't have a quality process; you have a recipe for disaster."
- "Automation is the only way to take authority away from human error and give it to the system's architecture."
- "Tools like Liquibase are not optional; they are the gatekeepers of your project's structural integrity."

## Relevance: 5/5
This lecture is essential for any modern software engineer or architect looking to implement robust CI/CD pipelines and maintain strict quality standards in stateful applications.
