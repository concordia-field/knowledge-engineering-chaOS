---
id: <type>.<slug>
type: <type>
archetype: <entity | concept | claim | experiment | example | teaching | analogy>
name: <Display name>
summary: >
  <The intent: one self-contained sentence.>
status: open
maturity: seed
revision: 1
scope: <where this holds, and where it stops>
sources:
  - id: source.<slug>
    role: <primary | definition | reference | data | validation | justification | historical | synthesis | secondary>
    locator: <page, section, timestamp — as precise as the source allows>
relations: []
assumptions: []               # ASM ids relied on; an open one caps status at `conditional`
review: not-yet-developed
# From maturity `reviewed`, replace the line above with:
# review:
#   reviewer: <name>
#   reviewer_kind: human
#   authority: <role that gives the right to decide>
#   decision: approved
#   date: YYYY-MM-DD
#   reference: audits/batch-<n>.md
---

# <Display name>

## Context

<In which circumstances does this have meaning? Scope, boundary, assumptions.>

## Description

<What it is, in plain language, distinct from its neighbours. Ordinary picture first.>

## Properties

<What characterises it. Facts with source and locator. Keep apart:>

- **Observed:** <fact> (source.<slug>, <locator>)
- **Attributed:** <what a named source claims; not asserted here>
- **Interpretation:** <labelled as such, or Not applicable: reason>

## Behaviour

<What happens: rules, changes, procedure, justification. Or: Not applicable: <reason>.>

## Relations

<How it connects, and how. Name the bond, not just the link.>

### Sources

| Source | Role | Locator |
|---|---|---|
| source.<slug> | <role> | <locator> |
