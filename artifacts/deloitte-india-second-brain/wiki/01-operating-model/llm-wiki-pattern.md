---
title: LLM Wiki Pattern
type: concept
tags: [karpathy, llm-wiki, architecture]
status: active
updated: 2026-05-14
source_count: 1
---

# LLM Wiki Pattern

Andrej Karpathy's LLM Wiki pattern reframes knowledge management as compilation. Instead of retrieving raw chunks every time a person asks a question, an agent reads new material and updates a persistent Markdown wiki.

## Structure

- Raw sources: immutable input material.
- Wiki: generated Markdown pages, maintained by the LLM.
- Schema: instructions that tell the agent how to ingest, query, lint, and maintain the wiki.

## Operations

- Ingest: read a source, summarize it, update relevant pages, add cross-links, and log the change.
- Query: answer from the compiled wiki, then write valuable answers back into the wiki.
- Lint: periodically find stale claims, contradictions, missing links, broken links, orphan pages, and missing concepts.

## How It Applies Here

For Deloitte India, the important shift is from "news clipping" to "living synthesis". The scanner may discover a new DPDP update, RBI direction, or Deloitte report, but the durable work is updating [[DPDP Privacy Compliance]], [[Regulatory Radar]], or [[AI At Scale]] so future readers inherit the synthesis.

## Sources

- [Andrej Karpathy, LLM Wiki gist](https://gist.github.com/karpathy/442a6bf555914893e9891c11519de94f)

