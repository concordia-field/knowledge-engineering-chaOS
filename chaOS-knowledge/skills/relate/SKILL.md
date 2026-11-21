---
name: relate
description: Record what connects, with evidence. Add typed, forward-only relations between nodes citing source ids, and weighted habit relations in spiral memory citing event ids. Use when connecting nodes, when a pattern in the work repeats, or when the hook or a reflection surfaces a repeat.
---

# Relate

Contract: [CONTRACT.md](../../CONTRACT.md#relation). Bonds: [LEXICON.md](../../LEXICON.md#bonds).

Two kinds of relation, never mixed.

| | About the subject | About the work |
|---|---|---|
| Lives in | node `relations` | `.spiral/memory.dot` |
| Evidence | source ids (`source.…`) | event ids (`e-…`) |
| Bonds | dependency, equivalence, representation, evidence, association, analogy | habit |
| Weight means | how much independent support | how often it recurred |

## Between nodes

1. Use the **most specific** bond. `related-to` is a last resort and should be rare.
2. **No upgrades.** Support is not proof unless the bond is `proves`. Association is not cause. Analogy is never evidence and always carries `limits`.
3. Qualify what is conditional: `scope`, `condition`, `confidence` (`supported`, `provisional`, `unknown`).
4. Forward only. Write each fact once; inverses are computed.
5. A target that does not exist yet is a reservation: allowed before `reviewed`, an error after.

## In spiral memory

1. Only from events you can cite: `spiral remember "<from>" <bond> "<to>" --evidence e-…,e-…`.
2. Weight is the number of distinct events. Do not cite the same event twice to inflate it.
3. **Repetition is a verdict.** When unsure whether two events show the same pattern, ask.
4. A habit relation describes what people do, not what is true. It never crosses into node `relations`.

## Report

Relations added (from, bond, to, evidence), reservations left open, and any bond you wanted but the lexicon lacks (proposed, not added).
