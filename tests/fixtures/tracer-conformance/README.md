# TRACER and Heavy-Garden Conformance Fixtures

This directory contains synthetic, owner-neutral cases for evaluating the combined TRACER and Work Ledger garden behavior. It contains no mature-ledger claims, owner names, participant data, historical garden records, private paths, or release receipts.

The exact fixture leaves are:

- `README.md`
- `cases.jsonl`
- `rubric.json`
- `trial-log.example.json`

`PROTOCOL.md`, `TRACER.md`, and the applicable adapter remain authoritative. These fixtures are evaluation evidence, not a source of requirements and not proof that an implementation works outside the recorded harness, version, prompt, environment, and trials.

## Portable startup guard

Before relying on ledger state for a conformance run, parse
`current/tracer-state.json` strictly, require `activation_status` to be
`active`, and compare its recorded `register_sha256` with the raw SHA-256 of
`current/claims.jsonl`. The hash is a content hash; a Git object ID is not a
substitute. This fixture intentionally supplies no copy-paste shell script:
compound scripts, property/method access, redirects, and shell variables are
not qualified Claude Desktop command shapes. Claude Desktop must use its
tracked adapter's separate native read and one-file hash operations. A
maintainer using another harness must implement and record an independently
qualified equivalent. In every route the harness still parses the complete
JSON state record and applies the identity, generation, cutover, and recovery
rules in the Protocol. Any failed or inconclusive guard blocks the run rather
than being treated as a warning.

## Use

1. Freeze the implementation candidate, source/requirement hashes, case file, rubric, prompt, evaluator/calibrator, harness/model version, exposed sampling settings, trial count, and failure disposition before running a case.
2. Without running the behavioral suite, prove `cases.jsonl` has exactly 38
   physical lines, all 38 are nonblank parseable JSON objects, and all 38 have
   unique nonempty `case_id` values. Reject any other shape or duplicate.
3. Use the case's named `oracle`. Mechanical cases require exact deterministic outcomes. Judgmental cases use the frozen rubric and a separately prompted or evidentially separated evaluator or named human calibration.
4. Begin critical variable cases with five trials per accessible harness unless a requirement-level reason for a different count was frozen before execution.
5. Record each run using the fields demonstrated by `trial-log.example.json`. A failed or inconclusive critical case blocks the claimed surface. Shared-model or shared-context correlation must be disclosed; majority vote cannot turn unresolved disagreement into a pass.

The case set deliberately tests both directions of the boundary:

- a complete TRACER trace does not replace the mandatory heavy-garden conservation audit; and
- a complete heavy-garden audit does not replace TRACER's pre-action trace, premise/link assessment, stance, memory decision, or dependency revisit;
- ordinary garden questions do not replace the mandatory first owner-confirmation card for relevant registered claims and their material interrelationships; and
- coordinator authorization does not replace substantive claim review, while a Deep review permits only one reviewer-directed repair and recheck before owner cancellation/rollback or maintainer recovery, never another revision or bypass.

Getting below the context limit, passing a validator, producing three agreeing reports, or recording hashes is never by itself semantic success. If the exact pinned tokenizer is unavailable, the numeric trigger/adoption gate is blocked and inconclusive; a word count is never a trigger, fallback, or compliance estimate.
