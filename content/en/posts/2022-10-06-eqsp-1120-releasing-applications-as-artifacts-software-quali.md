---
title: "EQSP 11/20: Releasing Applications as Artifacts"
date: 2022-10-06T00:00:00Z
tags:
  - "yegor"
  - "software-engineering"
cover:
  image: "https://img.youtube.com/vi/9YeTbqFr85s/maxresdefault.jpg"
  alt: "EQSP 11/20: Releasing Applications as Artifacts"
  relative: false
draft: false
---

> **Watch:** [https://www.youtube.com/watch?v=9YeTbqFr85s](https://www.youtube.com/watch?v=9YeTbqFr85s)

## Summary
In this lecture, Yegor Bugayenko explains the critical distinction between a software library (package) and a full-scale application in the context of release management. While a library is a dependency used by other developers, an application is a final product that requires a more robust deployment strategy. The central thesis is the "Artifact Philosophy": an application should be delivered as a single, immutable, and versioned unit—such as a Docker image or a "fat" JAR file. This approach ensures environment independence and eliminates the risks associated with manual file transfers or configuration errors.

Yegor emphasizes that deployment should never involve a "git pull" on a production server. Instead, it should be a controlled "switch" where a new version of the artifact is launched alongside the old one. To maintain data integrity during this transition, he suggests a "read-only mode," where the old version stops writing to the database just before the traffic is redirected to the new version. Furthermore, the entire process must be fully automated. Using tools like Rultor, developers should trigger releases through simple commands in a ticket or pull request, leaving the heavy lifting of testing, tagging, and deploying to autonomous bots. This eliminates human error and ensures that the production environment remains a "sacred" space untouched by manual tweaks.

## Key Insights
- "An application is not just code; it is a single, immutable artifact that must contain everything it needs to run."
- "If you are doing a 'git pull' on your production server, you are not a professional; you are a hobbyist playing with fire."
- "The deployment process is essentially a traffic switch between two immutable states of the system."
- "Zero-downtime is achieved not by magic, but by placing the system in read-only mode during the critical seconds of the transition."

## Relevance: 5/5
This video is essential for understanding modern CI/CD practices, DevOps culture, and the shift from "code-centric" to "artifact-centric" delivery, which is foundational for scalable software engineering.
