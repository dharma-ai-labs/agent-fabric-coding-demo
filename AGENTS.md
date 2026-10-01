# Synthetic Job Factory

## Owned skill provenance

For maintained owned repository skill authoring, revision, packaging, and use,
apply `docs/foundation/09-skill-provenance-and-adherence.md` from verified
`dharma-ai-labs/dharmamegha` at the intended approved commit. Keep its shared
prerequisite in each entrypoint and retain exact-byte load receipts with results;
assess adherence and outcome separately. Update its coverage manifest after
reviewing changed skill bytes. Synthetic tests do not establish production or
signed-runtime compliance.

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
