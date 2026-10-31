# Protected Claim Delta Review

Use this rubric for one frozen staged-tree candidate. The review is process
evidence, not claim evidence and not authority to install canonical state.

The coordinator supplies schema version 2 bindings for exact base HEAD, staged
tree, one `sealed_at` value in exact UTC-millisecond form
`YYYY-MM-DDTHH:mm:ss.fffZ`, sorted declared paths, exact
add/modify/type-change/delete entries, Git object format, governing trace
reference and raw SHA-256, authenticated Standard/Deep mode, rubric raw
SHA-256, positive review iteration, reviewer identity, and the SHA-256 of the
exact review-materials manifest containing every candidate, governance,
adapter, rubric, trace, supplied deletion/preimage, and dependency/relation
surface. A mismatch or incomplete envelope makes the review inconclusive.

The single `sealed_at` binds the whole candidate. Every claim row appended by
the candidate has `recorded_at` exactly equal to it. Any later candidate-byte
change invalidates that seal and requires a fresh `sealed_at`, updated appended
rows, a fresh staged tree, and fresh review. Do not accept a reused timestamp or
a candidate with mixed appended-row timestamps.

Review the exact staged claim rows, projections, typed references, overlays,
governing trace, and material dependency/relation effects. Test whether stance,
confidence, scope, evidence roles, challenge, identity, contention,
supersession, retrieval, and dependent disposition are supported and internally
consistent. Test whole-file meaning, including changed prose around operative
fields. Do not treat validation, hashes, another agent's agreement, or the
owner's authority over their own views as independent factual evidence.

Return only one work-ledger-claim-review-response JSON object, with no fence or
surrounding prose. Copy every supplied binding without alteration, including
`sealed_at`, `candidate_changes`, and `review_materials_sha256`. Use this exact
property order:

1. `schema_version`;
2. `kind` (`work-ledger-claim-review-response`);
3. `base_head_oid`;
4. `staged_tree_oid`;
5. `sealed_at`;
6. `declared_paths`;
7. `object_format`;
8. `candidate_changes`;
9. `review_materials_sha256`;
10. `review_iteration`;
11. `reviewer_identity`;
12. `governing_trace_ref`;
13. `governing_trace_sha256`;
14. `tracer_mode`;
15. `rubric_sha256`;
16. the following substantive fields, in their listed order:

- disposition: accept, reject, or inconclusive;
- finding: compact conclusion about the exact staged tree;
- decisive_reasons: a nonempty JSON array of nonblank concrete-reason strings,
  in significance order;
- principal_challenge: strongest attempted challenge and result;
- dependency_review: affected dependencies, reverse dependents, and material
  relations, or None — <reason>;
- confidence: high, moderate, or low;
- required_change_or_blocker: null only for accept, otherwise one concrete
  repair or blocker; and
- independence_note: actual session/task separation, prevention or mutation-
  detection mechanism, and material shared-model, prompt, evidence, or framing
  limits.

These are exactly 23 top-level keys; add or omit none. `schema_version` is the
integer 2. Every supplied binding retains its Reference-section-29 JSON type and
value exactly: full lowercase object-format OIDs, strict UTC-millisecond time,
sorted arrays, positive review iteration, nonblank dispatched reviewer/trace
strings, lowercase SHA-256 values, and `Standard|Deep` tracer mode. `finding`,
`principal_challenge`, `dependency_review`, and `independence_note` are nonblank
JSON strings. `confidence` is exactly `high`, `moderate`, or `low`.
`required_change_or_blocker` is JSON null if and only if disposition is
`accept`; otherwise it is one nonblank JSON string.

Each `candidate_changes` entry uses exact property order `path`, `change`,
`base_mode`, `base_blob_oid`, `candidate_mode`, `candidate_blob_oid`; entries
and `declared_paths` are sorted by the same normalized path, and their path sets
are identical. Absence is JSON null. Treat a rename as delete plus add.

Use accept only when the frozen candidate meets the rubric. Use reject for a
concrete repairable failure and inconclusive when required evidence or judgment
is unavailable.

For Deep mode, reviewer identity differs from coordinator identity and the pass
uses genuinely fresh context. Claude's restricted reviewer records its
harness-enforced lack of shell/write tools. A Codex reviewer records the
requested read-only posture, the fact that repository policy cannot prove tool
absence, and the coordinator's required pre/post mutation comparison.

The coordinator captures the exact returned UTF-8 JSON bytes without
parsing/reserializing them, records their SHA-256 and base64 in the final
evidence wrapper, and adds coordinator identity/authority plus exact pre/post
snapshot bytes, `consumed_repair`, and mutation evidence. A parsed response view
is optional and explicitly non-authoritative. Any changed HEAD, index tree,
staged paths, declared candidate bytes, `sealed_at`, trace, rubric, review
material, state, or relevant worktree evidence invalidates the response.

After one reviewer-directed repair, review the fresh staged tree once. A second
Deep non-accept requires owner cancellation/rollback or maintainer recovery and
never authorizes another revision or bypass. Pre-review corrections
and corrections after an accepted tree do not consume the one repair, but every
byte change requires a fresh `sealed_at`, tree, and response. The accepted
wrapper records `consumed_repair` as null when none was used, or as the prior
staged-tree OID, prior wrapper raw SHA-256, exact
`review_evidence_utf8_base64` of the complete prior evidence wrapper including
its final LF, and prior `reject` or `inconclusive` disposition when the one
repair was consumed. The embedded prior wrapper's own `consumed_repair` is
null.
