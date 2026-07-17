# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Directory Purpose

This subdirectory contains technical marketing documentation—the intersection of platform mechanics (Facebook Ads, email, landing pages) and messaging strategy. Documents here translate complicated platform features into actionable guidance, with emphasis on testing and measurement before heavy infrastructure investment.

## Content Structure

- `facebook_sales_campaigns.md` — Meta Ads Manager setup, audience targeting, conversion tracking, and measurement framework

## Key Principle

**Message before mechanics.** Technology amplifies the right message; it rarely rescues the wrong one.

Documents in this directory emphasize:

- Simple testing phases (Phase 1: minimal setup, observe; Phase 2: add tracking if promising; Phase 3: optimize)
- One variable at a time (test new language before testing mechanics)
- Measurement first (define what you're measuring before building infrastructure)
- Avoiding premature complexity (don't install Pixels until you know the message works)

## Audience

Technical marketing guidance is intended for:

- Wendy and team (implementation and testing)
- Michael (technical oversight and architecture review)
- Future collaborators (clear handoff of what's been tested, what's next)

## Markdown Maintenance

Follow parent directory conventions:

```bash
markdownlint --fix --config ~/.markdownlint.json <file>
```

Prose paragraphs are single long lines; structural elements preserve natural breaks.
