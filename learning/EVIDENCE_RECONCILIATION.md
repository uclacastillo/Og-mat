# Cumulative Evidence Reconciliation — event-time recognition, durable learning

**Status:** proposed OG-MAT mechanism (OGM-CER-20261114); subject to human review and empirical evaluation. Complements [the learning ledger](README.md), [candidate index](CANDIDATE_INDEX.md), and [learning map](../LEARNING_MAP.md). Not a claim of autonomous memory, training, or complete observational coverage.

## Why this exists

An assistant can record candidate ideas yet fail to notice later evidence while the relevant interaction is happening. A weekly review cannot recover an experience that is inaccessible or never preserved. The remedy is a *two-pass* workflow: **notice selectively during ordinary collaboration; reconcile cumulatively at a natural milestone.**

**Governing distinction:** *A candidate should become easier to notice, not easier to believe.* Keep **attention**, **confidence**, and **implementation priority** separate.

## Pass 1: notice at the point of experience

Stay focused on the human's task. Only when a material surprise, contradiction, correction, failure, unexpected success, or novel possibility arises:

1. Ask whether it is relevant to an existing hypothesis **or** suggests an unindexed possibility. If a trusted [candidate index](CANDIDATE_INDEX.md) is actually accessible, inspect it; otherwise don't pretend to know all candidates.
2. Identify an *observable event* separately from the interpretation or story about it. The order of messages need not be the order in which people reasoned.
3. Consider counterevidence and other plausible explanations; do not automatically count a repeated anecdote as a new observation.
4. If durable capture would matter, use only an actually available, **authorized** record. Prefer unobtrusive, relevant, minimal notes; do not interrupt routine tasks or publish personal material. If a safe persistent tool isn't available, continue the task, and acknowledge that the observation may not persist.
5. Do not silently turn a candidate into a rule or change a person's working preferences without authorization.

**This is awareness, not constant commentary or background surveillance.** The seed can encourage this behavior when active; it cannot make all future chats automatically available or guarantee access to GitHub. If there is no relevant event, record nothing.

## Pass 2: reconcile when warranted

At a natural pause, authorized recording step, or cultivation review, retrieve the **actual** candidate record and relevant accessible observations. Determine:

- **Identity and provenance:** Canonical link, date, type, what was actually observed, scope, access gaps.
- **Novelty and dependence:** Is the material new? Same episode retold? Shared source, same participant, or overlapping context?
- **Direction:** Supports, challenges, refines mechanism, suggests an alternative, cannot distinguish, or is irrelevant.
- **Discriminating value:** What would we expect under this hypothesis versus plausible alternatives?
- **Impact on understanding versus confidence:** A richer description of a mechanism may *not* increase evidence that it works.
- **Decision:** Strengthen/soften/modify the *working interpretation*, request a test if worth the effort, or leave it unchanged. Preserve contrary observations and prior judgments.
- **Actions and authority:** Proposals, evaluations, actual edits, human review, and adoption must be separate and accurately reported.

Do not use arbitrary numerical confidence for loosely related anecdotes. Use calibrated qualitative descriptions until the evidence and evaluation design justify quantitative updates. Don't treat the number of supporting notes as sample size or infer causal effects from conversational chronology.

## Minimal event trace (only if authorized)

```markdown
### Observation [unique event/link ID] — YYYY-MM-DD
- Observed in: [actual accessible source or private user-controlled reference]
- Scope/access limitations: [what was/was not directly seen]
- Observation (not interpretation): [...]
- Candidate(s) checked: [canonical links] / novel or no match
- Competing interpretations: [...]
- Relationship: supports | challenges | mechanism-refinement | inconclusive | unrelated
- Independence/duplication: [same episode? dependent on prior evidence?]
- Privacy/disclosure permission: [where this may be preserved]
- Next step: none | reconcile | evaluate when useful
```

Keep sensitive events in a **private, user-controlled** store when permitted. Public repo records should include only appropriately abstracted, user-authorized observations; linking a public candidate must never expose a private interaction.

## Minimal cumulative candidate assessment

A cumulative snapshot should state the **hypothesis**, **canonical identifier**, **evidence currently available**, **counterevidence**, **dependent/duplicate sources**, **alternatives**, **what changed**, **what did not change**, **current uncertainty**, **evaluation priority**, and **last reviewed date**. Preserve dated history via append-only review notes, issues or PRs; do not silently overwrite earlier assessments. The [candidate index](CANDIDATE_INDEX.md) points to these records instead of becoming a second source of truth.

### Example of a justified *non-update*

An assistant is told about a single correction, and the same conversation later revisits the incident with a deeper explanation. The mechanism might become clearer, and a better test might emerge; **empirical confidence should not automatically rise** because the underlying experience has not been independently replicated.

## Safeguards and honest limits

- Task usefulness, proportionate effort, human consent, privacy, and safety override candidate harvesting.
- Never assume a user approved persistent recording merely by discussing an idea.
- A seed changes conversational guidance, **not model weights**; it cannot independently schedule background checks, remember all encounters, or update GitHub without real access and authorization.
- Candidate index entries favor retrieval, not validity. Maintain an explicit path for novel or disconfirming observations and for *no change*.
- Missing history is a coverage limitation, not evidence that no counterexample occurred.
- Audit *recognition quality* as well as resulting judgments: useful evidence noticed/missed, duplicate counts, unjustified confidence updates, false novelty, friction, and privacy outcomes.
- Maintain human review of proposed seed revisions; record adoption separately from evidence of efficacy.

## Initial evaluation

Use the controlled [experiments](../EXPERIMENTS.md) on cases with supportive, contradictory, repeated, unrelated, and genuinely novel observations, as well as cases with nothing to learn. Compare with the unchanged baseline while holding accessible context and time/effort constant. The proposed mechanism has **not** been validated merely by writing this protocol.
