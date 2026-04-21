# DRIFT Wiki

This directory is a persistent, LLM-maintained synthesis layer for this repository.

## Architecture

- Raw sources (read-only): root markdown files, `docs/`, `background/`
- Maintained knowledge layer: `wiki/` markdown pages
- Operational control files:
  - `index.md` (catalog)
  - `log.md` (append-only operations timeline)
  - `sources.md` (ingest coverage tracker)

## Operating Loop

1. Ingest new or updated source files into wiki pages.
2. Query the wiki for synthesis and comparison.
3. File durable query outputs back into wiki pages.
4. Lint regularly for contradictions, broken links, and coverage gaps.

## Quick Prompts For Copilot

- `ingest all pending`
- `ingest docs/l1_context_matrix_v2.md`
- `query wiki: what is the highest-risk action misfit pattern?`
- `refresh index`
- `show recent activity`
- `lint wiki`

## Notes

- `background/` is currently available as a source category and can be ingested when files are added.
- This wiki is intentionally markdown-first and git-friendly.
