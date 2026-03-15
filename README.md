# Venture-OS

Venture-OS is the **planning, coordination, and operational memory layer** for a portfolio of digital ventures.

It is designed for a **solo founder using AI as a small product team**.

This repository is the shared source of truth for:

- venture strategy
- project definitions
- build instructions
- execution progress
- lessons learned
- agent operating rules

This repository is **not** the main codebase for each product.

Each real product should normally live in its **own separate project repository**.

Venture-OS exists to coordinate those projects, guide AI agents, and preserve context across long build cycles.

---

# Purpose

The purpose of Venture-OS is to help one founder consistently build, launch, improve, and manage multiple digital products without losing context or drowning in unfinished work.

The system is designed to support:

- fast experimentation
- disciplined execution
- simple and maintainable builds
- small but compounding revenue streams
- long-term ownership of digital assets

The core business goal is **financial freedom** through a portfolio of products rather than dependence on a single big success.

---
# Source of Truth

Project files inside Venture-OS are the source of truth for product intent and build direction.
Actual product repositories are the source of truth for implementation.

---

# System Model

Venture-OS follows a simple agent structure:

## Generator
The Generator builds.

Primary tool:
- Gemini

Typical responsibilities:
- scaffolding projects
- implementing MVP features
- turning specifications into working code
- suggesting simpler build paths

---

## Reflector
The Reflector critiques, tightens, and protects.

Primary tool:
- Claude

Typical responsibilities:
- code review
- debugging
- refactoring
- security and vulnerability review
- product sanity checks
- launch readiness checks

---

## Curator
The Curator preserves context and improves the system over time.

Primary location:
- Venture-OS repository

Typical responsibilities:
- storing project definitions
- tracking progress
- recording lessons
- refining workflows
- keeping projects aligned with founder goals

---

# Core Principles

## 1. Revenue First
The purpose of projects is to create income.

Projects do not need to be huge to matter.

Small products generating **£100–£500 per month each** are valuable and can compound meaningfully.

---

## 2. Speed to Market
A working MVP in front of real users is more valuable than extended planning or perfect architecture.

Launch fast, learn quickly, improve deliberately.

---

## 3. Simplicity Wins
All systems should remain understandable and maintainable by **one developer with AI assistance**.

Avoid unnecessary complexity, infrastructure, and premature scaling.

---

## 4. Controlled Scope
Project scope must be driven by the project files.

AI agents should not silently expand features, add technologies, or change product direction without explicit approval.

---

## 5. Separate Planning From Code
Venture-OS stores the planning and coordination layer.

Actual product code should usually live in separate repositories.

This prevents confusion, bloated repos, and mixed responsibilities.

---

# Repository Structure

```text
venture-os/
  README.md
  GOALS.md
  GEMINI.md
  CLAUDE.md
  LESSONS.md
  AGENT_IMPROVEMENTS.md

  projects/
    <project-name>/
      overview.md
      tech-stack.md
      master-build-prompt.md
      progress.md

  execution/
    active-projects.md
    weekly-review.md
