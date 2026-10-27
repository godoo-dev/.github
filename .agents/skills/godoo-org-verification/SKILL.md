---
name: godoo-org-verification
description: Verify Godoo's public organization-profile source, navigation, visibility and publication identity; maintain those proof instructions when the interface changes.
---

# Organization-profile verification

This repository publishes Markdown orientation, not an Odoo runtime or package.
The user interface is `profile/README.md` at https://github.com/godoo-dev/.
Its only required local tooling is Git and a text reader; authenticated remote
readback uses `gh`. No product suites, Odoo containers or credentials are needed.

Before proof record `git rev-parse HEAD`, `git status --short` and
`git diff -- profile/README.md AGENTS.md .agents/skills`. Inspect the selected
candidate and unrelated dirty work; do not reset it. Confirm this is the profile
repository with `git remote get-url origin`. Keep evidence outside the checkout
through owner-paths and retain candidate/diff hashes for an uncommitted trial.

1. Read the complete profile as a new visitor. Follow public getting-started
   links to their actual repository requirements and licenses. Verify the affected
   public repository/release URLs with `gh api repos/godoo-dev/NAME` or the exact
   release endpoint. Check new relative links against source and section headings.
   Resolve claims from owner evidence, not a copied profile claim. Apply AGENTS'
   visibility boundary to every changed title, URL, example and metadata field.
2. Run `git diff --check`. Read all changed skill frontmatter/resources and AGENTS
   links; if installed skill-creator is available, run its `quick_validate.py` for
   each changed skill. Missing validators limit structural proof only. The GitHub
   Markdown API (`gh api markdown --method POST --field mode=gfm --field
   context=godoo-dev/.github --raw-field text=TEXT`) can preview actual rendering
   without changing repository content. Inspect rendered links/headings for the
   changed journey; successful rendering alone proves no product claim.
3. For an authorized publication, use normal source integration and record the
   pushed SHA. Then read `gh api repos/godoo-dev/.github/commits/main --jq .sha`
   and `gh api repos/godoo-dev/.github/contents/profile/README.md?ref=SHA`; decode
   the content and compare exact local bytes. An authenticated source readback
   proves publication at that ref, not browser rendering or every downstream link.
   If rendered-site acceptance matters, inspect https://github.com/godoo-dev/
   through an available browser and report any cache/availability limit separately.

There is no repository-owned executable CI or product publication workflow at the
initial migration. Do not claim these manual checks are enforced by branch rules;
inspect applied rules separately when enforcement is the requested question.
No process, port, remote account or data is created by this proof. Clean up only
owned scratch fixtures, retaining useful evidence. Do not replay an uncertain push:
read remote refs first. Capture a demonstrated defect through **godoo-org-capture**;
technical/product repairs require their own scope.

When profile interfaces or routes change, compare the affected instructions with
actual source and supported tooling. Repair proven instruction drift within the
task; preserve expected behavior and failing evidence for actual regressions.
Report exercised source/navigation/readback separately from untested rendered-site
behavior. Use this procedure before claiming the documentation delivery complete.
