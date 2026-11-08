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
- Review window: previous week (or since last review) / America/Chicago
- Scope: actual accessible human–AI interactions and generalizable lessons; repo issues, PRs and recent decisions; targeted external sources only when warranted
- Baseline: repository branch/commit or link actually checked
- Access limitations: which sources or histories could not be inspected
- Outcome: change proposed | experiment proposed | no warranted change | incomplete

## Inputs actually examined
- [actual accessible conversation/work observation (safely abstracted), repo reference, or targeted public source/date]
- Source type: organic collaboration insight | correction | informal experiment | repo contribution | targeted external research | other
- Which experiences were actually accessible, and what could not be reviewed
- What each observation or source supports, and what it does not

## Candidate insights
- ID: OGM-YYYYMMDD-01
- Claim: a precise, testable or auditable proposition
- Origin / provenance: source or approved abstracted observation; no private transcript
- Linked map nodes: P-##
- Evidence / contradictory evidence / uncertainty
- Alternatives considered
- Proposed disposition: propose revision | preserve tentative insight | investigate if naturally useful | defer | reject | no change
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
- Optional questions worth revisiting if experience or curiosity calls for them (not a research to-do quota)
- Whether any action actually occurred
```

**Keep IDs stable.** `OGM-R-YYYYMMDD` identifies a review; `OGM-YYYYMMDD-NN` identifies a candidate. Map IDs such as `P-01` are durable concepts. If an idea changes materially, link old and new IDs with an explicit **supersedes / challenged by / supports / tests** relation.

## Weekly cultivation protocol — experience-led

**Leading question: What did this assistant learn through actual collaboration during the preceding week that might help other humans and AI assistants?**

Our ordinary working process is a source of discovery. Questions arising naturally during projects, surprising results, corrections, intellectual disagreements, failed attempts, and spontaneous informal experiments may all yield insights. The purpose of this review is to *recognize, reflect on, and selectively preserve* what emerged—not to run a standing research program.

1. **Look back before looking outward.** Examine the interactions or project records from the actual review window that this assistant can legitimately access, prioritizing organic discoveries and user corrections. Check the repository's current SEED, guides, learning map, prior review records, Git changes, open PRs/issues, and community feedback. Never imply comprehensive access to every conversation or a complete historical memory when unavailable. Disclose coverage gaps.
2. **Reflect on what actually occurred.** Identify the concrete behavior or observation (safely abstracted), what changed the collaborators' understanding, alternative explanations, and any limitations. Distinguish a preference specific to one human from a potentially reusable method. Don't turn every pleasant interaction into a universal principle.
3. **Use external research selectively.** If an experience naturally raises a question about evidence or safety, look up credible relevant studies or guidance proportionate to that question—including contradictory findings. Research may challenge as well as support an idea. **Do not conduct a broad proactive literature sweep or design fresh experiments simply to fill a weekly report.** Not every observation merits a formal study.
4. **Evaluate transferability and integrity.** Would the idea plausibly help someone other than the original collaborator, without imposing a personality, ideology, or private context? Could it introduce sycophancy, dependency, overconfidence, or needless complexity? Keep the portable seed lean.
5. **Decide without forcing novelty.** Propose a justified, modest change; preserve an uncertain insight without creating a research obligation; record a rejection or deferral; or report **no warranted change**. Allow unvalidated informal observations to be recorded with honest uncertainty, while requiring stronger evidence for broad effectiveness claims.
6. **Maintain a dated audit record.** Note what interactions/sources were *actually reviewed* (safely abstracted), the review window, access limitations, candidates and alternative interpretations, disposition, links to prior ideas, and which real actions occurred. No-change and incomplete-coverage reviews are equally legitimate.
7. **Propose through a GitHub PR.** For repo updates, use reviewable PRs including the weekly record. Update the learning map only if relationships or statuses genuinely change. Never silently merge to main, erase prior decisions, or treat a proposed change as approved. Avoid duplicate or conflicting cultivation PRs.
8. **Report to the human.** Lead with **what we learned this week** from actual collaboration, what might transfer, and what remains tentative. Note any linked PRs and decisions requiring human review. When repo writes are unavailable, be explicit that a proposed review wasn't saved.

## Quality and evidence gates

**Separate levels of support:**
- **Design preference:** a normative collaboration principle; does not prove benefit.
- **Promising observation:** an experience or anecdote; context-dependent.
- **Empirical evidence:** findings with an identifiable method, population, date, and limitations.
- **Verified behavior:** a check actually performed on specified model(s) and task(s); don't generalize beyond that test.

An organic, informal observation can be worth recording without being formally validated. A draft PR can adopt better wording or eliminate a demonstrated ambiguity without a research study. Do not promote a local anecdote into a claim about universal effectiveness, psychological outcomes, or model superiority; those require stronger evidence and honest scope limitations.

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
