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

## Document Organization

Files follow a naming pattern that groups related content:

- `notes-<name>.md` — raw notes and observations from a given perspective (Michael, Wendy, etc.)
- `notes-<base>_summary.md` — curated synthesis and key takeaways
- `notes-<base>_summary.plan.md` — structured plan derived from summary analysis
- `notes-<base>_summary_critique.md` — critical review of the synthesis
- `critiques_from_team_POV.md` — multi-perspective reviews organized by role/function
- `<topic>_transitions.md` — connective analysis between topics

## Cross-Linking and Structure

Documents use cross-references (see git history: `d891d5e`, `ce3ac0b`) to map relationships:

- Link between summary and raw notes so readers can drill down from synthesis
- Group related critiques by role or perspective
- Use headings and subheadings to organize perspectives (Critical Review, Supportive Review, Success Vision, Failure Risks)

When adding new analysis:

1. Keep raw notes and synthesis separate
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
