# Synthetic Job Factory

This repository contains synthetic coding-demo material only.
Consult the installed Agent Fabric manifest, catalog, lexicon and applicable skills before work.
Use `npm test` to observe the current defect and verify repairs.
The Implementer owns local coding changes. The Reviewer answers bounded repository questions and reviews evidence.
Keep raw credentials, grants, provider authentication, private graders and evaluation inputs outside this repository.
Approved reports are in `reports/`; approved repository skills are in `.agents/skills/`.

## Required behavior

Applying a logical job must affect its tenant balance once. A later retry may
have a new attempt ID without becoming a new logical job. Distinct tenants
remain independent. Inputs rejected as invalid must not change state.

<!-- BEGIN:review-severity-gate -->
## Review guidelines

These rules apply to every code review in this repository, whether Claude, Codex, another agent or a person does it. They also apply to every agent that acts on review findings.

- Rate each finding from 1 to 10 on how often it would happen, and from 1 to 10 on how bad it would be. Report both scores and their product with the finding.
- For security findings, rate how often by whether an attacker can reach it, not by how often it happens in normal use.
- Score severity 9–10 for exposed customer data or secrets, lost or corrupted data, wrong money movement, or production down.
- A finding that breaks a rule stated elsewhere in AGENTS.md (for example a repository rule, security default or testing contract) always blocks the merge, whatever its score.
- If the product is below 5, leave the code alone. List the finding in the review as non-blocking, with both scores and a proposed issue title. Create the issue only where this repository's tracker rules allow it; otherwise leave it for the PR author.
- If the product is 5 or more, fix it in the change or block the merge on it.
- The threshold is 5 unless AGENTS.md sets another value for this repository.

## Scope of changes

- Do not design for rare or future cases nobody asked about.
<!-- END:review-severity-gate -->
