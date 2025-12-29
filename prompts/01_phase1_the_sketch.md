# Phase 1: The Sketch — Product Definition

**Goal:** Transform your concept into a structured Product Requirements Document (PRD) that will serve as the master context for the AI.

## The Context
You are the **Visionary**. The AI is the **Senior Product Manager**.
Your job is to provide the "Raw Notes" (The Pain, The Users, The Tech Stack).
The AI's job is to structure this into a formal document.

## The Prompt

```markdown
You are a Senior Product Manager. Take the following raw notes about a new project and structure them into a formal **Product Requirements Document (PRD)**.

**My Notes:**
*   **Project Name:** [Insert Project Name]
*   **Problem:** [Paste your problem statement]
*   **Users:** [List your user personas]
*   **Features:** [List your key user stories]
*   **Success Metrics:** [List your success metrics]
*   **Tech Stack:** [Specify your tech stack, e.g., Better T Stack (TanStack Router, Hono, Drizzle, Better Auth)]

**Your Task:**
Create a `PRD.md` file. It must include sections for:
1.  Introduction (Problem Statement & Solution)
2.  User Roles & Personas
3.  Functional Requirements (turn each user story into a formal requirement with an ID, e.g., `FR-1.1`).
4.  Non-Functional Requirements (suggest sections for Performance, Security, and Accessibility based on the tech stack).
5.  Success Metrics.
6.  Out of Scope (suggest some features that could be deferred).
```

## The Outcome
You will get a `PRD.md` file. **Save this file.** It is the "Source of Truth" for all future steps.
