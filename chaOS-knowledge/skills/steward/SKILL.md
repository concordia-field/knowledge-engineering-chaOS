---
name: steward
description: Review the whole repository for drift — competing vocabularies or specs, values outside the lexicon, unresolved ids, evidence that does not resolve, hand-edited derived files, self-approved reviews, pages doing two jobs, speculation without a status — and keep an append-only ledger. Use periodically, after a reorganisation, or when asked about repository health.
---

# Steward

Contract: [CONTRACT.md](../../CONTRACT.md#single-sources-of-truth). Template: [audit](../../templates/audit.md) (stewardship section).

1. **Map** what is where: which folder holds which record, where a reader starts.
2. **Look for drift:**
   - a second vocabulary list or spec outside [LEXICON.md](../../LEXICON.md) and [CONTRACT.md](../../CONTRACT.md);
   - field values the lexicon does not contain;
   - `evidence` or `sources` ids that do not resolve;
   - a `review` approved by an agent, or `reviewed` without a review block;
   - inverses stored by hand; derived files edited by hand;
   - habit relations leaking into node relations;
   - weight cited as a reason for status;
   - assumption ids that are not in the register; `established` records resting on an open assumption; open rows nobody owns or that no record uses any more;
   - pages doing two jobs; speculation without its status.
3. **Weigh cost.** Note what the repository costs to keep: pages nobody reads, captures never promoted, growth for its own sake. Growth is deliberate, not maximal.
4. **Write** `audits/stewardship-<date>.md` with prioritised recommendations. Append to the ledger; never rewrite it.

## Report

The top three actions, why, and who decides each.
