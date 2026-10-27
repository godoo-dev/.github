---
name: godoo-org-capture
description: Capture, triage or retrieve Godoo organization-profile requests, work breakdowns and deferred observations in this repository's GitHub issues.
---

# Organization-profile capture

Choose the home before writing. Family-map corrections and this repository's work
belong in `godoo-dev/.github` GitHub issues. Settled public orientation belongs in
`profile/README.md` through **godoo-org-docs**. Product engineering belongs to the
identified product's own intake; retain a needed link or dependency here only when
it affects the profile outcome. Private portfolio choices stay with Marc/Fleet in
their private home; surface the need here in the conversation without contacting
another agent or writing its tracker. Routine narration stays in the session.

Use **reporting-for-humans** when available with the chosen readers, destination,
claims and qualifications. Otherwise write a self-contained problem/current result,
supporting evidence and limits, remaining acceptance and next actor. Retain useful
deferred observations early without requiring a settled solution; read-only work
or a speculative warning alone creates no write.

## Find and retain coverage

Use authenticated `gh` with the explicit repository; do not inherit a shared
issuectl store. Confirm `gh repo view godoo-dev/.github --json nameWithOwner,isPrivate`.
Open an explicit issue with `gh issue view NUMBER --repo godoo-dev/.github
--json number,url,title,body,state,labels,updatedAt`. Otherwise list both open and
closed coverage:

```sh
gh issue list --repo godoo-dev/.github --state all --limit 100 --json number,url,title,body,state
```

For complete older coverage use `gh api --paginate
'repos/godoo-dev/.github/issues?state=all&per_page=100'` and exclude objects with
`pull_request`. GitHub search indexing is supplementary, not a unique-key check.
Read likely matches and relevant linked decisions, without scanning other backlogs.

GitHub has no intake state or automatic idempotent create here. The issue body
records proposed/accepted scope, material uncertainty, acceptance and next action.
Reuse actual semantic coverage; keep closed completion as dated history. A distinct
correction needs its own identity and linked coverage, not reopening an old request.
For imported or repeatable intake, use a stable `Source-ID: sha256:<digest>` over
the complete source namespace and outcome identity; retain private originals only
in owner evidence. Never publish raw private metadata. Compare that marker in
all-state issue bodies before a create or retry. If a create response is lost,
reconcile the marker and meaning before retrying; uncertainty permits no duplicate.
This procedural deduplication is not an atomic provider uniqueness guarantee.

After the public-visibility check in AGENTS, put exact prose in an owner-paths
scratch file, then use `gh issue create --repo godoo-dev/.github --title TITLE
--body-file FILE`. Read the returned issue back. Capture creates neither acceptance,
pickup, engineering authority, schedule nor resource holding. Return only project,
canonical URL, created/updated/already-covered result, actual disposition and gaps
through the invoking conversation; send no notification.

## Triage, breakdown and changed results

Use a checklist for a small outcome; link independently useful issues for distinct
acceptance or ownership. Parent completion requires integrated acceptance even
when its pieces finish. Retrieve the parent and the affected pieces when resuming.
Known-owner technical uncertainty stays project-local; a proposed cross-project
choice is not authority to arrange delivery.

At a consequential result, blocker or decision, reread the canonical issue and
recompose its current body. Preserve useful decisions, attributed requirements,
dated evidence and remaining work; remove superseded current claims. Compare
`updatedAt`/body immediately before `gh issue edit NUMBER --repo godoo-dev/.github
--body-file FILE` and abort/reconcile changed inputs; the edit has no CAS guarantee.
Reconcile only known contradictory active summaries, including linked profile
claims, while preserving closed history. Batch related changes. Unchanged progress
needs no update. `gh issue comment` is for an explicitly requested or reader-worthy
decision, never agent messaging or routine logs. Close only supported completion
with `gh issue close NUMBER --repo godoo-dev/.github --reason completed`; use
`--reason 'not planned'` only for an actual rejection/duplicate decision. Read back
state and meaning, then resume the original work after capturing a deferred finding.
