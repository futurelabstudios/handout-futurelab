# Deloitte USI Skill Repository

Ten downloadable `SKILL.md` files for common Deloitte USI workflows. Each sample is meant to be copied into its own skill folder as `SKILL.md`, then customized with approved team sources, templates, review rules, and confidentiality constraints.

## Download Links

- [Download complete skill kit](deloitte-usi-skill-files.zip)
- [Executive Briefing](skill-files/executive-briefing/SKILL.md)
- [Meeting To Action](skill-files/meeting-to-action/SKILL.md)
- [Presentation Storyline](skill-files/presentation-storyline/SKILL.md)
- [Spreadsheet Insight](skill-files/spreadsheet-insight/SKILL.md)
- [Audit Data Profiler](skill-files/audit-data-profiler/SKILL.md)
- [Research Synthesis](skill-files/research-synthesis/SKILL.md)
- [Proposal Response](skill-files/proposal-response/SKILL.md)
- [Process Documentation](skill-files/process-documentation/SKILL.md)
- [Second Brain Curator](skill-files/second-brain-curator/SKILL.md)
- [Risk And Control Review](skill-files/risk-control-review/SKILL.md)

## 01. Executive Briefing Skill

Problem it solves: Turns scattered notes, reports, emails, and working analysis into a crisp leadership-ready brief.

```markdown
---
name: executive-briefing
description: Create concise executive briefs from notes, reports, emails, transcripts, analyses, and source documents. Use when the user needs a leadership-ready summary, decision memo, client update, board-style note, or one-page synthesis with implications, evidence, risks, and next actions.
---

# Executive Briefing

## Workflow

1. Confirm audience, decision context, time horizon, and desired length.
2. Inventory the source material and separate facts from interpretation.
3. Extract the core issue, recommendation, evidence, risks, dependencies, and open questions.
4. Write in a consulting style: direct headline, short sections, quantified evidence where possible.
5. Include source references or filenames when available.
6. End with decisions needed, owner, and next action.

## Output

Use this structure:

- Situation
- So what
- Recommendation
- Evidence
- Risks and mitigations
- Decisions needed
- Next actions

## Quality Gate

Flag missing source evidence, unclear assumptions, numbers that need validation, and any content that may be confidential or client-sensitive.
```

## 02. Meeting To Action Skill

Problem it solves: Converts meeting notes or transcripts into decisions, actions, risks, and follow-ups.

```markdown
---
name: meeting-to-action
description: Convert meeting notes, transcripts, recordings, or rough bullets into decisions, action items, risks, blockers, open questions, and stakeholder follow-ups. Use for internal team meetings, client workshops, governance forums, project check-ins, and post-meeting documentation.
---

# Meeting To Action

## Workflow

1. Identify meeting purpose, date, attendees, and business context.
2. Separate confirmed decisions from discussion points and assumptions.
3. Extract actions with owner, due date, dependency, and expected output.
4. Capture risks, blockers, unresolved questions, and escalation items.
5. Produce a concise follow-up note ready to send or paste into a tracker.

## Output

Return:

- Meeting summary
- Decisions made
- Action register
- Risks and blockers
- Open questions
- Suggested follow-up message

## Quality Gate

Do not invent owners or due dates. Mark missing values as `TBD`. Flag sensitive client, employee, or financial details before sharing.
```

## 03. Presentation Storyline Skill

Problem it solves: Turns raw thinking into a deck narrative with slide titles, exhibit ideas, and executive flow.

```markdown
---
name: presentation-storyline
description: Build consulting-style presentation storylines from raw notes, analyses, data points, workshop outputs, or draft bullets. Use when the user needs a slide outline, executive narrative, section flow, slide titles, exhibit recommendations, or speaker notes.
---

# Presentation Storyline

## Workflow

1. Clarify audience, objective, decision to influence, and meeting length.
2. Create a storyline with one message per slide.
3. Convert vague section labels into action-oriented slide titles.
4. Recommend exhibits: chart, table, process flow, operating model, timeline, or decision matrix.
5. Add speaker notes only where they clarify the argument.

## Output

Use a table with:

- Slide number
- Slide title
- Core message
- Suggested visual
- Source or input needed
- Speaker note

## Quality Gate

Check that the deck has a clear opening answer, logical flow, no duplicated slides, and a specific close or decision ask.
```

## 04. Spreadsheet Insight Skill

Problem it solves: Helps users understand, clean, test, and explain spreadsheet-based analysis.

```markdown
---
name: spreadsheet-insight
description: Analyze spreadsheets, tables, CSVs, and Excel-style workbooks for structure, data quality, formulas, outliers, summaries, and business insights. Use when the user needs spreadsheet profiling, formula explanation, data cleanup suggestions, pivot logic, exception checks, or an insight summary from tabular data.
---

# Spreadsheet Insight

## Workflow

1. Identify sheets, tables, row counts, column names, and key fields.
2. Profile missing values, duplicates, date ranges, numeric ranges, and unusual categories.
3. Explain formulas and dependencies in plain language.
4. Identify outliers, breaks, reconciliation issues, or inconsistent labels.
5. Convert findings into business implications and next checks.

## Output

Return:

- Dataset overview
- Data quality observations
- Key calculations or formulas
- Outliers or exceptions
- Suggested cleanup or validation steps
- Executive insight summary

## Quality Gate

Do not change source data unless explicitly asked. Preserve assumptions, filters, and any rows excluded from analysis.
```

## 05. Audit Data Profiler Skill

Problem it solves: Creates an evidence-aware workflow for profiling audit extracts before testing.

```markdown
---
name: audit-data-profiler
description: Profile audit datasets such as general ledger, journal entries, trial balance, AP, AR, revenue, inventory, payroll, fixed assets, vendors, customers, and workpaper extracts. Use when the user needs completeness checks, row counts, control totals, field profiling, candidate keys, duplicates, exception criteria, or audit-ready data observations.
---

# Audit Data Profiler

## Workflow

1. Preserve raw files and record filenames, extract dates, sheet names, row counts, and column counts.
2. Identify candidate keys, amount fields, date fields, status fields, user fields, and reference numbers.
3. Profile nulls, duplicates, ranges, unusual values, and low-frequency categories.
4. Tie totals to control totals, trial balance, subledger, or prior workpaper references where available.
5. Separate observations from audit conclusions.

## Output

Return:

- Scope and source files
- Population overview
- Control totals and reconciliation status
- Field quality observations
- Candidate tests
- Exception criteria
- Limitations and follow-up

## Quality Gate

Do not expose sensitive row-level data unnecessarily. Treat red flags as items for audit follow-up, not final conclusions.
```

## 06. Research Synthesis Skill

Problem it solves: Converts multiple articles, reports, websites, and notes into a sourced research memo.

```markdown
---
name: research-synthesis
description: Synthesize research from articles, websites, reports, market scans, interview notes, and internal documents into a sourced consulting memo. Use when the user needs an industry brief, competitor summary, technology landscape, trend analysis, source comparison, or implications for a client or internal team.
---

# Research Synthesis

## Workflow

1. Clarify research question, audience, geography, sector, and decision context.
2. Separate facts, source claims, assumptions, and implications.
3. Compare sources for agreement, disagreement, recency, and credibility.
4. Extract implications for strategy, risk, operating model, talent, technology, and next actions.
5. Provide citations or links for all material claims.

## Output

Use this structure:

- Executive answer
- Key findings
- Evidence table
- Contradictions or uncertainty
- Implications
- Recommended next research

## Quality Gate

Flag outdated sources, weak evidence, unsupported claims, and areas requiring primary validation.
```

## 07. Proposal Response Skill

Problem it solves: Helps teams structure proposals, RFP responses, and client-ready solution narratives.

```markdown
---
name: proposal-response
description: Draft and improve proposals, RFP responses, client pitches, capability statements, and solution narratives. Use when the user needs win themes, response structure, executive summary, scope, approach, timeline, assumptions, risks, differentiators, or review comments for a client-facing proposal.
---

# Proposal Response

## Workflow

1. Identify client need, decision criteria, scope, timeline, and must-answer questions.
2. Create win themes tied to client outcomes.
3. Draft a response structure with clear sections and proof points.
4. Map capabilities, methodology, deliverables, team roles, risks, and assumptions.
5. Review for executive clarity, differentiation, and compliance with RFP instructions.

## Output

Return:

- Executive summary
- Win themes
- Response outline
- Proposed approach
- Deliverables
- Assumptions and dependencies
- Risks and mitigations
- Review checklist

## Quality Gate

Do not invent credentials, case studies, pricing, or commitments. Mark missing proof points and approvals required.
```

## 08. Process Documentation Skill

Problem it solves: Converts workflow knowledge into SOPs, RACI, controls, and training-ready documentation.

```markdown
---
name: process-documentation
description: Convert rough workflow notes, interviews, process maps, screenshots, policies, and operating knowledge into SOPs, RACI tables, control points, checklists, and training documentation. Use when the user needs a repeatable process document or process improvement summary.
---

# Process Documentation

## Workflow

1. Identify process objective, trigger, inputs, systems, roles, outputs, and frequency.
2. Map current-state steps in sequence.
3. Capture handoffs, approvals, controls, exceptions, and decision points.
4. Convert into SOP language with clear owners and evidence requirements.
5. Identify gaps, risks, improvement ideas, and automation candidates.

## Output

Return:

- Process objective
- Scope and trigger
- RACI
- Step-by-step SOP
- Controls and evidence
- Exceptions and escalations
- Improvement opportunities

## Quality Gate

Flag ambiguous ownership, missing approvals, unclear evidence, and steps requiring policy confirmation.
```

## 09. Second Brain Curator Skill

Problem it solves: Keeps a knowledge base fresh, linked, source-backed, and ready for AI interaction.

```markdown
---
name: second-brain-curator
description: Maintain a source-backed second brain by ingesting notes, links, documents, decisions, prompts, and project updates into structured markdown pages. Use when the user needs to create, refresh, deduplicate, link, summarize, or query a living knowledge base for a person, team, project, function, or department.
---

# Second Brain Curator

## Workflow

1. Start from the team `SKILL.md`: role, sources, confidentiality rules, output formats, and review gates.
2. Ingest approved sources and preserve raw source references.
3. Distill into durable wiki pages: projects, people, decisions, risks, processes, definitions, and reusable prompts.
4. Link related pages using consistent names and backlinks.
5. Mark freshness: last updated date, source, owner, confidence, and review status.
6. Write validated learnings back into the brain after each useful AI interaction.

## Output

Return:

- New or updated pages
- Source trail
- Links created
- Stale pages needing review
- Open questions
- Suggested next refresh

## Quality Gate

Do not overwrite human-approved pages without flagging the change. Separate source facts from AI synthesis.
```

## 10. Risk And Control Review Skill

Problem it solves: Reviews outputs for risk, assumptions, controls, confidentiality, and readiness before sharing.

```markdown
---
name: risk-control-review
description: Review drafts, analyses, AI outputs, workpapers, presentations, emails, and proposed automations for risks, assumptions, controls, confidentiality, evidence quality, and stakeholder readiness. Use before sharing client-facing, leadership-facing, audit-supporting, or decision-critical material.
---

# Risk And Control Review

## Workflow

1. Identify audience, decision impact, confidentiality level, and whether the output is client-facing.
2. Check claims against available sources.
3. Identify assumptions, missing evidence, unsupported numbers, and overstatements.
4. Review confidentiality, personal data, client-sensitive data, and inappropriate disclosure risk.
5. Check ownership, approvals, review status, and next action.
6. Recommend edits in priority order.

## Output

Return:

- Readiness rating
- Critical issues
- Assumptions to validate
- Evidence gaps
- Confidentiality risks
- Required approvals
- Suggested edits

## Quality Gate

Be conservative. When source evidence is missing or sensitive data may be exposed, recommend review before use.
```
