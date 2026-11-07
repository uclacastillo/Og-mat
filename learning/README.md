# OG-MAT Learning Ledger
*How to keep a useful map and a credible audit trail of OG-MAT's evolution.*

This directory holds the **dated evidence-and-decision trail** behind the living [Learning Map](../LEARNING_MAP.md). The map is a navigable synthesis. Review records are the history. Git commits, issues, and pull requests provide supporting links, though Git history alone is not a tamper-proof archival system.

## Why this exists

A changelog tells us **what** changed. This ledger should also tell us **why**, **from what evidence**, **who decided**, **what was uncertain**, **how the change relates to earlier ideas**, and **what happened afterward**. It should record failures and no-change reviews, not just successes.

## Folder contract

- `../LEARNING_MAP.md`: current high-level concepts, relations, and status. Update it when a meaningful relationship or status changes.
- `reviews/YYYY-MM-DD[-suffix].md`: one dated review or foundation entry. Weekly reviews should be dated by the local review date. These records are **append-only in meaning**: don't silently delete prior judgments; issue a dated addendum or later superseding record instead.
- GitHub issues / pull requests: actual discussions, proposed edits, checks, acceptance or rejection, and merge status. Link to specific issues, PRs, commits, or external references whenever accessible.
- `../SEED.md` and other core files: the material a user actually gives their assistant. Keep the portable seed compact and self-contained.

## Each weekly review must record

```markdown
# Cultivation review — YYYY-MM-DD
- Review ID: OGM-R-YYYYMMDD
- Review date / timezone: YYYY-MM-DD / America/Chicago
- Scope: repo issues, PRs, changes, public evidence, accessible generalized collaboration lessons
- Baseline: repository branch/commit or link actually checked
- Access limitations: which sources or histories could not be inspected
- Outcome: change proposed | experiment proposed | no warranted change | incomplete

## Inputs actually examined
- [source title, URL / repo reference, publication date if known, accessed date]
- Source type: peer-reviewed study | preprint | practitioner account | repo contribution | first-hand collaboration observation | other
- What it actually supports and what it doesn't

## Candidate insights
- ID: OGM-YYYYMMDD-01
- Claim: a precise, testable or auditable proposition
- Origin / provenance: source or approved abstracted observation; no private transcript
- Linked map nodes: P-##
- Evidence / contradictory evidence / uncertainty
- Alternatives considered
- Proposed disposition: test | propose revision | defer | reject
- Rationale; expected benefits and plausible harms
- How the candidate could be falsified or reassessed
- Proposed edit / experiment / issue / PR link, if any

## Decisions and lineage
- Approval state: proposed | human approved | declined | merged | superseded
- Decider and decision date if actually recorded
- Changed files / PR / commit references, if any
- Which earlier insight or rule this updates or replaces

## Next review
- Unresolved questions
- Evidence to seek
- Whether any action actually occurred
```

**Keep IDs stable.** `OGM-R-YYYYMMDD` identifies a review; `OGM-YYYYMMDD-NN` identifies a candidate. Map IDs such as `P-01` are durable concepts. If an idea changes materially, link old and new IDs with an explicit **supersedes / challenged by / supports / tests** relation.

## Weekly cultivation protocol

1. **Read before writing:** examine the current SEED, growth/integrity/evaluation guides, map, latest merged review, open cultivation PRs, and relevant GitHub discussions. Avoid duplicating or overwriting an ongoing proposal.
2. **Search for possible improvements:** inspect accessible and consent-appropriate generalized observations from collaboration, relevant credible research (including contrary findings), and community feedback. If a source isn't accessible, document the gap. Do not invent what an article, conversation, issue, or model test says.
3. **Evaluate potential generality:** would this benefit other humans and AI systems, or is it merely a local preference? Is it consistent with agency, honesty, and privacy? Is the seed becoming overly long or prescriptive?
4. **Make a disposition:** propose a justified small change; propose a test when evidence is immature; record a rejection/deferral; or record **no warranted change**. Never add novelty just to meet a weekly cadence.
5. **Maintain a dated record** for the week, including a precise audit of inputs, evidence, uncertainty, and what actually happened. For a no-change week, the review entry alone is a valid deliverable.
6. **Propose through a GitHub PR** to keep edits reviewable. Include the new review record; update the map and core files only when justified. Do not merge your own PR, silently change main during the scheduled review, or imply a proposal has been accepted.
7. **Report to the human:** concise summary of key candidates, what was verified, proposed PR/issue links, and any access limitation or pending human decision. If the required write tools are unavailable, provide a review with explicit status **not written to repository**, and do not imply the audit exists there.

## Quality and evidence gates

**Separate levels of support:**
- **Design preference:** a normative collaboration principle; does not prove benefit.
- **Promising observation:** an experience or anecdote; context-dependent.
- **Empirical evidence:** findings with an identifiable method, population, date, and limitations.
- **Verified behavior:** a check actually performed on specified model(s) and task(s); don't generalize beyond that test.

A draft PR can adopt better wording or eliminate a demonstrated ambiguity without a research study. Claims about universal effectiveness, psychological outcomes, or model superiority require stronger evidence and honest scope limitations.

Explicitly examine alternatives and disconfirming evidence where stakes warrant it. Distinguish research being published **this week** from older research first found this week. Link credible primary sources when possible; avoid citations from memory. Never represent a literature search as exhaustive unless it actually was.

## Public privacy boundary

This is a **public repository**. No private chat transcripts, identifying biographies, secrets, user files, confidential work, unconsented personal anecdotes, or private connector results belong here. Generalized insights from collaboration may be recorded only at an abstraction level that cannot reasonably expose private context. Do not auto-publish personal data while attempting to preserve provenance. Where full source detail cannot ethically be disclosed, label its origin generically and its limitations; don't fabricate a public citation.

An audit trail is not permission to collect more data. Only use material already available with legitimate access; obey platform privacy and safety requirements.

## Governance and reversibility

- **Proposal is not approval.** An open PR is not an adopted principle.
- **Merge documents adoption, not efficacy.** Evidence and approval are different dimensions.
- If a merged recommendation later proves wrong, open a corrective PR, add a new dated review linking the old one, and update the map status. Do not erase the earlier reasoning.
- Prefer minimal, reviewable changes and avoid duplicate cultivation PRs.
- Contributors should be able to fork or challenge the system; OG-MAT must remain free to outgrow its original design.

## Starting point

[2026-11-07 — Origin and baseline](reviews/2026-11-07-foundation.md)
