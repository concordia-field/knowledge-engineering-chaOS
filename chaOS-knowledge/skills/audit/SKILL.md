---
name: audit
description: Close a batch of three to five nodes, or a reflection, with a blameless append-only audit — check each node against the floor, compare across nodes, record what the agent misunderstood, and prepare (never take) contract decisions. Use when a batch or the first proof run is finished, when reflection is due, or when asked to review recent work.
---

# Audit

Contract: [CONTRACT.md](../../CONTRACT.md). Template: [audit](../../templates/audit.md).

1. **Scope.** List the nodes in the batch and why each was chosen. The first batch, the proof run, should include the awkward cases.
2. **Floor, per node.** Source read in full; nothing written from memory; nothing dropped from the capture list; weakest honest status; scope stated; attributions intact; no upgraded bonds; absences written; reads well without the frontmatter.
3. **Across nodes.** Compare with at least two earlier nodes: structure, voice, naming, how sources are cited.
4. **Journal.** If reflection is due, run `spiral review` and look at repeats. Record new habit relations via [relate](../relate/SKILL.md).
5. **Assumptions.** Walk the open rows in `assumptions.md`. Validate or reject what the batch made checkable; recheck every record that used a rejected one.
6. **What did the agent misunderstand?** Write it plainly. Each answer becomes a rule in the project's `AGENTS.md`.
7. **Decisions.** Contract or lexicon changes are *proposed* in a decision record from the [decision](../../templates/decision.md) template, for a human to accept. Changes happen only between batches.
8. **Close.** Run `spiral reflected` if this was a reflection. The audit is append-only: follow-ups are added, history is not rewritten.

## Report

Nodes accepted and held back (with reasons), checks run and not run, misunderstandings, decisions awaiting a human.
