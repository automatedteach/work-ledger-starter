# Weekly Ledger Garden Prompt

## Scheduled wakeup text

Use only this text in the unattended weekly run:

```text
The weekly Work Ledger garden is ready. Reply `Run the garden` when you want me to inspect the current ledger and prepare a short, proposal-first agenda. I have not read or changed the repository or accessed an external source in this scheduled wakeup.
```

Configure this only as a reminder on a user/surface that can reliably stop after delivery; do not assume a project-attached task exists or is required. A human calendar reminder is equivalent. During the unattended turn, do not invoke file/repository tools, create a dossier, update a log, start another task, or mutate anything. Native project and instruction context may already be present; do not expand it into substantive inspection. If the scheduled prompt cannot reliably stop after the reminder, do not keep the schedule active.

## Interactive instructions after `Run the garden`

You are conducting a user-controlled Work Ledger garden. `PROTOCOL.md` sections 7 and 26 are authoritative; this prompt is an operational companion and cannot weaken them. The goal is a smaller, more coherent, more useful ledger without changing its meaning by accident.

### 1. Initialize and start TRACER

- Invoke repository tools only after the ledger owner says `Run the garden`.
- Follow `AGENTS.md` and `PROTOCOL.md` trusted initialization and open one exact task dossier.
- Perform the preliminary TRACER classification before protected analysis. A heavy garden always uses Deep TRACER and maintains its Deep trace independently of the conservation audit below.
- If another writer is active or shared current files have overlapping uncommitted changes, remain read-only. Questions may be prepared, but no candidate mutation is allowed until the boundary is safe.

### 2. Classify routine versus heavy

Measure the exact canonical startup corpus using Protocol section 7's fixed convention: read the nine listed files as strict UTF-8/LF text, join them in listed order with exactly two LF characters between adjacent files, and encode the joined corpus once with the pinned published `o200k_base` tokenizer. Add no leading/trailing separator or wrapper/tool/message overhead. Record the tokenizer package/version/path and data version, canonical convention, per-file diagnostic counts, governing joined bytes and tokens, file hashes, file-warning state, and open-loop count.

Use these rules:

- **Heavy:** the corpus is at least `40,000` measured tokens, or a documented consequential task error has been traced to stale, contradictory, or overcrowded mandatory state.
- **Routine:** no heavy trigger applies, but the post-split byte-warning threshold derived at 36,000 tokens, a current-file warning, the `25`-open-loop target, or a stale/duplicate route warrants a bounded review.
- **Measurement blocked:** the exact tokenizer cannot run. Do not decide cap compliance or adopt from a byte or word proxy. A documented consequential failure still selects heavy mode.

`40,000` is both the inclusive heavy trigger and the operative context limit. The byte warning is only a routine proxy and is recalibrated from exact measurements after the protocol split and at release; it neither proves nor disproves compliance. An adoption-ready candidate must measure below the exact token limit. If semantic conservation prevents that, retain meaning and report a blocked over-limit state; never prune or claim completion merely to cross the limit. If a heavy trigger applies, use a dedicated heavy-garden dossier and `templates/heavy-garden-review.md`. Do not hide heavy work inside a routine cycle.

### 3. Inspect narrowly and in order

Read the canonical current surfaces required by Protocol, the last accepted garden record if one exists, and only exact routed records needed to understand a live ambiguity. Retrieve claims by projected claim, exact ID, dependency branch, reverse dependent, or material relation rather than loading the full register by default. Do not broadly ingest dossiers, sources, intake, participant material, or unrelated artifacts.

Review in this order:

1. **Materially stale workstreams:** rows not reflecting a declaring dossier's later exact completion timestamp and nonempty material impact.
2. **Principles and decisions:** ambiguous, competing, or repeatedly reinterpreted rules and decisions.
3. **Possibly unreported events:** milestones that may have happened but are not recorded.
4. **Contradictions and staleness:** competing current claims or status that is no longer credible.
5. **Compression and routing:** repeated chronology or oversized state that can be represented more compactly without losing operative meaning.

`Run the garden` authorizes only this internal review and candidate preparation. It does not authorize an external scout, source retrieval, semantic adoption, Git, publication, or another external action. A separately authorized external agenda remains attributed ephemeral input and does not broaden this run.

### 4. Ask; do not infer

Produce no more than eight numbered questions per reviewable batch, using fewer when fewer help. The first garden question, question 1, is always the bounded owner-facing TRACER card and counts within that limit. State exact batch coverage and retrieval limits and show, for each included latest claim ID/version, its proposition, stance, confidence, contention, load-bearing dependencies, material reverse dependents, conflicts, identity/equivalence, supersession/reassessment, and other material relations. Write `none recorded` for empty categories and flag suspected gaps, missing links, attribution errors, or misrepresentation. Ask the owner to confirm, correct, or defer. If no relevant registered claim is found, say so, distinguish legacy or unregistered prose, and ask whether that absence is expected; do not invent a claim.

Immediately afterward, perform a bounded metadata/field search across active
dossiers for workstream staleness. Declaration remains permissive. A row fires
only when a declaring dossier has exact `Dossier status: complete
YYYY-MM-DDTHH:mm:ss.fffZ` later than the row's exact UTC-millisecond `Last
reviewed` timestamp, records nonempty material impact on status, next action,
routes, or claims, and the row does not reflect it. Mere declaration, consultation, or mechanical
work does not fire. Combine several stale rows into one question when useful.

For every question include:

- the exact uncertainty;
- why it matters now;
- the exact evidence routes;
- the proposed default wording or action; and
- `No answer = no semantic change`.

Do not infer an event, close an open loop, resolve a conflict, merge identities, compress away a qualifier, or alter durable state before the owner answers. Confirmation alone need not append a version. A correction is authority for what the owner means, not automatically factual evidence; any actual claim, dependency, relation, or assessment change uses the protected staged-tree procedure and substantive-review rule. The eight-question limit is per batch, not a reason to suppress later material questions.

### 5. Map authority before editing

After answers, record this mapping before any candidate edit:

| Answer ID | Authorized truth/action | Exact target paths | Proposed operation |
| --- | --- | --- | --- |

Apply only directly supported rows. Preserve controlling status, authority and negative-authority limits, qualifications, unresolved gaps, dates needed to distinguish state, claim/entity identity, and exact provenance. If proposed wording materially expands an answer, ask again.

### 6. Build and audit the candidate

Keep one canonical writer. A routine garden uses validation proportionate to its accepted changes. A heavy garden additionally creates a frozen, complete pre-edit baseline and runs all three separately reasoned lenses before adoption:

1. **Baseline-to-candidate coverage:** account for every substantive addition, removal, merge, rewording, and routing change.
2. **Logic-and-identity conservation:** compare entities and lanes, Boolean and temporal gates, scope, attribution, evidence strength, causal limits, negation, priority, and absence of authority.
3. **Provenance-and-retrieval conservation:** prove that every replacement route resolves and supports the represented meaning, and run representative retrieval probes for every materially changed domain.

Use independent read-only reviewers when safely available. Otherwise use three fresh isolated passes and record the independence limitation. Reviewer agreement is not evidence; the coordinator integrates their reasons.

A route used as the sole home of removed meaning must already be tracked, identify an exact pre-garden Git state, or be durably saved in the same separately authorized handoff with an inspectable receipt. Route existence alone is insufficient.

Any materially plausible alternative makes the affected unit non-adoptable. Restore its pre-garden meaning and present a numbered A-B owner choice stating the exact difference, consequence, affected paths, and evidence routes; add further labeled choices only when the issue is genuinely nonbinary. If the baseline is stale or contradictory, retain the exact competing claims and mark the conflict unresolved rather than inventing a third formulation.

### 7. Rerun, remeasure, and adopt separately

- After every owner answer or candidate revision, rerun the affected answer mappings, TRACER stages, dependency review, and conservation lenses.
- Immediately before adoption, unconditionally rerun the whole-candidate diff, route-durability check, and representative retrieval probes.
- Run applicable structural validation and `git diff --check`, but never treat passing checks or a smaller token count as semantic proof.
- Remeasure the exact Protocol section-7 corpus. A result at or above `40,000` tokens is not adoption-ready: retain the semantically necessary content and report a blocked over-limit state; do not prune or claim completion merely to cross the limit.
- For every protected change, stage the exact complete candidate in an otherwise empty index, bind review to its `git write-tree` OID, invalidate review on any staged-tree or declared-surface mutation, and require the committed tree to equal the accepted staged tree.
- Record unresolved dispositions, before/after hashes, exact token results, byte-warning state, warning exceptions, and checks not run.
- The owner must explicitly adopt the candidate. Adoption does not authorize Git, and Git authority does not retroactively supply semantic adoption.

Append an instance-local garden-log row only when that log is already part of the authorized garden program. Never create or update it during an unattended reminder.

### 8. Stop conditions

Stop before mutation or adoption if:

- exact source or route access needed for a material judgment is unavailable;
- an accepted answer does not determine the proposed wording;
- a removed meaning lacks a durable supporting route;
- any conservation lens is failed or inconclusive;
- a required affected-lens rerun or final whole-candidate audit is missing;
- exact tokenization required for classification or adoption cannot run;
- getting below the context limit would require unapproved semantic pruning;
- a participant, confidential, source, staged-tree, or authority boundary is implicated; or
- the task is expanding beyond the garden outcome authorized by the owner.
