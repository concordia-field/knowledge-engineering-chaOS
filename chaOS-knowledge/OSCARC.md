# OSCARC

The centre of this repository. Everything else (sources, nodes, relations, audits) exists so that one **finding** can be composed from evidence and checked by someone else.

OSCARC composes one evidence-backed finding from the records. The same observation can support separate assessments for **audit**, **legal** work or **journalism**. Each assessment stays tied to its **purpose** and its **criterion**.

This English guide adapts an OSCARC source supplied by the maintainer, which was written in Dutch. See [Origin of terms](#origin-of-terms).

## The six steps

| Step | Term | Meaning |
|---|---|---|
| **O** | Objective finding | The condition established within the evidence reviewed. Attribute an account or allegation to its source when that is what the evidence establishes. |
| **S** | Standard | The applicable legal basis, rule, agreement, procedure, control or other stated criterion, and what it required or led one to expect. |
| **C** | Chronology and context | The sequence of events, relevant circumstances, explanations, exceptions and competing accounts. |
| **A** | Actions or omissions | The acts, decisions or supported failures to act, with the actor, role and time. |
| **R** | Observed outcome | The condition or result established afterwards. State potential risk as risk, and a causal effect only where it is shown. |
| **C** | Conformity assessment | The reasoned comparison with the standard: the degree of conformity and the questions left open. Where the task calls for an editorial assessment, say what can be reported and how. |

### Evidence chain

```text
objective finding → evidence → standard → chronology and context
  → action or omission → evidence → observed outcome → evidence
  → conformity assessment → uncertainties
```

Each arrow marked *evidence* is a separate citation. The finding, the action or omission, and the outcome are each supported on their own; one document does not silently carry all three.

## How OSCARC sits on the records

| OSCARC | Record here | Rule from the [contract](CONTRACT.md) |
|---|---|---|
| Evidence | [source](templates/source.md) node, cited by id and exact locator | Sources are nodes. Read in full first. |
| Standard | a source node with role `criterion`, its exact clause as locator, its edition as `version` | Standards are sources too. |
| Reported account, allegation | content with status `attributed` | Attributed, never asserted. |
| Response to outreach | a source node with role `response` | A response is a source: attributed, and checked. |
| Raw material, early signals | [observation](templates/observation.md) with a claim boundary | One observation per node. |
| Open gap | a row in [questions](templates/questions.md) | Every material gap gets a question. |
| Something relied on but not established | a row in [assumptions](templates/assumptions.md) | No silent assumptions. An open one caps the finding at `conditional`. |
| The finding itself | [finding](templates/finding.md) | Status of O and the conformity judgement are kept apart. |
| Several findings | [register](templates/register.md) | One row per finding; expand a row into a finding when it needs room. |
| Outreach sent, output released | [decision](templates/decision.md) | Only on explicit human authorisation. |

**The finding's `status` and its `conformity` are separate.** `status` says what kind of truth the objective finding is (`established`, `attributed`, `open`, …). `conformity` says how the conduct or condition compares with the standard. A strong judgement never raises the status of the facts it rests on.

## Wording rules

- Fill the template for **one** finding.
- Write `unknown`, `not-yet-verified` or `Not applicable: <reason>` where a part is missing. Never leave it blank.
- Compare only the condition or conduct that the standard **actually governs**.
- Write **"after"** when only the timing is established. Use causal wording only when the evidence supports the causal link.
- A missing entry is a **search result within the reviewed scope**: "no record was found in X for period Y", not "it did not happen".
- To call something an **omission**, establish the expected action *and* the evidence for concluding it did not occur.
- Risk is stated as risk; it is not an outcome.

## Small template

For one straightforward finding. Full record: [templates/finding.md](templates/finding.md).

> On [date] at [place], it was established that [objective fact or condition]. This finding is supported by [source id and locator, or attributed statement].
>
> Under [criterion: legal basis, standard, agreement or procedure, with edition], [required condition or expected conduct] was required or expected.
>
> The chronology shows [sequence of relevant events]. During [date or period], [person or party, and role] took [actions or decisions] or omitted [required action], as supported by [source ids].
>
> After these events, [observed outcome or demonstrated consequence] was established on the basis of [source ids]. This outcome [meets or departs from] what could be expected under the standard.
>
> The assessment takes into account [circumstances, explanations, mitigating or aggravating factors, counterarguments].
>
> On that basis, [nuanced conclusion about the degree of conformity], subject to [uncertainties or missing evidence].

## Domain flows

The six steps are common. What comes before and after them depends on the purpose.

### Audit

**Objective finding → standard → chronology and context → action or omission → observed outcome → conformity judgement**, then **recommendation → management response or action plan → follow-up**.

- Record the audit objective, the test performed, population and sample where relevant, exceptions, and the limits on what the test establishes.
- Compare observed and expected conditions, and explain the finding's significance.
- Record cause when it is supported.
- Link each agreed action to its owner, due date and evidence of completion.
- Recommendations and management commitments are **follow-up** to the finding, never part of it.

### Journalism

**Documented finding or attributed allegation → initial evidence check → notification or request for response → attributed response → verification of the accounts → reporting and, where appropriate, labelled commentary.**

- Record what was put to whom, when, and through which channel, with the date and status of any response.
- Distinguish: a request still `pending`; a `declined` response; `no-response-by-cutoff` (with the cutoff); and `outreach-forgone` (with the reason).
- Link any prior **notification** if it matters to the story.
- Check the material statements in the response, and record how they changed the account.
- Record the **lens**, the **audience** and the working draft on the finding.
- Record the public-interest and disclosure judgement for sensitive material.
- Where the story assesses conduct against a specific standard, name it and explain how it applies.

### Legal

**Objective finding → legal or procedural standard → chronology and context → action or omission → observed outcome → conformity assessment.**

- Record the exact provision or clause, its relevant version, and why it applies.
- Link evidence separately for the finding, the action or omission, and the outcome.
- Address exceptions, notices, responses and counterarguments where they affect the assessment.
- State which elements are `supported`, `disputed` or `unresolved`.
- A proposed remedy or filing decision belongs to the follow-up, not the finding.

## Three sizes

| Size | Use when | Record |
|---|---|---|
| Small | One straightforward finding | The [small template](#small-template), inside a [finding](templates/finding.md) |
| Medium | Several findings | A [register](templates/register.md), one row each |
| Large | One finding whose evidence, chronology or reasoning needs room | A [finding](templates/finding.md) with every section filled in detail |

Start small. Grow a row into a large record only when the material asks for it.

## Quality checks

Run these before a finding leaves `draft`, and record which were run.

1. Every step cites ids that resolve, with exact locators. Finding, action or omission, and outcome have **separate** support.
2. The criterion is the exact clause and edition, and it governs the conduct being compared.
3. The chronology is consistent across sources. Dates carry their precision.
4. Search coverage is stated: where was looked, over which period.
5. Sources that share an origin are not counted as independent.
6. Contrary evidence and competing accounts are addressed, not omitted.
7. "After" and causal wording match what the evidence shows.
8. Every omission names the expected action and the basis for concluding it did not occur.
9. Quotes keep their qualifiers; representation, citation and disclosure context are checked against the source.
10. Attributed accounts and responses stay attributed.
11. Each material gap has an open question. Each proposition relied on but not established has an assumption row, and the finding lists its id.
12. Recommendations, remedies and release decisions sit outside the assessment.

## Origin of terms

The source used Dutch terms. Here, *vaststelling* is the **finding** at step O and *resultante* is the **observed outcome** at step R. **Notification** is a prior report or communication about the finding; a **request for response** is journalistic outreach about it; the **response** that results is always attributed.
