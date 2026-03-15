# LESSONS.md

This file stores reusable lessons discovered while building, reviewing, testing, deploying, and maintaining projects inside Venture-OS.

This file is append-only unless the founder explicitly requests cleanup or restructuring.

Its purpose is to stop repeated mistakes, improve future decisions, and preserve useful knowledge across projects.

This is a **shared operational memory file** for the founder, Gemini, and Claude.

---

# How To Use This File

Add lessons only when they are:

- reusable
- practical
- specific
- likely to matter again

Good lessons are short and actionable.

Bad lessons are vague, motivational, or too tied to one tiny moment.

---

# Update Rules

When adding a lesson:

- append, do not rewrite the whole file
- keep it concise
- group it under the most relevant section
- include the date when useful
- focus on decisions, mistakes, blockers, and patterns
- prefer concrete lessons over abstract observations

If a lesson is only relevant to one project, consider keeping it in that project’s `progress.md` unless it is likely to matter again.

---

# What Belongs Here

Examples of good lessons:

- architecture lessons
- deployment lessons
- security lessons
- monetisation lessons
- workflow lessons
- repeated mistakes to avoid
- stack decisions that worked or failed
- product simplifications that saved time
- distribution insights that matter across projects

---

# What Does Not Belong Here

Do not add:

- long diary entries
- raw brainstorming
- vague thoughts
- duplicate information from `progress.md`
- project plans
- emotional reflections unless they affect execution quality

---

# Core Principles

- Simple systems are better than clever systems.
- A working MVP is more valuable than a perfect design.
- Revenue matters more than novelty.
- Solo-dev maintainability matters more than technical impressiveness.
- Launch speed matters, but not at the cost of critical security or broken core logic.
- Repeated mistakes must be captured and avoided.

---

# Global Lessons

## Product

- Keep MVP scope tight. If a feature does not help validate demand, improve the core user experience, or support monetisation, it is probably not needed yet.
- A simpler version launched sooner is usually better than a broader version launched later.
- Small products making modest revenue are valuable. Do not reject ideas only because they are not huge.
- If distribution is unclear, the idea is weaker than it looks.
- If monetisation is vague, the idea is weaker than it looks.
- Good product decisions reduce build time and maintenance burden.

## Engineering

- Prefer well-supported tools, libraries, and frameworks over clever custom setups.
- Avoid overengineering early. Complexity should be earned by actual traction.
- Keep architecture simple enough for one developer with AI assistance to maintain.
- Separate planning repos from product repos.
- Server-side validation matters whenever money, permissions, or protected actions are involved.
- Do not trust client-side logic for pricing, access, or security-sensitive decisions.
- Fix the core workflow before improving polish.

## AI Workflow

- The repo is the source of truth, not agent memory.
- Agents should read system context first, then project context, then work in the product repo.
- Gemini should plan before building.
- Claude should review before refactoring.
- Agents should update `progress.md` after each meaningful session.
- If a lesson repeats twice, record it here.
- If a workflow issue repeats twice, record it here.

## Founder Execution

- Too many active projects destroys momentum.
- Finishing near-complete work often beats starting something new.
- Fast progress comes from small, well-defined steps.
- Over-preparing systems can become disguised procrastination.
- The goal is profitable shipped products, not perfect internal systems.

---

# Reusable Lesson Entry Format

Use this format for new lessons when useful:

## [Category]

### YYYY-MM-DD
- Lesson
- Why it matters
- Optional: project/source

Example:

### 2026-03-14
- Keep payment calculations server-side only.
- Prevents checkout mismatches and security problems.
- Source: booking app review

---

# Recent Lessons

### 2026-03-14
- Keep Venture-OS as the planning and coordination layer only.
- Put actual source code in separate product repos.
- This keeps AI context cleaner and repos easier to manage.

### 2026-03-14
- Do not rely on long-term agent memory across weeks.
- Preserve continuity in `overview.md`, `master-build-prompt.md`, `progress.md`, and this file.

### 2026-03-14
- Force a planning step before implementation.
- This reduces drift, overbuilding, and unnecessary rework.

### 2026-03-14
- Claude should act as the final quality and launch gate.
- Gemini should build, Claude should tighten, simplify, secure, and validate.

---

# Categories For Future Lessons

Use these sections as needed.

## Monetisation

## Distribution

## Product Scope

## UX / User Flow

## Architecture

## Security

## Deployment

## AI Workflow

## Founder Workflow

## Launch

## Maintenance
