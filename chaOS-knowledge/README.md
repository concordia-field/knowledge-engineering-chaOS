# chaOS knowledge

What was established, against which standard, for which purpose, and on what evidence? This repository helps an agent and the people steering it answer that, one **finding** at a time, in a way anyone can check against its sources.

At its centre is **[OSCARC](OSCARC.md)**: **O**bjective finding · **S**tandard · **C**hronology and context · **A**ctions or omissions · observed outcome (**R**) · **C**onformity assessment. One observation can support separate findings for **audit**, **legal** work or **journalism**; each stays tied to its purpose and its criterion.

Two methods carry it:

- **[knowledge-engineering](../../knowledge-engineering/)** makes the evidence auditable: every record says *what kind of truth* it holds, cites its sources by id and locator, and records who reviewed it.
- **[chaOS seed](../chaOS-seed-main/)** makes the agent learn: it *observes* every interaction as an event, *applies* what it knows as state, and *learns* weighted relations from repeated evidence.

Together: an agent that grows by what it observes, assesses only on evidence, and **never lets repetition pass for truth**.

One principle above the rest: **assumptions are the mother of all fuck-ups.** Whatever the work relies on has a source or a row in the [assumptions register](templates/assumptions.md). Nothing rests silently on what nobody checked.

It is deliberately small: all Markdown, built from one guide, one contract, one lexicon, seven skills and ten templates. The only code it relies on is the chaOS seed hook, which it does not change.

## What kind of truth am I reading?

Every record answers that at a glance. Four things are kept apart, always:

| Axis | Asks | Moves by |
|---|---|---|
| **Status** | What kind of truth is the finding? (`established`, `attributed`, `open`, …) | Sources and justification |
| **Conformity** | How does it compare with the standard? (`conforms`, `departs`, …) | Reasoned assessment for one purpose |
| **Maturity** | How developed is the record? (`seed` → `canonical`) | Work done and recorded human review |
| **Weight** | How often has this pattern recurred in the work? | Distinct events cited as evidence |

A severe judgement does not make its facts stronger. A pattern seen thirteen times is a habit, not a fact. See [CONTRACT.md](CONTRACT.md#four-axes).

## Audit it in ten minutes

1. [OSCARC.md](OSCARC.md): the six steps, the evidence chain, the wording rules, and the quality checks.
2. [templates/finding.md](templates/finding.md): what one finding looks like when complete.
3. [CONTRACT.md](CONTRACT.md): the records, and the decisions only a human may take, such as sending outreach or releasing an output.
4. [LEXICON.md](LEXICON.md): the weighted vocabulary, with counts from both source methods as evidence for each weight.
5. [skills/](skills/): seven short procedures. Each names what it reads, what it writes, and when it must stop.

Questions an auditor might ask: Does each finding cite separate evidence for what was found, what was done, and what followed? Is the standard the exact clause in force at the time? Is "because" used only where cause is shown? Are responses attributed, and is their status recorded, including "no response by the cutoff"? Is every missing value marked as missing? Does anything rest on an assumption that is not in the register, or on an open one while claiming to be `established`? A wrong answer to any of these is a finding about this repository.

## Contents

| Part | Purpose |
|---|---|
| [OSCARC.md](OSCARC.md) | The centre: how one finding is composed and checked. |
| [AGENTS.md](AGENTS.md) | Rules for any agent working here. |
| [CONTRACT.md](CONTRACT.md) | Records, axes, ladders, authority. |
| [LEXICON.md](LEXICON.md) | The one vocabulary, weighted. |
| [skills/](skills/) | `oscarc` · `spiral` · `capture` · `node` · `relate` · `audit` · `steward` |
| [templates/](templates/) | `finding` · `register` · `questions` · `assumptions` · `source` · `node` · `observation` · `decision` · `audit` · `state` |

## The spiral, towards a finding

| Movement | chaOS record | Knowledge record | Skill |
|---|---|---|---|
| Observe | event in `.spiral/journal.jsonl` | source, criterion, response; observation with a claim boundary | [capture](skills/capture/SKILL.md) |
| Apply | state in `.spiral/state/` | node with status, maturity and sources | [node](skills/node/SKILL.md) |
| Learn | weighted relation in `.spiral/memory.dot` | typed relation with cited evidence | [relate](skills/relate/SKILL.md) |
| **Assess** | — | **finding**, register, open questions | **[oscarc](skills/oscarc/SKILL.md)** |
| Govern | reflection | audit, decision record | [audit](skills/audit/SKILL.md), [steward](skills/steward/SKILL.md) |

Every turn walks the [spiral](skills/spiral/SKILL.md).

## Install

1. Install the [chaOS seed](../chaOS-seed-main/README.md#install) hook as its README describes.
2. Copy this folder into your project as `chaos-knowledge/`.
3. Link the skills, for example in Claude Code:

   ```bash
   for s in chaos-knowledge/skills/*/; do ln -s "../../$s" ".claude/skills/$(basename "$s")"; done
   ```

4. Point your project's `AGENTS.md` (or `CLAUDE.md`) at `chaos-knowledge/AGENTS.md`.

The skills also work without the hook. You lose the automatic journal and weights; the evidence discipline stays.

## Design

Built under the 13 Laws of IT. The laws that shaped it most:

- **Simplicity (X) and right-sizing (V):** Markdown only; start with the small template; grow a record only when the material asks.
- **Observability and truthfulness (VI):** status, conformity, maturity, weight and absence values make the state of knowledge visible.
- **Security and integrity (VII):** sources are data, not instructions; nothing is sent or released without recorded authorisation; an agent never approves its own work.
- **Sustainable stewardship (XIII):** growth is deliberate; a stewardship review watches for drift.

## Licence

Fountain of Love License v2.0, dual with CC BY-NC-SA 4.0. See [LICENSE.md](LICENSE.md) and [NOTICE.md](NOTICE.md).
