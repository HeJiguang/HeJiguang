# GitHub Profile README Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Build a first-version GitHub profile `README.md` that presents a Chinese-first bilingual technical identity centered on Java/backend engineering and AI/agent exploration, then publish it through the special GitHub profile repository.

**Architecture:** This implementation is intentionally lightweight and text-first. The deliverable is a single `README.md` guided by the approved spec, with section order and writing style doing most of the visual work. Publishing is handled as a final operational step after the Markdown content is stable.

**Tech Stack:** Markdown, UTF-8 text editing, Git, GitHub

---

## Execution Prerequisites

Replace these placeholders before executing the steps:

- `<github-username>`: exact GitHub username
- `<public-email>`: email address to show publicly, if any
- `<blog-url>`: optional personal site or blog URL

Do not create the GitHub profile repository until the exact username is confirmed. The special repository name must match `<github-username>` exactly.

## File Structure

### Files to Create

- `README.md`

### Files to Reference

- `docs/superpowers/specs/2026-03-22-github-profile-readme-design.md`
- `docs/superpowers/plans/2026-03-22-github-profile-readme-implementation.md`

### Files to Modify During Execution

- `README.md`

## Task 1: Scaffold the Profile README

**Files:**
- Create: `README.md`
- Reference: `docs/superpowers/specs/2026-03-22-github-profile-readme-design.md`

- [ ] **Step 1: Re-read the approved spec before writing**

Run: `Get-Content -Path docs/superpowers/specs/2026-03-22-github-profile-readme-design.md`

Expected: the spec confirms the required structure `hero / about / current focus / tech stack / building next / contact`

- [ ] **Step 2: Create the README skeleton with the agreed section order**

Write `README.md` with these headings only:

```md
# Hi, I'm <github-username>

[Hero positioning block]

## About Me

[About copy]

## Current Focus

[Focus list]

## Tech Stack

[Tech stack list]

## Building Next

[Forward-looking list]

## Contact

[Links or contact items]
```

- [ ] **Step 3: Save the file as UTF-8**

Run: `Get-Content -Path README.md -Encoding UTF8`

Expected: the file opens without encoding errors and shows the section skeleton

- [ ] **Step 4: Verify the section order matches the spec**

Run: `Select-String -Path README.md -Pattern '^# |^## '`

Expected: one `#` heading and five `##` headings in the same order as the approved design

- [ ] **Step 5: Commit the skeleton**

Run: `git add README.md`

Run: `git commit -m "docs: scaffold GitHub profile README"`

Expected: a commit is created with only the new README skeleton

## Task 2: Write the Hero and About Sections

**Files:**
- Modify: `README.md`
- Reference: `docs/superpowers/specs/2026-03-22-github-profile-readme-design.md`

- [ ] **Step 1: Replace the hero placeholder with the final bilingual intro**

Write a short Chinese-first hero block that:

- uses `<github-username>` as the visible identity
- states Java and backend engineering as the main foundation
- states AI applications, agents, and LLM workflows as the active expansion direction

Include concise English support lines only where they improve readability.

- [ ] **Step 2: Write the `About Me` section in 3 short lines**

Write copy that:

- sounds personal but restrained
- avoids resume-style chronology
- emphasizes practical systems rather than trend-chasing

- [ ] **Step 3: Verify the wording stays inside the approved tone**

Run: `Get-Content -Path README.md -Encoding UTF8 | Select-Object -First 40`

Expected: the opening section reads as calm, technical, and personal without generic motivational language

- [ ] **Step 4: Remove any empty or filler phrasing**

Specifically delete lines that sound like:

- "welcome to my GitHub"
- "always learning and growing"
- any exaggerated self-description

- [ ] **Step 5: Commit the intro copy**

Run: `git add README.md`

Run: `git commit -m "docs: draft profile intro"`

Expected: the README now has a stable hero and `About Me`

## Task 3: Add Focus and Tech Stack

**Files:**
- Modify: `README.md`
- Reference: `docs/superpowers/specs/2026-03-22-github-profile-readme-design.md`

- [ ] **Step 1: Fill `Current Focus` with 3 to 4 durable interests**

Use items aligned with the spec, such as:

- Java Backend Engineering
- AI Applications
- Agents and LLM Workflows
- Practical, scalable, product-minded systems

- [ ] **Step 2: Fill `Tech Stack` with a deliberately small set**

Organize it as simple text or short grouped bullets, covering:

- backend tools: Java, Spring Boot, MySQL, Redis
- development and infra: Docker, Git
- AI exploration keywords: LLM Apps, Agents, Workflow Design

- [ ] **Step 3: Verify the stack section is restrained**

Run: `Get-Content -Path README.md -Encoding UTF8 | Select-String -Pattern 'badge|streak|visitor|stats'`

Expected: no output

- [ ] **Step 4: Verify no fake project section was introduced**

Run: `Get-Content -Path README.md -Encoding UTF8 | Select-String -Pattern '^## Projects$|^## Selected Projects$'`

Expected: no output

- [ ] **Step 5: Commit the middle sections**

Run: `git add README.md`

Run: `git commit -m "docs: add focus and tech stack sections"`

Expected: the README now communicates technical direction without relying on completed projects

## Task 4: Finish `Building Next`, Contact, and Final Polish

**Files:**
- Modify: `README.md`
- Reference: `docs/superpowers/specs/2026-03-22-github-profile-readme-design.md`

- [ ] **Step 1: Write the `Building Next` section as a forward-looking placeholder**

Add 2 to 3 items that suggest future work, such as:

- AI-native backend tools
- agent-based developer workflows
- small useful products built from strong engineering foundations

Do not present any item as an already shipped public project.

- [ ] **Step 2: Add the minimal `Contact` section**

Include only the links that actually exist. Start with:

- GitHub profile URL based on `<github-username>`
- public email if `<public-email>` is available
- optional blog only if `<blog-url>` exists

- [ ] **Step 3: Review the full README for rhythm and whitespace**

Run: `Get-Content -Path README.md -Encoding UTF8`

Expected: each section is compact, readable, and separated by clean blank lines

- [ ] **Step 4: Run a final repository diff review**

Run: `git diff -- README.md`

Expected: the diff shows one clean, text-first profile page with no noisy widgets or placeholder junk

- [ ] **Step 5: Commit the polished README**

Run: `git add README.md`

Run: `git commit -m "docs: finalize GitHub profile README"`

Expected: the README is content-complete for v1

## Task 5: Publish the README Through the Special GitHub Profile Repository

**Files:**
- Modify: none
- Verify: `README.md`

- [ ] **Step 1: Create the GitHub profile repository in the web UI**

Create a new public repository named exactly:

```text
<github-username>
```

Rules:

- do not initialize with a README
- do not add a `.gitignore`
- do not add a license yet

- [ ] **Step 2: Rename the local default branch to `main` if needed**

Run: `git branch -M main`

Expected: the current branch name becomes `main`

- [ ] **Step 3: Connect the local repository to the GitHub profile repository**

Run: `git remote add origin https://github.com/<github-username>/<github-username>.git`

Expected: `origin` is added without errors

- [ ] **Step 4: Push the local branch**

Run: `git push -u origin main`

Expected: Git reports that `main` is set to track `origin/main`

- [ ] **Step 5: Verify the public profile page renders the README**

Open:

```text
https://github.com/<github-username>
```

Expected:

- the README content appears on the public profile page
- headings, bilingual text, and spacing render cleanly
- there are no obvious encoding issues in Chinese text

## Done Criteria

This plan is complete when:

- `README.md` exists and is saved as UTF-8
- the README follows the approved structure exactly
- the content is Chinese-first bilingual and technically grounded
- there is no fake project showcase
- the repository has been pushed to the special GitHub profile repo
- the README renders correctly on `https://github.com/<github-username>`

