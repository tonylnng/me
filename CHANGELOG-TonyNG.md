# Changelog — TonyNG.md / TonyNG-EN.md

All notable changes to the personal AI-onboarding profile (`TonyNG.md` and `TonyNG-EN.md`) are documented here.

This changelog focuses on **what changed and why** — not just the diff. It doubles as a public log of how I've refined the way I work with AI agents over time.

Format inspired by [Keep a Changelog](https://keepachangelog.com/).
Versioning is informal — `vN` marks meaningful structural revisions, not every micro-edit.

---

## [v3 / EN] — 2026-05-12

### Added
- **English version** (`TonyNG-EN.md`) — for international AI agents and English-speaking collaborators. Not a literal translation — uses English imperative voice ("Never open with...", "Lead with the conclusion") which English LLMs follow more precisely.
- **Bilingual default in EN version**: header explicitly instructs "respond in Traditional Chinese (HK) by default; switch to English only when I write in English first" — preserves Chinese-first working environment even when the EN file is loaded.

### Why
Some AI tools (especially US-hosted enterprise platforms) treat non-English system prompts as second-class. Having an EN version that still mandates Chinese responses gets the best of both worlds.

---

## [v3] — 2026-05-12

### Changed
- **§12 closing instruction** rewritten from a single ambiguous line into **3 conditional rules**:
  1. First time reading → 5–10 sentence summary of understanding
  2. Already read (same session / project / vault) → skip ack, get to work
  3. Tony explicitly asks "do you understand me?" → re-output full understanding
- **§9 trailing whitespace bug** fixed (`**HKT (UTC+8) **` → `**HKT (UTC+8)**`)

### Why
v2's closing "please summarize your understanding in 5–10 sentences" conflicted with Rule 1 ("don't restate my question"). It also caused token waste on every conversation. The new conditional structure separates one-time onboarding from daily interaction.

---

## [v2] — 2026-05-12

### Changed
- **§1 Role** generalized: `CTO · Senior Director` → `Senior Tech Executive (CTO / Senior Director level)` — removes ambiguity about whether it's one title or two
- **§3 side tracks** restructured: split into "side tracks" + standalone "long-term goal" subsection, added "open source contributions" item, named specific verticals (healthcare, finance, government)
- **§4 tech environment** added explicit "default stack" code block + one-line directive — prevents AI from defaulting to Python/Windows assumptions

### Removed
- Specific company name (ASL) — kept the file portable across professional contexts
- Detailed cron scheduling specifics (frequency limits) — too implementation-specific for a profile doc

### Why
Earlier version was too tied to my current employment context. AI agents need patterns and preferences — not org chart details that go stale.

---

## [v1] — 2026-05-12

### Added
- **Initial release** of `TonyNG.md` — a 12-section AI-onboarding profile in Traditional Chinese (HK)
- Sections: Identity snapshot · Five golden interaction rules · Active projects · Tech stack · Thinking style · Response format · Code preferences · Content creation · Time/notifications · Red lines · Typical question types · One-line summary
- **Self-aware blind spots section** — derived from a multi-framework personality analysis (MBTI ENTJ-A · DISC D/C high-high · Big Five O92/C95/N15 · Enneagram 8w1). The AI is explicitly authorized to call out four recurring patterns: weak F dimension, pacesetting overload, won't-let-go gate reviews, perfectionist procrastination.

### Design decisions
- **Audience: AI, not humans** — the file optimizes for what AI agents need to model a user, not what would impress a recruiter
- **Imperative voice over descriptive** — "Lead with the conclusion" beats "I prefer answers that start with the conclusion"
- **Pattern over biography** — "I'm a Disciplined Pioneer who owns every gate" beats "I worked at Company X for 5 years"

---

## Conventions

- **Major rewrites**: bump `vN`, document under a new heading
- **Small edits / typo fixes**: no entry needed
- **Breaking changes to AI behavior** (e.g., closing instruction rewrite): always documented with "Why" rationale
- **Dates**: ISO format (YYYY-MM-DD), Hong Kong time
