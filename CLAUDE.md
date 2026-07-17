# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Purpose

This repository documents the Wendy AI project—conference notes, analysis, structured critiques, and knowledge synthesis from the AI Advantage Summit and related stakeholder perspectives.

## Markdown Maintenance

Markdown linting follows the global configuration with line-length enforcement disabled:

```bash
markdownlint --fix --config ~/.markdownlint.json <file>
```

Apply fixes to all markdown in the repo:

```bash
markdownlint --fix --config ~/.markdownlint.json *.md
```

Per the global CLAUDE.md rules:
- Prose paragraphs are one long line with no embedded newlines (soft-wrap via editor)
- Structural elements (lists, tables, code blocks) preserve natural line breaks
- `M-q` in emacs unfills hard-wrapped prose back into single lines

## Repository Structure

The repository is organized into two project subdirectories, each with its own CLAUDE.md:

### `ai-advantage-summit-2025/`

Conference notes and team analysis from the 3-day AI Advantage Summit 2025 that Michael attended with Wendy.

- `notes-michael.md` — Raw conference notes organized by day
- `critiques_from_team_POV.md` — Multi-perspective team analysis of speaker insights and themes

### `wendy-clone-project/`

Design and planning documentation for the custom-built Wendy Clone / BLOOM_AI_Core AI system, an alternative to the Tony Robbins/Dean Graziosi bootcamp.

- `notes-wendy.md` — Full ChatGPT conversation transcript of system design
- `notes-wendy_summary.md` — Curated synthesis organized by topic
- `notes-wendy_summary.plan.md` — Structured implementation plan
- `notes-wendy_summary_critique.md` — Critical review and feasibility assessment
- `notes-wendy_transitions.md` — Connective analysis linking themes

### Root Level

- `CLAUDE.md` — Repository-wide guidance
- `README.md` — High-level project overview
- `.markdownlint.json` — Markdown linting configuration

## Document Conventions

Within each project subdirectory, follow these patterns:

- `notes-<name>.md` — raw notes or source material (conference observations, conversation transcripts)
- `notes-<base>_summary.md` — curated synthesis extracted from source
- `notes-<base>_summary.plan.md` — structured plan derived from analysis
- `notes-<base>_summary_critique.md` — critical review of feasibility, risks, and assumptions
- `notes-<base>_transitions.md` — connective analysis bridging topics or documents

### Cross-Linking

Documents use cross-references (see git history: `d891d5e`, `ce3ac0b`) to map relationships:

- Link between summary and raw notes so readers can drill down from synthesis
- Group related critiques by role or perspective
- Use "See also" sections to surface related documents in other subdirectories

### Editing Guidelines

When adding or updating analysis:

1. Keep raw notes and synthesis in separate files
2. Add "See also" or link sections to surface related documents
3. Organize complex critiques by perspective (Critical, Supportive, Vision, Risk)
4. Run markdownlint before committing

## Git Workflow

Commits typically involve:

- Adding or reorganizing notes
- Extracting summaries from raw content
- Applying markdown fixes (`markdownlint --fix`)
- Cross-linking documents for coherence

Use descriptive commit messages that name what changed (e.g., "Add success vision and failure risks for each role").
