# Candidate — Resolve before deferring

- **Candidate ID:** OGM-20261121-01
- **Date / timezone:** 2026-11-21 / America/Chicago
- **Status:** Candidate proposed for human review; **not** adopted, validated, or merged
- **Source type:** Organic collaboration correction, reported in the current discussion and abstracted for a public repository; supporting proposal is a reasoning hypothesis, not independent empirical evidence
- **Related foundations:** P-03 (human agency), P-06 (honesty and boundaries), P-07 (useful human outcomes); also P-05 (learning from correction)
- **Adjacent, still-unmerged proposals:** [PR #4 — purpose-aware initiative](https://github.com/uclacastillo/Og-mat/pull/4) and [PR #7 — cumulative evidence reconciliation](https://github.com/uclacastillo/Og-mat/pull/7)
- **Disposition:** Preserve **one** tentative candidate and its supporting observations; do not make additional standalone principles, edit `SEED.md`, or schedule a new recurring experiment

## Candidate claim

> **Resolve before deferring.** When an assistant can reasonably resolve a meaningful uncertainty itself, it should do so rather than transfer avoidable verification work to the human through guessing, unnecessary hedging, or requests for confirmation. Reserve human attention for genuinely unresolved questions, user-specific information, authority, values, and judgment.

This is **not** an instruction to verify every statement or to conceal uncertainty. The appropriate response depends on stakes, probability and cost of error, quality and availability of verification, time, and the person's goal. When reliable verification is unavailable or disproportionate, disclose the limitation plainly and still provide useful, appropriately scoped work.

## Observed problem and supporting observations

A collaborator reported an ordinary conversational attribution mistake: an assistant gave an incorrect answer to a question that reportedly had an inexpensive, available way to check. The person had to catch or correct the error. The reported episode was **not independently audited** for this record, and no quantified cost or baseline comparison is available.

This prompted a distinction among three possible behaviors:

1. **Unsupported confident guess:** can externalize error detection and correction to the human.
2. **Unresolved hedge when a check is feasible:** can be more honest yet still externalize avoidable checking effort.
3. **Proportionate verification before responding:** may protect both accuracy and the person's attention, when the check has sufficient expected value.

A second, related observation was that a retained correction only earns its value if it changes behavior on a relevant future task. Disclosing a prior mistake at the point of use can help, but disclosure is not a substitute for applying the lesson. Whether a future assistant can retain that lesson depends on authorized memory or accessible context; no persistent memory is assumed.

These are **supporting observations**, not independent proof of the proposed rule's efficacy. The key potential discovery is that an assistant might be candid about its uncertainty while still imposing unnecessary effort on the human.

## Why this might add something beyond existing OG-MAT

The current [SEED](../../SEED.md) already instructs the assistant to distinguish known, inferred, and unknown; verify consequential or changing facts when tools allow; and make useful progress. [INTEGRITY](../../INTEGRITY.md) similarly discourages unsupported answers hidden behind hedges. An execution lapse could fully explain the reported mistake.

The candidate asks whether OG-MAT should make **avoidable verification burden on the human** more explicit as an operational consideration, rather than treating honest disclosure as an adequate endpoint. It sharpens the relationship between truthful uncertainty (P-06) and useful outcomes (P-07), while reserving human judgment and authority (P-03).

This may already be adequately addressed by [PR #4](https://github.com/uclacastillo/Og-mat/pull/4), which considers the net benefit, effort, reversibility, and authority of an assistant's initiative. [PR #7](https://github.com/uclacastillo/Og-mat/pull/7) separately concerns how lessons are noticed and reconciled. **Do not duplicate or pre-approve either pending proposal.** If the narrower candidate contributes no distinct benefit, attach the observation to PR #4 or close it as redundant.

## What this record does *not* advance

The originating discussion contained five candidate formulations. This record does not separately propose a universal claim-labeling system, mandatory multi-model checking, a requirement to disclose every historical miss, or replacement of accuracy and agency measures with a single human-cost score. These may be techniques or evaluation dimensions in some contexts, but were not established as additional principles by the observed episode.

## Failure modes and constraints

- **Overchecking:** tool calls, second opinions, and searches can add delay, noise, cost, privacy exposure, or new errors without improving the answer.
- **False verification:** finding a plausible source or receiving model agreement does not establish that the claim is true; checks should have relevant quality and independence.
- **Incorrectly withholding human involvement:** the person's own facts, values, consent, and consequential decisions cannot be resolved solely by AI confidence or consensus.
- **Illusory improvement:** verbal assurances, citations, or prior-error disclosures can look responsible while behavior remains unchanged.
- **Generalizing one preference:** some people deliberately want to inspect evidence to learn, exercise oversight, or develop their own judgment. The aim is to remove *avoidable* burden, not meaningful participation.
- **Unmeasured errors:** an assistant cannot reliably audit mistakes it did not detect, so self-recorded corrections alone cannot establish efficacy.
- **Unsupported continuity:** no cross-session lesson persistence should be claimed without actual authorized mechanisms.

## Plausible alternatives

1. **No new principle needed:** existing SEED/INTEGRITY guidance is sufficient; the attribution failure is merely incomplete execution.
2. **A narrower example suffices:** add an example under the existing Verify step, but only if observations justify touching the portable seed.
3. **Purpose-aware initiative subsumes it:** document the observation under pending PR #4 rather than retaining a separate candidate.
4. **Verification is not the bottleneck:** conversational errors might more often arise from lack of tools, poor retrieval quality, or failure to recognize when facts are uncertain.

A useful review should compare these alternatives instead of assuming a new rule is warranted.

## Low-burden way to reassess

If similar situations naturally arise, observe a small set of **matched, non-sensitive tasks where a credible inexpensive check is available**. Compare current OG-MAT behavior with a minimal `resolve before deferring` instruction, keeping tool access and conditions comparable. Assess:

- Did the response avoid an incorrect or unnecessarily deferred answer?
- Was the check actually performed and capable of resolving the claim?
- Did it reduce subsequent human corrections or requests for substantiation?
- Did it add delay, irrelevant checking, or false confidence?
- Did it preserve meaningful human authority and useful progress?

Use independently checkable outcomes where feasible, including occasional independent review of outputs; do **not** ask the human to maintain or inspect a per-claim ledger. Distinguish observed corrections from unknown undetected errors. Informal observations are suitable for refining the hypothesis, not proving a universal effect.

**Falsifier / reason to fold into existing guidance:** If a matched comparison shows no reduction in consequential mistakes or needless deferral, or the extra verification creates equal or greater burden, do not add the instruction to the seed. Also fold the candidate into PR #4 if its effect is indistinguishable from existing purpose-aware initiative guidance.

## Approval and lineage

The human requested that this observation be **captured as a candidate**, not that OG-MAT's portable seed be rewritten. This record is a reviewable proposal only. Any future seed or map policy revision requires a separate justification and human approval. Public provenance is deliberately abstracted; no private dialogue or identifying details of the reported episode are reproduced.
