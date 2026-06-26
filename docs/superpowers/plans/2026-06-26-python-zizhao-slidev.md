# Python 自招 Slidev Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Build a runnable Slidev deck for a two-hour Python autonomous-admission prep session.

**Architecture:** Use a minimal Slidev project rooted in the current workspace. Keep the teaching content in `slides.md`, visual polish in `style.css`, and original reference screenshots in `assets/slides`.

**Tech Stack:** Slidev, Markdown, CSS, local image assets.

---

### Task 1: Project Skeleton

**Files:**
- Create: `package.json`
- Create: `.gitignore`

- [ ] Add a minimal package manifest with `dev`, `build`, and `export` scripts.
- [ ] Add `.gitignore` entries for dependencies and generated Slidev output.

### Task 2: Slide Assets

**Files:**
- Create: `assets/slides/p01.jpg`
- Create: `assets/slides/p02.jpg`
- Create: `assets/slides/p03.jpg`
- Create: `assets/slides/p04.jpg`
- Create: `assets/slides/p05.jpg`
- Create: `assets/slides/p06.jpg`
- Create: `assets/slides/2025-context.png`

- [ ] Copy the source images into the workspace so the deck is portable.

### Task 3: Main Deck

**Files:**
- Create: `slides.md`

- [ ] Write the two-hour route.
- [ ] Map P01-P06 to exam skills.
- [ ] Add template slides for `input`, formulas, branches, loops, and `turtle`.
- [ ] Add three short变式 exercises and answer slides.
- [ ] Add open-question templates for campus mini-program, check-in, voting, and QR-code scenarios.

### Task 4: Visual Styling

**Files:**
- Create: `style.css`

- [ ] Add a restrained classroom-friendly visual system.
- [ ] Improve code readability and callout styling.
- [ ] Keep Chinese text large enough for projection.

### Task 5: Verification

**Commands:**
- Run: `npm install`
- Run: `npm run build`
- Run: `npm run dev -- --host 127.0.0.1`

- [ ] Install dependencies.
- [ ] Build the deck.
- [ ] Start the local preview server and report the URL.

