---
title: "И37: А. М. Бородин | PostgreSQL | Yandex Cloud | Open source in Russia"
date: 2026-03-04T17:16:00Z
tags:
  - "yegor"
  - "software-engineering"
  - "infrastructure"
draft: false
---

> **Source:** [https://www.youtube.com/watch?v=YuwLCBRCvUA](https://www.youtube.com/watch?v=YuwLCBRCvUA)

This transcript features an interview between Yegor Bugayenko and Andrey Borodin, a significant contributor to PostgreSQL and a developer at Yandex Cloud. The discussion covers the culture of open-source development, the technical differences between major databases, and the "ancient" workflows of the PostgreSQL community.

## Summary

The conversation begins with a lighthearted debate over the "correct" pronunciation of PostgreSQL. Borodin argues from an engineering perspective: terminology exists to ensure clear communication between team members, and as long as there is no misinterpretation, the specific phonetics matter less than the clarity of the system being built. 

A central theme of the interview is the comparison between **PostgreSQL and MySQL**. Borodin admits that while he finds MySQL's architecture slightly more interesting in some respects, he views PostgreSQL as the superior choice for a developer who wants to impact the core of the technology. He notes that MySQL’s development is now heavily controlled by Oracle, making it difficult for outside contributors to land patches. In contrast, PostgreSQL remains a "truly free" database where an independent engineer can "inflict benefit" (a humorous Russian idiom for doing good) on the project without being an employee of a specific corporation.

The most contentious point of the interview is the **PostgreSQL development process**. Yegor expresses shock that a world-class project still relies on mailing lists (`PGSQL Hackers`) rather than modern platforms like GitHub or GitLab. He describes the experience as "prehistoric," feeling like he's back in the era of FidoNet, dealing with unformatted plain text and no syntax highlighting. 

Borodin defends this "boiled frog" existence (referring to how he has grown accustomed to the environment). He argues that while the tools are old, they are rarely the bottleneck. To the PostgreSQL community, the **rationale and the thought process** behind a patch are more important than the code itself. He emphasizes that "code is a shallow thing" that anyone can write; the real value lies in the architectural meaning and the discussion surrounding it. He describes a workflow where patches are received via email and applied manually using console tools like `git am`. Despite the lack of modern UI, the project maintains high standards through various CI systems and the rigorous oversight of a small group of "committers" who ensure the integrity of the main repository.

## Key Insights

*   **On Technical Communication:** "Engineers speak so that they understand each other... if you were understood unambiguously without misinterpretation, call it whatever you want."
*   **On Open Source Freedom:** "PostgreSQL is a truly free database where you can actually 'inflict benefit' [make a real impact]. Bringing a patch to MySQL today is very difficult [without working for Oracle]."
*   **On Tools vs. Philosophy:** "Almost never are the tools the problem. I’ve just become the 'boiled frog' in this mailing list... Code is a shallow thing that anyone can do; it’s the human thoughts and the meaning that matter."
*   **On the Value of Community:** Borodin highlights that contributing to Postgres isn't just about code—it’s an education in logic and even language, noting how reading senior developers' (like Tom Lane) commit messages helped him learn nuanced English.

## Relevance: 4/5

This interview is highly relevant to **Software Engineering** and **Open Source Management**. It provides a rare look into how one of the world's most successful software projects maintains a high bar for quality using "outdated" methods. While it doesn't touch on **OOP** (Postgres is written in C), it offers profound insights into **distributed team management**, the importance of architectural documentation over "shiny" tools, and the professional growth path of a high-level systems engineer.
