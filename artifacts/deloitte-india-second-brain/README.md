# Deloitte India Living Second Brain

Public-source, Markdown-first second brain for Deloitte India professionals.

This workspace instantiates two ideas:

- Andrej Karpathy's LLM Wiki pattern: immutable raw sources, a compiled Markdown wiki, and a schema file that tells the agent how to maintain the wiki.
- Garry Tan's GBrain pattern: compiled truth pages, entity and topic pages, timelines, backlinks, recurring scans, and skills that turn repeat work into durable operating procedure.

## What is included

- `wiki/`: human-readable Markdown wiki pages with YAML frontmatter, wikilinks, source links, and update notes.
- `raw/sources/`: source register for the seed research.
- `raw/news/`: generated news captures from the internet scanner.
- `tools/scan_news.py`: deterministic RSS/news scanner for 6-hour radar updates.
- `tools/build_html.py`: builds `index.html` from the Markdown wiki.
- `tools/build_latest.py`: builds `latest.html` from the current radar inbox.
- `AGENTS.md`: the maintenance schema for future Codex/LLM sessions.
- `index.html`: colorful Deloitte-inspired wiki reader generated from the Markdown files.
- `architecture.html`: visual architecture map of the living second brain.
- `latest.html`: aesthetic latest-intelligence briefing generated from the radar.

## Refresh flow

Run this from the workspace root:

```bash
python3 deloitte-india-second-brain/tools/scan_news.py
python3 deloitte-india-second-brain/tools/build_html.py
python3 deloitte-india-second-brain/tools/build_latest.py
```

The scanner fetches relevant public news/RSS signals, scores them for Deloitte India relevance, deduplicates previously seen URLs, writes captures under `raw/news/`, updates the inbox radar, and rebuilds the HTML reader.

## Editorial rule

This is a synthesis layer, not a mirror of the internet. Do not paste full articles into the wiki. Keep raw source links, summarize claims in original words, and mark confidence and freshness.
