---
name: audit-data-profiler
description: Profile Deloitte USI audit datasets such as general ledger, journal entries, trial balance, AP, AR, revenue, inventory, payroll, fixed assets, vendors, customers, and workpaper extracts. Use when the user needs completeness checks, row counts, control totals, field profiling, candidate keys, duplicates, exception criteria, or audit-ready data observations.
---

# Audit Data Profiler

## Problem It Solves

Audit extracts get profiled before testing, with source trails and control totals.

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
