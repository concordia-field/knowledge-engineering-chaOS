# Lexicon

The one vocabulary of this repository. Every value an agent writes into a field comes from here. To add a word, write a decision record; do not add it in passing.

## How words are weighted

Words carry weight the way relations do in chaOS: by evidence. Each term's weight is a step on the seed's rhythm (13, 8, 5, 3, 2, 1). Two counts are its evidence:

- **KE**: occurrences across the knowledge-engineering method (documents, schemas, scripts);
- **OS**: occurrences in the OSCARC guide as supplied.

Counted 2026-11-21, case-insensitive, by word stem. The knowledge-engineering folder was changing while it was counted, so KE counts are a snapshot. Counts guide the weight; they do not decide it alone. Where judgement overrode a count, the note says why.

A **bridge** term (marked ⇄) weighs on both sides. Bridges are where this repository is more than either of its parents: they let a finding be composed from the same records a knowledge base is built from.

Words that name a virtue are not here; words that make it checkable are. "Transparency" and "sovereignty" occur in neither source. What both repeat instead are *evidence*, *source*, *decision* and *review*: the means by which a reader checks for themselves.

### 13 · the spine

| Term | KE | OS | Meaning |
|---|---|---|---|
| **OSCARC** | – | – | Objective finding, Standard, Chronology and context, Actions or omissions, Observed outcome (R), Conformity assessment. The method this repository is built around: [OSCARC.md](OSCARC.md). |
| **finding** ⇄ | 9 | 21 | One condition established within the evidence reviewed, assessed against a standard for a purpose. |
| **evidence** ⇄ | 97 | 21 | Ids that resolve, cited separately for each step that needs support. |
| **source** ⇄ | 518 | 4 | Where a statement comes from; itself a node, cited by id, role and exact locator. |
| **status** | 207 | 2 | What kind of truth a statement holds. |
| **kind of truth** | 17 | 0 | The question every page answers at a glance. Weighted for purpose, not frequency. |

### 8 · load-bearing

| Term | KE | OS | Meaning |
|---|---|---|---|
| **standard** ⇄ | 5 | 10 | The criterion a finding is compared with: legal basis, rule, agreement, procedure or control. Also called **criterion**. |
| **observed outcome** ⇄ | 9 | 12 | The condition or result established afterwards (R). |
| **conformity assessment** | 0 | 17 | The reasoned comparison with the standard, with its degree and its open questions. Counts *assessment* and *conformity* together. |
| **decision** ⇄ | 117 | 8 | A choice reserved to a human, recorded with options, owner and date. |
| **review** ⇄ | 192 | 6 | A recorded human judgement, naming reviewer, authority and decision. |
| **relation** | 265 | 0 | A typed, directed, forward-only edge between ids. |
| **contract** | 189 | 0 | The rules a record must meet: [CONTRACT.md](CONTRACT.md). |
| **maturity** | 119 | 0 | How developed a page is, from `seed` to `canonical`. |
| **assumption** | 48 | 0 | A proposition relied on but not established; recorded as an `ASM-<nnn>` row, never left silent. Raised from 3 by judgement, not count: the maintainer's first principle is that assumptions are the mother of all fuck-ups. |

### 5 · working

| Term | KE | OS | Meaning |
|---|---|---|---|
| **action or omission** ⇄ | 4 | 9 | What an actor did, decided, or did not do (A). An omission needs the expected action and evidence it did not occur. |
| **response** | 0 | 14 | What a party said when asked. Always attributed; itself a source. |
| **chronology** | 0 | 8 | The sequence of events with dates and their precision (C). |
| **attributed** ⇄ | 35 | 6 | Preserved as a named source said it; not asserted by this repository. Raised from 3 for OSCARC's reliance on it. |
| **purpose** | 29 | 1 | Why the assessment is made: `audit`, `journalism` or `legal`. Weighted for its role in keeping assessments apart. |
| **scope** ⇄ | 69 | 3 | What was reviewed, and where a statement holds. |
| **claim** | 104 | 1 | A statement precise enough to be true or false. |
| **observation** | 118 | 3 | One atomic, not-yet-understood observation with a claim boundary. |
| **audit** ⇄ | 70 | 3 | A blameless, append-only record of review; also one of the three purposes. |
| **absence** | 50 | 0 | A written value for what is missing. |
| **authority** | 60 | 0 | The right to decide, held by a named human. |

### 3 · guards

| Term | KE | OS | Meaning |
|---|---|---|---|
| **uncertainty** ⇄ | 8 | 4 | What remains unknown after the assessment, each with a question. |
| **causal link** | 0 | 4 | Wording reserved for what the evidence shows; otherwise write "after". |
| **register** ⇄ | 181 | 3 | A table where every row gets a decision: here, the findings register. Weighted down: the KE extraction register is not used here. |
| **provenance** | 36 | 0 | The chain from a statement back to its source. |
| **preserve, then normalise** | 43 | 1 | Keep the source's wording beside your own, with the reason. |
| **claim boundary** | 10 | 0 | What an observation does not establish. |
| **weakest honest status** | 8 | 0 | The default when choosing a status. |
| **blocked** | 28 | 0 | A source that cannot be read. Work stops; nothing is written from memory. |
| **batch** | 73 | 0 | Three to five records made and audited together. |
| **drift** | 19 | 0 | Two lists, specs or meanings diverging. |
| **steward** | 32 | 0 | One who cares for the repository's health, not its growth. |

### 2 · edges

| Term | KE | OS | Meaning |
|---|---|---|---|
| **notification** | 0 | 4 | A prior report or communication about the finding. |
| **request for response** | 0 | 2 | Journalistic outreach about the finding. |
| **search coverage** ⇄ | 9 | 2 | Where was looked, over which period. A missing record is a search result, not a fact. |
| **locator** ⇄ | 19 | 1 | The exact place in a source: clause, page, timestamp. |
| **lens** ⇄ | 15 | 2 | The perspective that shapes an interpretation; named when it matters. |
| **audience** ⇄ | 18 | 3 | Who will read the output. |
| **follow-up** ⇄ | 8 | 3 | Recommendations, remedies, management responses: kept apart from the assessment. |
| **independent** | 21 | 0 | A second source that does not share the first one's origin. |
| **dictionary** | 45 | 0 | One sentence per shared term, before it earns a node. |
| **misunderstanding** | 12 | 0 | What the agent got wrong; every one becomes a guardrail. |
| **stop the line** | 3 | 0 | Pause and repair the process. Rare in text, decisive in practice. |

### 1 · named once

**inbox** (raw, never cited) · **derived** (generated, never hand-edited) · **reservation** (a link to a record not yet written) · **proof run** (the first batch, chosen to break the contract) · **portal** (a pointer to a better source).

## Values

### Status: what kind of truth

| Value | Meaning |
|---|---|
| `defined` | Fixes meaning by convention; neither true nor false. |
| `established` | Accepted within the stated scope and assumptions. |
| `conditional` | Holds only if named assumptions hold. |
| `open` | Neither established nor refuted. |
| `disputed` | Reliable sources disagree. |
| `refuted` | Shown false within the stated scope. |
| `experimental` | Supported mainly by measurement or exploration. |
| `heuristic` | Useful reasoning without the force of justification. |
| `interpretive` | A reading: historical, editorial, conceptual. |
| `attributed` | Preserved as a named source said it; not asserted here. |

### Conformity

`conforms` · `partly-conforms` · `departs` · `not-assessable` (the evidence does not allow a comparison; say why).

### Purpose

`audit` · `journalism` · `legal`.

### Response status

`pending` · `declined` · `no-response-by-cutoff` (with the cutoff date) · `outreach-forgone` (with the reason) · `responded`.

### Legal element

`supported` · `disputed` · `unresolved`.

### Assumption

`open` → `validated` (link the evidence) · `rejected` (link what changed as a result). A record resting on an `open` one is at most `conditional`.

### Question

`open` · `answered` (cite the source) · `unanswerable` (say why) · `withdrawn` (say why).

### Maturity

`seed` → `draft` → `structured` → `reviewed` → `canonical`. Meanings in [CONTRACT.md](CONTRACT.md#two-ladders).

### Growth

`dance` → `noticed` → `routine` → `governed` → `re-seed`. Thresholds in the chaOS seed's `src/growth.mjs`.

### Absence

`unknown` · `not-applicable` · `not-yet-verified` · `not-yet-developed` · `open` · `not-known` (nothing documented; not "none") · `not-in-source` (the source was read and does not say).

### Source access

`direct` · `indexed-full` · `indexed-partial` · `blocked`.

### Source role

`primary` · `criterion` (a standard, cited by exact clause and edition) · `response` (what a party said when asked) · `definition` · `reference` · `data` · `validation` · `justification` · `historical` · `synthesis` · `secondary`.

### Review

`reviewer_kind`: `human` · `agent`. `decision`: `approved` · `changes-requested` · `rejected`. Only `human` may approve.

### Observation

Workflow: `captured` → `screened` → `ready` → `promoted` · `merged` · `rejected` (kept as a negative result). Origin: `derived` · `measured` · `representation-induced` (the pattern comes from how it was represented) · `proposed`.

### Confidence (per relation)

`supported` · `provisional` · `unknown`.

### Decision and audit

Decision status: `proposed` · `accepted` · `superseded` · `rejected`. Audit outcome per record: `accepted` · `held-back` · `blocked`.

### Archetypes

Each project names its own types and maps each onto one archetype. A **finding** maps onto `claim`.

| Archetype | For |
|---|---|
| `entity` | A principal subject with comparable properties. |
| `concept` | An idea other nodes point to. |
| `claim` | A statement that can be true or false; includes findings. |
| `source` | A citable origin; includes criteria and responses. |
| `observation` | One observation with a claim boundary. |
| `experiment` | A reproducible investigation that says what it does not establish. |
| `example` | A concrete instance of another node. |
| `teaching` | A page for an audience; cannot raise the status of what it teaches. |
| `analogy` | A mapping between domains, with stated limits. |

### Bonds

Relation `type` values, by category. Use the most specific.

| Category | Bonds |
|---|---|
| dependency | `depends-on` · `requires` · `uses` · `derives-from` · `defined-by` · `precedes` · `supersedes` |
| equivalence | `equivalent-to` · `approximates` · `same-as` |
| representation | `expresses` · `models` · `exemplifies` · `teaches` |
| evidence | `supports` · `contradicts` · `proves` · `refutes` · `cites` · `attributed-to` · `does-not-establish` |
| assessment | `assessed-against` (finding → criterion) · `responds-to` (response → finding) · `follows-up` (recommendation or decision → finding) |
| habit | `follows` · `precedes-in-practice` · `replaces` (patterns learned from the journal) |
| association | `associated-with` (needs `scope`) · `related-to` (last resort) |
| analogy | `analogous-to` (needs `limits`; never evidence) |

The `habit` bonds describe what the person and agent *do*, learned from events. They never appear between knowledge records as if they were facts about the subject. No bond means "caused": causation is stated in the finding's prose, with its evidence.
