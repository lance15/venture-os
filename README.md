# Venture-OS

Venture-OS is the **coordination and planning layer** for building multiple digital ventures toward financial freedom.

It acts as a **shared brain** for human and AI collaborators by storing:

* project definitions
* build instructions
* execution progress
* lessons learned
* AI workflow rules

Actual applications and products live in **separate repositories**.
This repository contains the **strategy, structure, and execution system** that guides them.

---

# Purpose

The purpose of Venture-OS is to make it possible for a **solo developer working with AI tools** to consistently launch, iterate, and manage multiple revenue-generating projects.

The system focuses on:

* rapid experimentation
* disciplined execution
* small but consistent revenue generation
* preventing unfinished projects
* leveraging AI as a development team

The long-term objective is to build a **portfolio of digital assets** that collectively generate meaningful income.

---

# How This System Works

Venture-OS follows a simple agent architecture:

Generator → Reflector → Curator

### Generator

Builds the product.

Primary tool:

* Gemini (via Antigravity IDE)

Responsibilities:

* scaffolding projects
* building MVP features
* generating initial implementations

---

### Reflector

Reviews and improves the work.

Primary tool:

* Claude Code

Responsibilities:

* code review
* debugging
* refactoring
* architectural improvements
* reducing technical risk

---

### Curator

Maintains long-term knowledge.

Primary location:

* Venture-OS repository

Responsibilities:

* storing project definitions
* tracking progress
* recording lessons
* improving workflows

---

# Repository Structure

```text
venture-os
│
├── README.md
├── GOALS.md
├── CLAUDE.md
├── GEMINI.md
├── LESSONS.md
├── AGENT_IMPROVEMENTS.md
│
├── projects/
│   └── project-name/
│       ├── overview.md
│       ├── tech-stack.md
│       ├── master-build-prompt.md
│       └── progress.md
│
└── execution/
    ├── active-projects.md
    └── weekly-review.md
```

---

# Project Folder Structure

Each project folder contains the core information needed for AI agents to understand and build the product.

### overview.md

Defines the project concept:

* goal
* target users
* problem solved
* revenue model
* MVP scope

---

### tech-stack.md

Defines technical choices:

* frameworks
* backend services
* hosting
* dependencies

This prevents AI agents from introducing unnecessary technologies.

---

### master-build-prompt.md

The authoritative build specification.

It contains:

* product behaviour
* feature descriptions
* constraints
* build instructions

AI builders must follow this document closely.

---

### progress.md

Tracks execution history.

After each meaningful development session, AI agents must append:

* date
* objective
* work completed
* files modified
* blockers
* next step

This allows future sessions to quickly resume context.

---

# Key System Principles

### Revenue First

Projects are evaluated primarily on their ability to generate income.

Even small projects generating **£100–£500 per month** are valuable.

---

### Speed to Market

Launching quickly is more important than perfect architecture.

Working MVPs beat theoretical designs.

---

### Portfolio Strategy

Financial freedom is achieved through **multiple successful products**, not one large bet.

This system encourages many experiments while maintaining disciplined execution.

---

### Controlled Scope

AI agents should not expand project scope beyond what is defined in the project files unless explicitly instructed.

---

### Solo Developer Friendly

All projects should remain maintainable by **one developer using AI tools**.

Avoid unnecessary complexity, infrastructure, or enterprise patterns.

---

# AI Agent Workflow

Before working on a project, AI agents must read:

1. `projects/<project>/overview.md`
2. `projects/<project>/tech-stack.md`
3. `projects/<project>/master-build-prompt.md`
4. `projects/<project>/progress.md`
5. `LESSONS.md`
6. their instruction file (`CLAUDE.md` or `GEMINI.md`)

Only then should they work inside the project’s code repository.

---

# Lessons and Continuous Improvement

Two files capture accumulated knowledge.

### LESSONS.md

Stores product, engineering, and business insights discovered during development.

---

### AGENT_IMPROVEMENTS.md

Stores improvements to how AI agents should operate.

Examples:

* preferred coding style
* workflow improvements
* recurring mistakes to avoid

---

# Execution Tracking

The `execution/` directory tracks high-level venture progress.

This includes:

* currently active projects
* portfolio status
* weekly reviews

---

# Long-Term Vision

Venture-OS exists to make it possible for a single founder working with AI tools to operate like a **small product studio**.

By combining structured planning, AI development, and disciplined execution, the system aims to produce a portfolio of profitable digital products.

The end goal is **financial freedom through ownership of scalable digital assets**.
