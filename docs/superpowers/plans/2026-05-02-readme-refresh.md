# README Refresh Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Rewrite `README.md` into a more visual, product-style document while preserving the current information.

**Architecture:** Keep the existing banner asset and rebuild the markdown structure around it. Use compact sections near the top for navigation, quickstart, and featured roles, then retain the detailed installation, invocation, and workflow guidance lower in the document.

**Tech Stack:** Markdown, SVG

---

### Task 1: Rebuild Top-Level README Structure

**Files:**
- Modify: `README.md`

- [ ] **Step 1: Add product-style hero and quick navigation**

Add banner, H1, concise summary, and a jump-link strip near top of `README.md`.

- [ ] **Step 2: Add quickstart tiles section**

Add a fast-scanning section near the top with the main entry workflows: help, inspect, review, fix.

- [ ] **Step 3: Add featured agent cards**

Add a markdown/HTML-light featured section that highlights a small subset of agents with stronger visual treatment.

### Task 2: Preserve Detailed Guidance

**Files:**
- Modify: `README.md`

- [ ] **Step 1: Keep installation commands intact**

Retain Windows and macOS/Linux install commands and reload note.

- [ ] **Step 2: Keep invocation examples**

Retain the existing core invocation examples and place them under a clearer section.

- [ ] **Step 3: Keep all 16 agents documented**

Retain the full agent list with one-line descriptions.

- [ ] **Step 4: Keep recommended workflows**

Retain the existing workflow prompts and organize them under a clearer heading.

### Task 3: Verify README Requirements

**Files:**
- Modify: `README.md`

- [ ] **Step 1: Verify banner reference remains**

Run: `Select-String -Path .\README.md -Pattern 'assets/banner.svg'`
Expected: one match

- [ ] **Step 2: Verify install commands remain**

Run: `Select-String -Path .\README.md -Pattern 'Copy-Item','.codex/skills','cp -R ./skills/multi-agent-dev'`
Expected: matches found

- [ ] **Step 3: Verify all 16 agents remain**

Run: `Select-String -Path .\README.md -Pattern 'repo-intake','codebase-cartographer','bug-hunter','frontend-debugger','test-engineer','implementation-minimalist','security-reviewer','performance-profiler','architect-reviewer','docs-maintainer','accessibility-reviewer','workflow-strategist','diff-reviewer','final-merge-reviewer','dependency-reviewer','database-reviewer'`
Expected: matches found for all patterns
