# Phase 2: The Blueprint — System Architecture & Design

**Goal:** Create the complete technical and visual blueprint for the application before writing implementation code.

## The Context
You are the **Architect**. The AI is the **Designer & Scaffolder**.
You feed it the PRD, and it generates the structured documents.

---

## Step 1: Create User Flow Diagrams

```markdown
Based on the attached `PRD.md`, create a **User Flow Diagram** using Mermaid syntax. The diagram should show the journey from a user receiving an invite link, to registering, logging in, viewing the dashboard, and RSVPing to a session.
```

**Outcome:** A `docs/navigation/app-navigation-flow.md` file.

---

## Step 2: Generate ASCII Wireframes

```markdown
Using the user flow and PRD, create ASCII art wireframes for the following key screens:
1.  **Dashboard / Fixtures List:** Show a list of upcoming sessions, with status badges (e.g., 'Open', 'Full').
2.  **Fixture Detail Page:** Show details for one session, attendees list, and an area for a member to set their status (Attending/Not Attending).
3.  **Registration/Onboarding:** Include fields for name, email, and club selection.
```

**Outcome:** A `docs/wireframes/` directory with markdown files.

---

## Step 3: Design the Database Schema

```markdown
You are a Database Architect. Based on the attached PRD and wireframes, design a complete database schema for the [Project Name].

**Your Task:**
1.  Define the schema for the following tables: [List tables, e.g., users, clubs, members, fixtures].
2.  Include all necessary columns, data types, and relationships (foreign keys).
3.  Write the schema using **Drizzle ORM syntax** (or Prisma/SQL) in separate files.
4.  Create an `index.ts` file that exports all schema tables.
```

**Outcome:** A complete Drizzle/Prisma schema.

---

## Step 4: Define the API Contract

```markdown
You are a Backend Tech Lead. Based on the PRD, wireframes, and database schema, define the **tRPC API contract** (or REST/GraphQL).

**Your Task:**
For each of the following features, create a tRPC router file in `packages/api/src/routers/` with placeholder procedures and Zod input schemas:
1.  `clubs.ts`: `create`, `getSettings`, `update`.
2.  `fixtures.ts`: `create`, `list`, `detail`, `join`.
3.  `availability.ts`: `setAttendance`, `getAttendees`.

Include comments specifying the required user role for each procedure (e.g., `// Admin only`).
```

**Outcome:** A clear API contract.

---

## Step 5: Scaffold the Project

```markdown
You are a Senior Full-Stack Developer. Based on our tech stack (The Better T Stack: Turborepo, Bun, React, TanStack Router, Hono, Cloudflare Workers, Drizzle, Better Auth, tRPC), generate the complete monorepo file structure.

**Your Task:**
1.  Create the directory structure for `apps/web`, `apps/server`, and `packages/`.
2.  Generate `package.json` files for the root and each workspace, including all necessary dependencies.
3.  Generate `tsconfig.json` files with the correct path aliases.
4.  Create boilerplate configuration files: `turbo.json`, `vite.config.ts`, `wrangler.jsonc`.
```

**Outcome:** A complete, runnable project skeleton.

---

## Step 6: Define the Design System

*Note: This corresponds to the "High Density UI" Deep Dive in the talk.*

```markdown
You are a Lead UI/UX Designer. Create a `design_system.md` file defining the visual rules for the application.

**Requirements:**
1.  **Typography:** Define Heading font (e.g., Oswald) and Body font (e.g., Inter).
2.  **Spacing:** Define a "Mobile First" spacing scale (e.g., Base `p-3`, Md `p-6`).
3.  **Colors:** Define Primary, Secondary, and Destructive semantic tokens.
4.  **Components:** Define the shape of Cards (e.g., `rounded-xl`) and Buttons.
```

**Outcome:** A design rulebook that ensures the AI generates consistent UI code.
