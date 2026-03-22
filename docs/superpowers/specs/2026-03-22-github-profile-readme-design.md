# GitHub Profile README Design

Date: 2026-03-22
Status: Approved

## 1. Background

This project is the local starting point for a GitHub profile homepage. The user has not yet created the special profile repository on GitHub, and there are no completed showcase projects to feature right now.

The eventual GitHub repository must use the same name as the user's GitHub username so that the `README.md` becomes the public profile homepage.

## 2. Goal

Create a GitHub profile README that:

- presents a strong technical identity
- emphasizes Java and backend engineering as the core track
- shows active exploration of AI applications, agents, and LLM workflows
- feels simple, spacious, and polished rather than template-heavy
- works well even before any real project portfolio exists

## 3. Non-Goals

This first version should not:

- depend on having multiple completed projects
- look like a resume dump
- rely on dense badge walls, noisy stats, or decorative clutter
- overclaim experience with generic slogans
- imitate a flashy portfolio site inside a README

## 4. Audience

Primary audience:

- developers who visit the profile through GitHub
- potential collaborators
- future recruiters or hiring managers
- people evaluating technical direction and taste, not just raw activity volume

Expected first impression:

- grounded in backend engineering
- curious about AI-native systems
- capable of building practical systems, not only experimenting with trends

## 5. Positioning

The profile should communicate this identity:

> A Java/backend engineer who is steadily extending into AI applications, agent systems, and LLM-driven workflows.

Tone requirements:

- bilingual, with Chinese as the primary language
- concise and expressive
- more personal than a plain corporate summary
- still restrained and technically credible

## 6. Chosen Direction

Three directions were considered:

1. minimalist engineer card
2. light creator-style technical profile
3. metrics and stats driven profile

The selected direction is option 2:

`light creator-style technical profile`

Reason:

- it fits the user's wish for a homepage that is simple and atmospheric
- it allows personality without becoming noisy
- it does not require existing projects to look complete
- it supports future growth into a project showcase naturally

## 7. Content Strategy

Because there are no finished projects yet, the README should establish identity through:

- who the user is
- what technical areas the user is currently focused on
- what kinds of systems the user wants to build next

The README should avoid pretending that a large body of public work already exists. Instead, it should feel intentional, early-stage, and forward-moving.

## 8. Information Architecture

The README should follow this structure:

1. hero section
2. about me
3. current focus
4. tech stack
5. building next
6. contact

### 8.1 Hero Section

Purpose:

- establish identity immediately
- deliver a clear technical direction in one glance

Content:

- GitHub ID as the main heading
- one short bilingual positioning statement
- one short bilingual supporting paragraph

Rules:

- no inflated claims
- no generic passion statements
- no long opening paragraph

### 8.2 About Me

Purpose:

- explain the user's technical personality in a compact way

Content shape:

- around 3 short lines
- backend engineering as the foundation
- AI applications, agents, and LLM workflows as the expansion direction
- emphasis on practical, usable systems

### 8.3 Current Focus

Purpose:

- replace a missing project section with active technical intent

Recommended items:

- Java Backend Engineering
- AI Applications
- Agents and LLM Workflows
- Practical, scalable, product-minded systems

Rules:

- keep this list short
- prefer stable interests over temporary experiments

### 8.4 Tech Stack

Purpose:

- provide technical recognizability without turning the README into a badge wall

Recommended categories:

- Backend: Java, Spring Boot, MySQL, Redis
- Dev and Infra: Docker, Git
- AI Exploration: LLM Apps, Agents, Workflow Design

Rules:

- only include technologies the user is comfortable being associated with
- keep the set intentionally small
- prefer clean text or a few restrained icons over many badges

### 8.5 Building Next

Purpose:

- reserve space for future output without faking a project catalog

Suggested content:

- AI-native backend tools
- agent-based developer workflows
- small useful products built from strong engineering foundations

Evolution path:

- this section can later become `Selected Projects`

### 8.6 Contact

Purpose:

- give a lightweight path for follow-up

Allowed items:

- GitHub
- email
- blog or personal site if one exists later

Rules:

- keep only essential links

## 9. Visual and Writing Principles

The README should feel like a cover page, not a dashboard.

### 9.1 Layout

- maintain generous whitespace
- keep sections compact
- avoid table-heavy layout
- avoid unnecessary separators

### 9.2 Writing Style

- specific rather than motivational
- calm rather than loud
- expressive but not theatrical
- technically grounded

Avoid lines such as:

- love coding and life
- always learning and growing
- welcome to my GitHub

### 9.3 Bilingual Strategy

Chinese should be primary.

Recommended bilingual usage:

- bilingual hero statement
- bilingual section titles if useful
- selective English support for core identity phrases

The README does not need line-by-line mirrored translation everywhere. Over-translation will make the page feel heavier and less natural.

### 9.4 Visual Elements

Recommended default:

- rely mostly on typography, spacing, and section rhythm

Optional later additions:

- a small number of restrained icons
- at most one low-noise GitHub stats block

Not recommended for v1:

- many badges
- streak charts
- visitor counters
- animated gimmicks

## 10. Example Tone

The writing should feel close to this:

```md
# Hi, I'm <GitHub ID>

[Primary Chinese positioning sentence]
I build with Java and backend systems, while exploring AI-native applications, agents, and LLM workflows.

[Primary Chinese supporting sentence]
I care about turning solid engineering into useful systems and products.
```

This sample defines tone only. The final copy should be refined for the user's actual GitHub ID and final wording choices.

## 11. Implementation Notes

When implementation starts:

- create the profile `README.md`
- save the final `README.md` as UTF-8
- keep the first version text-first
- avoid adding a fake projects section
- make `Building Next` the forward-looking placeholder area
- keep the file easy to update as real projects appear

The local repository can be prepared now, but the GitHub-side profile repository must eventually be created under the exact GitHub username.

## 12. Acceptance Criteria

The design is successful if:

- the page feels clean and confident
- a visitor can quickly identify the user as Java/backend-first with AI direction
- the page still looks complete even without existing public projects
- the writing sounds personal but not self-indulgent
- future project growth can be added without restructuring the whole page
