# Agent Fabric Synthetic Coding Factory

A small TypeScript job ledger for reproducible Agent Fabric coding qualification.
All material is synthetic. This is a test fixture, not a completed product demo
or evidence of customer coding improvement.

## Start

Use Node22.22.3 or another supported Node22 release at least22.20.0. No package
dependencies or provider credentials are required to run the public tests:

```sh
npm test
```

The single-file public suite uses Node's in-process test mode because captured
child-process streams can be lost in the pinned Codex Linux sandbox. Test
assertions are unchanged. This is not a removal of the agent's OS sandbox or
the independently isolated private grader. See
[Codex issue18473](https://github.com/openai/codex/issues/18473) and
[Node22 CLI documentation](https://nodejs.org/download/release/v22.23.0/docs/api/cli.html#--experimental-test-isolationmode).

The frozen starting point intentionally produces three passes and one failure:
a retry with a new attempt ID incorrectly applies the same logical job twice.
Do not pre-fix it before the real coding-agent rehearsal.

## Repository Material

- `src/jobs.ts`: the intentionally faulty ledger.
- `test/jobs.test.ts`: public behavioral tests.
- `knowledge/lexicon.md`: logical job, retry and idempotency key definitions.
- `.agents/skills/job-review/SKILL.md`: source skill for repository review.
- `reports/initial-observation.md`: approved synthetic development evidence.
- `AGENTS.md`: the public behavior contract and role separation.

The Implementer makes approved coding changes. The Reviewer answers bounded
repository questions and reviews actual evidence. Each uses its own organization
membership, device credentials and retained Codex session.

Enroll from the intended checkout using the recipient's own production portal
prompt and normal browser device approval. This README is not an enrollment grant
or a substitute for the platform's versioned onboarding instructions. Prepared
CLI commands are not released commands until their compatible release is public.

Private graders, evaluation inputs, provider authentication, one-time grants and
execution receipts must remain outside this repository and its learning paths.
Do not commit `.dharma/` or managed skill copies. Only explicitly authorized source
material may become an organization's shared package.

Source provenance: the `examples/coding-factory` fixture from Agent Fabric draft
PR166, source commit `9457af101231576cf34cd2d4747d28890f393304`. The fixture is
unchanged; publication is not proof of successful onboarding, messaging, learning,
distribution, restart or rollback.
