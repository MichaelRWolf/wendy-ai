# Iterative Summary Plan

Companions:
- [notes-wendy_summary.md](notes-wendy_summary.md) – completed conversation summary generated from this plan.
- [notes-wendy_summary_critique.md](notes-wendy_summary_critique.md) – candid evaluation of the plan’s business alignment and risks.

## Scope Confirmation
- Inspect `notes-wendy.md` to confirm 8 118 lines and identify dialogue/transcript boundaries while respecting ≤400-line chunks.

## Chunked Analysis Loop
- For each chunk, classify as planning dialogue or podcast transcript.
- Dialogue: populate `notes-wendy_summary.md` following the required structure:
  - `# Title`
  - `## Planning Dialog`
    - `### Summary of conversation flow` with a single paragraph per sub-flow at ~10% of source word count
    - `### Goals of the project that was discussed`
    - `### Decisions (i.e. filename conventions, workflow, inputs, work products (outputs))`
    - `### Outstanding Questions`
    - `### Action Plan`
- Transcript: under `## Injested Files`, add `### <filename>` sections summarizing each ingested file (reuse existing summaries when present, otherwise create ~5% word-count summary) and include metadata (line count, max timestamp, speaker roster, per-speaker word counts, estimated talk durations, final timestamp).

## Progress & Guidance Sync
- After each chunk, report processed line ranges and pause for “continue analysis” before proceeding.

## Finalization
- Once all chunks are processed, consolidate the “Action Plan” content, ensure `notes-wendy_summary.md` matches the template, then export the finalized plan text to `notes-wendy_summary.plan.md` for reuse.

## Review & Next Steps
- Present the updated `notes-wendy_summary.md` for review and confirm no further direction is pending before ending the session.

