# Featured Agents Refresh Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Update the featured agent block in `README.md` to use the banner palette and show six requested agents.

**Architecture:** Keep the existing README layout and replace only the current featured card SVGs. Use a 3x2 HTML table with light, banner-aligned SVG cards so the section stays visually consistent with the repo banner.

**Tech Stack:** Markdown, inline SVG data URIs

---

### Task 1: Replace Featured Cards

**Files:**
- Modify: `README.md`

- [ ] **Step 1: Replace current 4-card block**

Swap the current featured block for six cards:
- `repo-intake`
- `bug-hunter`
- `security-reviewer`
- `test-engineer`
- `performance-profiler`
- `workflow-strategist`

- [ ] **Step 2: Retheme cards**

Use light gradient cards with dark slate text and blue/cyan accent details.

### Task 2: Verify Featured Section

**Files:**
- Modify: `README.md`

- [ ] **Step 1: Verify requested names exist**

Run: `Select-String -Path .\README.md -Pattern 'repo-intake','bug-hunter','security-reviewer','test-engineer','performance-profiler','workflow-strategist'`
Expected: all six matches found

- [ ] **Step 2: Verify removed old featured-only agent**

Run: `Select-String -Path .\README.md -Pattern 'frontend-debugger'`
Expected: match may still exist elsewhere in README, but not inside featured block
