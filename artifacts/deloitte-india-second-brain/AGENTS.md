# Deloitte India Second Brain Schema

This file is the operating manual for agents maintaining the Deloitte India second brain.

## Purpose

Maintain a living, public-source knowledge base for Deloitte India professionals. The wiki should help teams brief themselves quickly on market signals, regulatory shifts, client issues, Deloitte offerings, and reusable consulting perspectives.

## Layers

1. Raw sources
   - Location: `raw/`
   - Immutable captures and source registers.
   - Agents may add new source files, but should not rewrite a captured source except to fix metadata.
2. Wiki
   - Location: `wiki/`
   - Compiled synthesis in Markdown.
   - Agents own this layer: create pages, update pages, add backlinks, reconcile contradictions, and keep summaries current.
3. Schema
   - Location: `AGENTS.md`
   - This file. Update only when the operating model changes.
4. HTML reader
   - Location: `index.html`
   - Generated view. Rebuild with `python3 tools/build_html.py`; do not hand-edit generated markup unless the generator is updated too.

## Page Types

Use YAML frontmatter on every wiki page:

```yaml
---
title: Page title
type: map | concept | source-synthesis | radar | playbook | briefing
tags: [tag-one, tag-two]
status: seeded | active | needs-review
updated: YYYY-MM-DD
source_count: 0
---
```

Preferred folders:

- `00-inbox/`: untriaged internet radar and fresh signals.
- `01-operating-model/`: how the second brain works.
- `02-market-context/`: macro, budget, talent, and industry context.
- `03-client-issues/`: board and client-facing issue pages.
- `04-industries/`: sector-specific pages.
- `05-deloitte-india/`: Deloitte India offering and team context.
- `06-briefings/`: recurring executive readouts.

## Ingest Protocol

When ingesting a source:

1. Identify the source type, publisher, date, URL, and why it matters.
2. Add or update a raw source note if the item is durable.
3. Update the most specific wiki page first.
4. Update higher-level map pages only if the signal changes the synthesis.
5. Add wikilinks to related concepts.
6. Add source links inline under "Sources".
7. Append `wiki/log.md` with the ingest date, action, and touched pages.
8. Rebuild the HTML reader.

## Quality Bar

- Cite the public URL for factual claims.
- Prefer official Deloitte, regulator, ministry, exchange, and central-bank sources before media summaries.
- Keep source quotes under short excerpts only; paraphrase the rest.
- Mark uncertain or fast-moving claims as `needs-review`.
- Do not treat a source as true merely because it is recent.
- Separate facts, implications, and suggested actions.
- For legal, tax, audit, or regulatory content, avoid advice language; phrase as "watch item", "discussion prompt", or "needs specialist review".

## Link Conventions

- Use wikilinks for internal pages: `[[AI At Scale]]`.
- Use normal Markdown links for external sources.
- When a concept is mentioned on three or more pages, consider creating a dedicated concept page.
- Every page should have at least one outbound wikilink unless it is an inbox capture.

## Living Radar

The 6-hour scanner should feed `wiki/00-inbox/radar.md`. Agents should periodically promote durable items from the inbox into topic pages and leave weaker items in the inbox.

Promotion test:

- Is the source credible?
- Is the signal relevant to Deloitte India clients or professionals?
- Does it change an existing synthesis, create a new issue, or add a deadline?
- Can the claim be connected to at least one existing page?

## Lint Protocol

During maintenance, check for:

- Broken wikilinks.
- Pages with no sources.
- Stale pages older than 30 days in fast-moving topics.
- Contradictions between source pages and synthesis pages.
- Orphan pages with no inbound links.
- Overgrown pages that should split into a map plus child pages.

