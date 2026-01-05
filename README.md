# The AI Solopreneur: Resource Kit

Welcome to the official resource kit for the talk: **"The AI Solopreneur: How to Bootstrap a Startup Using Generative AI"**.

This repository contains the **Slides** and the **System Prompts** (The Organic-Growth Workflow) demonstrated in the presentation.

## 📂 Contents

### 1. The Slides
*   **[Interactive Slides (SPA)](https://ai-solopreneur.pages.dev/)**
*   **[Download PDF](./slides.pdf)**

## 🛠️ The "Context" Secret
In the talk, I mentioned using **Repomix** to give the AI context.
**Phase 1-3** can often be done with a fresh chat context.
**Phase 4 (Building)** requires the AI to understand your existing code.

**Recommended Workflow:**
1. Run `npx repomix` in your terminal to pack your codebase.
2. Copy the contents of `repomix-output.xml`.
3. Paste it into the chat *before* using the **Builder Prompts**.

### 2. The Prompts (The Organic-Growth Workflow)
These are the exact system instructions used to build [BadmintonHub.app](https://badmintonhub.app). They are designed to be used in sequence.

| Phase | Role | Goal | File |
| :--- | :--- | :--- | :--- |
| **1** | **Product Manager** | Idea → PRD Spec | [01_phase1_the_sketch.md](./prompts/01_phase1_the_sketch.md) |
| **2** | **Architect** | PRD → Blueprint (DB, API) | [02_phase2_the_blueprint.md](./prompts/02_phase2_the_blueprint.md) |
| **3** | **Project Manager** | Blueprint → Task List | [03_phase3_the_game_plan.md](./prompts/03_phase3_the_game_plan.md) |
| **4** | **Builder** | Task List → Code | [04_phase4_the_build_cycle.md](./prompts/04_phase4_the_build_cycle.md) |
| **5** | **Release Manager**| Code → Live App | [05_phase5_the_launchpad.md](./prompts/05_phase5_the_launchpad.md) |

## 🚀 Case Study
These prompts were used to build **BadmintonHub**, a real-world multi-tenant SaaS application, without a large team.
👉 **[Visit BadmintonHub.app](https://badmintonhub.app)**
