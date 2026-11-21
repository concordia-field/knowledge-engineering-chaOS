# knowledge-engineering chaOS

What was established, against which standard, for which purpose, and on what evidence?

This repository helps an AI agent, and the people steering it, answer that one **finding** at a time, in a way anyone can check against the sources. It joins a method for evidence-backed findings (**OSCARC**) to a method for auditable knowledge (**knowledge-engineering**) and an agent that learns from its own work (**chaOS**).

It is small by design. It is almost entirely Markdown, so it can be read and audited without running anything.

## What is here

| Folder | What it is | Start with |
|---|---|---|
| [chaOS-knowledge/](chaOS-knowledge/) | The opinionated variant: OSCARC at the centre, one contract, one weighted lexicon, seven skills, ten templates. | [README](chaOS-knowledge/README.md) |
| [chaOS-seed-main/](chaOS-seed-main/) | The chaOS seed: a tiny hook that journals every prompt and reply, keeps state, and learns weighted relations. chaOS-knowledge uses it unchanged. | [README](chaOS-seed-main/README.md) |

## Four principles

1. **Assumptions are the mother of all fuck-ups.** Whatever the work relies on has a source or a row in the [assumptions register](chaOS-knowledge/templates/assumptions.md). Anything resting on an open assumption is at most `conditional`.
2. **Every record says what kind of truth it holds.** How solid the facts are (`status`), how they compare with a standard (`conformity`), how developed the page is (`maturity`) and how often a pattern recurred (`weight`) are kept apart.
3. **Repetition earns structure, never truth.** The agent may turn a recurring pattern into a routine; it may not turn it into a fact.
4. **The agent prepares; a person decides.** Approving a review, sending outreach and releasing an output each need a recorded human decision.

## For an auditor or journalist

Read these five, in order, in about ten minutes:

1. [OSCARC.md](chaOS-knowledge/OSCARC.md): the six steps of a finding and the quality checks.
2. [templates/finding.md](chaOS-knowledge/templates/finding.md): one finding when complete.
3. [CONTRACT.md](chaOS-knowledge/CONTRACT.md): the records, and what only a human may decide.
4. [LEXICON.md](chaOS-knowledge/LEXICON.md): the vocabulary, each word weighted with its evidence.
5. [AGENTS.md](chaOS-knowledge/AGENTS.md): the rules an agent must follow.

## To use it

Install the [chaOS seed hook](chaOS-seed-main/README.md#install), copy `chaOS-knowledge/` into your project and link its skills. The steps are in [chaOS-knowledge/README.md](chaOS-knowledge/README.md#install). The skills also work without the hook.

## Lineage

Both parts derive from the Fountain of Love operating model. chaOS-knowledge also draws on the knowledge-engineering method and on OSCARC, adapted into English from a Dutch source supplied by the maintainer. See [chaOS-knowledge/NOTICE.md](chaOS-knowledge/NOTICE.md).

## Licence

Fountain of Love License v2.0, dual with CC BY-NC-SA 4.0. See [LICENSE.md](LICENSE.md).
