---
name: node
description: Create or revise one knowledge node with an explicit status, maturity, sources and absence values, written in five aspects. Use when asked to add, write, finish or correct a page for a named subject, or to promote a ready observation.
---

# One node

Contract: [CONTRACT.md](../../CONTRACT.md#node). Template: [node](../../templates/node.md).

1. **Smallest fitting record.** If a shared meaning is enough, write one sentence in `dictionary.md` instead.
2. **Capture first.** Every source this node will cite has been read via [capture](../capture/SKILL.md). Anything `blocked` stops here.
3. **Envelope.** `id: <type>.<slug>`, never to change. `status`: weakest honest. `maturity`: `seed` or `draft`.
4. **Five aspects.** Context, Description, Properties, Behaviour, Relations. `Not applicable: <reason>` where one does not apply. Never invent content to fill one.
5. **Keep four kinds of statement apart:** observed fact (with source and locator), source claim (`attributed`), interpretation (labelled), assumption (a row in `assumptions.md`, its id under `assumptions`).
6. **Preserve, then normalise.** Keep the source's form beside yours, with the reason they are equivalent.
7. **Sources** by id, role and locator. Facts that can be checked get two independent sources, or say they have one.
8. **Relations** via [relate](../relate/SKILL.md).
9. **Maturity.** You may raise it to `structured` when every field and aspect is present and every absence is written. Stop there: `reviewed` needs a recorded human review.
10. **Revision.** When the meaning changes, not the wording, say so in the report; claims made under the old meaning are rechecked.

## Report

Id, status, maturity, sources and their access, unresolved links, what a human must still decide.
