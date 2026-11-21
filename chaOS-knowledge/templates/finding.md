---
id: finding.<slug>
type: finding
archetype: claim
name: <Short title of the finding>
summary: >
  <The finding and its assessment, in one sentence.>
purpose: <audit | journalism | legal>
question: <the question this finding answers>
scope: <what was reviewed: sources, period, places, population>
audience: <who will read the output>
lens: <the perspective shaping interpretation, or not-applicable>
status: open                  # kind of truth of the objective finding (O)
conformity: not-yet-developed # conforms | partly-conforms | departs | not-assessable
maturity: draft
criterion:
  id: source.<slug>
  locator: <exact clause or provision>
  version: <edition in force at the time>
evidence:                     # separate support per step
  finding: [source.<slug>]
  action: [source.<slug>]
  outcome: [source.<slug>]
questions: []                 # ids from the questions register
assumptions: []               # ASM ids relied on; an open one caps status at `conditional`
review: not-yet-developed
---

# <Short title of the finding>

## O · Objective finding

<On [date] at [place], it was established that [condition]. Supported by [source id, locator]. Attributed accounts are named as such.>

## S · Standard

<The exact criterion and edition, why it applies, and what it required or led one to expect.>

## C · Chronology and context

| Date (precision) | Event | Actor and role | Source |
|---|---|---|---|
|  |  |  |  |

<Circumstances, explanations, exceptions, competing accounts. Search coverage: where was looked, over which period, with what result.>

## A · Actions or omissions

<Acts, decisions or omissions, with actor, role, time and source. For an omission: the expected action, and the basis for concluding it did not occur.>

## R · Observed outcome

<What was established afterwards, and on which evidence. Risk stated as risk. Causal link only where shown; otherwise "after".>

## C · Conformity assessment

<The comparison with the standard, its significance, mitigating or aggravating factors, counterevidence, and the conclusion on the degree of conformity, subject to [uncertainties]. For journalism: what can be reported, and how.>

### Uncertainties

<What remains unknown or unverified, each with a question id. What the assessment assumes, each with an ASM id.>

## Domain flow

<Keep only the part for this purpose. Write Not applicable: <reason> for the others.>

### Audit

- Objective, test performed, population and sample:
- Exceptions and limits of the test:
- Cause, if supported:

### Journalism

| Put to | What was put | When | Channel | Response status | Response source |
|---|---|---|---|---|---|
|  |  |  |  | pending · declined · no-response-by-cutoff (date) · outreach-forgone (reason) · responded | source.<slug> |

- Prior notification:
- How the response changed the account:
- Public-interest and disclosure judgement:

### Legal

| Element | Supported · disputed · unresolved | Evidence | Counterargument |
|---|---|---|---|
|  |  |  |  |

## Follow-up

<Kept apart from the assessment. Audit: recommendation, management response, owner, due date, evidence of completion. Legal: proposed remedy or filing. Journalism and all releases: decision id.>

## Checks

<Which quality checks from OSCARC.md ran, with results, and which did not.>
