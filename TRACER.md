# TRACER — Explicit, Proportional Claim-Dependency Reasoning

## Authority and precedence

`PROTOCOL.md` section 32 incorporates this file for material Work Ledger reasoning. Protocol remains controlling for owner authority, source and connector access, external action, Git, lifecycle, privacy, concurrency, and save/review/recovery boundaries. The owner-attested operational document copied below controls TRACER's epistemic and trace minima. A stricter Protocol rule constrains action; it does not waive a TRACER minimum. An unresolved incompatibility stops the affected action for owner resolution.

The copied body is preserved as source-authenticated normative text. The Work Ledger binding profile after it instantiates repository paths and closed implementation choices without changing that body.

<!-- BEGIN OWNER-ATTESTED DOCUMENT (ii) BODY -->
(ii) TRACER — Explicit, Proportional Claim-Dependency Reasoning

Apply TRACER before any consequential conclusion, recommendation, criticism, action, or durable-memory write, and whenever new information may invalidate reasoning already in use.

Mandatory textual trace

Create and maintain an explicit textual TRACER trace before acting on a material result. Do not rely on reasoning that has not been represented in text.

The trace may reside in a task-local reasoning buffer, scratch document, run log, structured artifact, worker return, or final response, but it must be available to every later stage that relies on it.

Use this envelope:

TRACER TRACE
Mode:
T — Target and triage:
R — Reconstruction:
A — Assessment:
C — Challenge:
E — Established result:
R — Record and revisit:

The trace need not reproduce every intermediate thought. Record the claims, dependencies, evidence, objections, uncertainty, and memory consequences that could materially change the result.

If no inspectable task-local textual workspace exists, place the required trace in the final response. For consequential user-facing outputs, always expose at least the conclusion, decisive reasons, confidence, and principal uncertainty or challenge.

A material claim is one whose revision could change a conclusion, action, plan, or future reasoning. A durable claim is likely to matter after the current task. A load-bearing claim is a material premise on which the result actually depends.

Proportionality rule

Use the lightest level of rigor likely to preserve decision quality, but create a textual trace at every level.

Light

Use for low-stakes, reversible, local, familiar, and ephemeral work with no serious conflict.

Write a compact trace containing:

the exact target;
the decisive reason or premise;
the principal sanity or disconfirming check;
the result and confidence;
and the memory decision.

Normally use no workers and make no canonical memory write.

Standard

Use for material recommendations, nontrivial interpretations, durable conclusions, or memory writes.

Write:

a clear premise–conclusion representation;
assessments of the load-bearing premises and links;
at least one serious attempted challenge;
the final stance, confidence, and practical decision;
and an explicit memory delta.
Deep

Use for high-stakes, irreversible, novel, contested, conflicted, or widely dependent conclusions.

Use, as warranted:

a richer argument or claim map;
multiple independent argument lines;
bounded worker traces;
adversarial checks;
conflict reconciliation;
and explicit downstream dependency review.

Escalate when stakes, uncertainty, irreversibility, novelty, evidential conflict, ambiguity, expected reuse, or dependency breadth increase. Reuse prior assessments whose scope and currency still match. Do not recompute unaffected branches.

Authority and delegation

The orchestrator owns:

the target and scope;
the selected rigor mode;
relevant-memory retrieval;
the shared reconstruction;
delegation boundaries;
integration of worker results;
the final epistemic stance;
the practical decision;
the canonical-memory write;
and dependent review.

Before dispatching workers, write the delegation plan in the trace.

A worker receives:

an exact claim, relation, or question;
the smallest sufficient context;
source and freshness constraints;
a required output schema;
and a stopping condition.

Each worker returns:

Claim or question:
Interpretation or reconstruction:
Evidence or source references:
Inferential significance:
Counterevidence or search limitation:
Finding and confidence:
Proposed task or memory delta:

Workers may create task-local textual artifacts but may not promote findings into canonical memory. Delegate only when the work is bounded and separable and the expected gain in speed, coverage, expertise, or independence exceeds context-transfer and integration costs.

Reconcile workers by examining their evidence and reasoning, not by counting votes. Record whether apparent agreement is genuinely independent.

T — Target and triage
Write the exact proposition, decision, criticism, or action under consideration.
Write its material scope:
entities;
time;
location;
conditions;
quantifiers;
exceptions;
and operative meanings.

When a doctrine, feature name, policy name, thesis label, or shorthand is used, record both:

the retrieval label; and
the precise statement or version being evaluated.

Use labels for retrieval and statements for reasoning.

Identify whether the target is factual, causal, predictive, interpretive, normative, procedural, or mixed when this changes what evidence is required.
Write the epistemic or practical threshold:
What would warrant acceptance, rejection, or suspension?
What confidence is required?
Is an action required even if the proposition remains unresolved?
Do downside risks justify a precautionary threshold?

Retrieve relevant memory.

Begin with:

exact IDs;
exact labels;
known aliases;
direct dependencies;
and recent relevant records.

Expand semantically when exact retrieval is inadequate, ambiguity or synonymy is likely, or duplicate identity is in question.

Write the retrieved claim IDs or summaries and flag any stale, conflicted, ambiguous, provisional, or superseded records that may matter.
Select and record Light, Standard, or Deep mode.
Decide whether any bounded questions merit delegation. Write the reason for delegation or nondelegation.
R — Reconstruct
Locate the reasoning through:
surrounding context;
signposting;
direct inquiry where possible;
a provisional first-pass interpretation;
and reconsideration as new information appears.
Write one line of argument at a time:
P1. Essential premise
P2. Essential premise
P3. Indispensable implicit bridge premise
C1. Material intermediate conclusion
C. Target conclusion

A compact equivalent is acceptable in Light mode, but the support structure must be textual.

Exclude:

irrelevant background;
premises supporting a separate argument;
objections;
evidence against the conclusion;
and premises for the opposite conclusion.

Represent these separately when material.

Mark each material claim, when relevant, as:
explicitly stated;
reconstructed from context;
inferred by the agent;
assumed for analysis;
or proposed as a repair.
Keep separate textual sections for:
faithful reconstruction;
evaluation;
objections or arguments for the negation;
and repaired reasoning.
Never silently improve an argument and attribute the improved version to its source.
Do not merge claims merely because their wording or embeddings are similar. Write whether they are:
identical;
aliases;
equivalent;
versions;
clarifications;
or merely related.
Use a simple premise list for simple cases and a richer map for complex cases. Do not omit the explicit representation merely because a graphical or database representation would be excessive.
A — Assess
Premises

For every load-bearing premise, write an assessment addressing the vulnerabilities that could change the result:

evidential support;
whether the evidence is direct or indirect;
source reliability, expertise, and access;
scope;
counterevidence;
temporal currency;
and dependence on shared sources or assumptions.

Use compact entries when possible:

P2: Supported by S1; current as of v4.2; scope matches; moderate-high confidence.

Distinguish source roles:

evidence — bears on whether the claim should be accepted or rejected;
meaning — helps define or interpret the claim;
context — supplies relevant background without itself establishing the claim.

Do not treat a source that formulates, names, or popularizes a claim as automatically providing evidence that the claim is true.

Inferential links

For every load-bearing inferential link, write:

Whether the premises could all be true while the conclusion is false.
If so, how strongly the premises nevertheless support the conclusion.
Any indispensable unstated bridge premise.
Whether the evidence establishes the full conclusion or only a narrower claim.
Whether apparently separate support lines are genuinely independent.
Whether the reasoning is deductive, inductive, abductive, causal, analogical, practical, or mixed when this affects evaluation.

Do not let agreement with a conclusion substitute for assessment.

When support ends, write the remaining foundation as an assumption, unresolved claim, or evidential gap. Do not invent deeper justification merely to complete the structure.

Calibrate confidence to the complete support structure. Do not count repeated summaries, correlated workers, or derivative sources as independent corroboration.

C — Challenge

Write at least one realistic attempted challenge for every material Standard or Deep result. In Light mode, write the most relevant sanity or failure check.

Select challenges proportionately from these families:

Counterexample or boundary

Can the premises hold while the conclusion fails? Does a nearby case reveal an exception or limitation?

Alternative or exhaustiveness

Is another explanation, interpretation, option, or course of action available? Do not treat a list as exhaustive unless exhaustiveness is supported.

Coherence and similar cases

Does the claim conflict with accepted claims, dependent plans, or the treatment of materially similar cases? Is an exception principled or ad hoc?

Meaning and scope

Has a term, quantifier, population, condition, standard, or time frame shifted between premise and conclusion?

Independence and provenance

Is the support circular, stale, duplicated, authority-dependent without underlying evidence, or correlated across sources or workers?

Write the challenge and its result:

Challenge: Candidate explanation X fits the evidence without P3.
Result: P3 is not established; narrow C from “must” to “probably.”

Do not infer absence merely because a limited search found nothing unless the search procedure warrants that inference.

If a challenge materially alters the argument, revise the written reconstruction or assessment. Do not patch the conclusion without updating its trace.

E — Establish
Integrate the evidence and reasoning in writing. Worker agreement is not itself evidence.
Assign and record an epistemic stance:
accept;
reject;
suspend — assessed but unresolved;
unassessed — not substantively examined.
Record confidence using the system’s standard scale.
Keep distinct:
the proposition;
the argument for it;
the stance toward it;
confidence;
the practical decision;
and the memory record’s operational status.
Do not confuse suspension or lack of assessment with the separate proposition that a claim is neither true nor false.
Keep epistemic judgment separate from practical choice. A precautionary or risk-sensitive action may be warranted while the underlying factual claim remains suspended.
As warranted:
repair the argument;
narrow the conclusion;
restrict its scope;
add a principled exception;
lower confidence;
reject the claim;
or suspend judgment.
Do not infer that a conclusion is false merely because one argument for it fails. Check for independent support.
Write what would materially change the result.
For consequential final outputs, present at least:
Conclusion or decision:
Scope:
Confidence:
Decisive reasons:
Principal challenge or uncertainty:
What would change the result:

A fuller trace may remain in the task-local artifact when available. If no such artifact is inspectable, include the complete trace in the final output.

R — Record and revisit
Record
Complete the trace with an explicit memory decision.
Memory delta: None — local and ephemeral.

or:

Memory delta: Add C17; supersede C8; mark Plan-4 for review.
Keep task-local candidate reasoning explicit throughout the run. Persist it canonically only when it is durable and material or when its unresolved status must constrain future agents.
Use the existing memory substrate. If it lacks structured claim storage, maintain one compact standing claim ledger rather than creating an unrelated file for every task.
Use this minimal durable record:
id: stable substrate identifier
claim: precise statement including material scope and time
stance: accept | reject | suspend | unassessed
confidence: system-standard scale
basis:
  - reference: source or durable claim reference
    role: evidence | meaning | context
    as_of: date or version when relevant
depends_on:
  - only load-bearing durable claim IDs
caveat_or_review_when: material limitation or update trigger
supersedes: optional prior record for a material revision
Add optional labels, aliases, claim types, relation metadata, and review dates only when they improve retrieval, interpretation, or update behavior.
Do not create a separate durable premise record merely because a premise appeared in the current trace. Create one when the premise is independently reusable, revisable, contested, volatile, or shared by multiple conclusions. Otherwise summarize it in the parent claim’s basis.
At minimum, distinguish when relevant:
necessary dependence or entailment;
defeasible support;
strict inconsistency;
broader conflict;
identity or aliasing;
and supersession.
Use specialized relations such as version_of, clarification_of, dichotomy, causal, interpretive, source-of-meaning, or reported because_of only when the task depends on their semantics. Write those semantics explicitly.
Store source references rather than duplicating long passages.
Store one canonical dependency direction and derive reverse dependents through an index or search.
Workers may propose a ledger delta. Only the orchestrator may authorize canonical commitment.
Preserve history for material changes in meaning, scope, stance, confidence, evidence, or dependencies. Non-semantic corrections may be edited in place.
Treat current, active, or canonical as approval for present operational use, not as a guarantee of truth.
Revisit

When a material claim or relation changes, write a dependency-review trace:

Changed claim:
Reason for change:
Direct load-bearing dependents:
Assessment of each dependent:
Plans or actions affected:
Further propagation required:
TRACER stage to re-enter:

Then:

Find direct dependents for which the changed claim was load-bearing.
Reassess those dependents explicitly.
Continue transitively only when a dependent conclusion, decision, or action changes materially.
Revise, suspend, or roll back affected plans and actions as warranted.
Re-enter TRACER at the earliest invalidated stage:
changed meaning or scope → Target;
changed interpretation → Reconstruct;
changed evidence or inference → Assess;
new counterexample or conflict → Challenge;
changed practical or epistemic judgment → Establish;
metadata-only correction → Record.

Stop when:

the explicit trace contains all load-bearing assumptions;
material ambiguity and conflict are resolved or represented;
stance and confidence are proportionate to the support;
the practical decision threshold has been addressed;
the memory delta and review conditions are explicit;
affected dependents have been reconsidered;
and further work is unlikely to change the result enough to justify its expected cost.
<!-- END OWNER-ATTESTED DOCUMENT (ii) BODY -->

## Work Ledger binding profile

### Runtime profile

Use the qualitative confidence scale `high | moderate | low`; use `null` exactly when stance is `unassessed`. If the source example says “moderate-high,” record `confidence: "moderate"` and `confidence_note: "toward the high end"`.

A trace is an inspectable decision-relevant account, not hidden chain-of-thought. It records the target and threshold, decisive claims and links, separate warrant assessments, the strongest relevant challenge and result, the scoped conclusion and decision, and the memory/dependency disposition. It may cite sensitive evidence without reproducing it.

Task-local traces use a unique marker such as `TRC-YYYYMMDD-01` in the initialized dossier. Standard and Deep work uses that dossier, except that an explicit bounded read-only consultation that forbids workspace writes puts the complete required trace in its final response as noncanonical, nondurable analysis. Each governing delimited trace contains exactly one literal `Mode: Standard` or `Mode: Deep` line. A material Light task that is legitimately non-substantial records the compact trace in inspectable task-local output. Worker returns use provisional local handles and never allocate canonical claim IDs.

The exact durable delimiters are:

```text
<!-- TRACER TRACE BEGIN: TRC-YYYYMMDD-01 -->
...
<!-- TRACER TRACE END: TRC-YYYYMMDD-01 -->
```

The begin and end IDs must match and be unique within the file. A claim's
`trace_ref` names the containing repository-relative path plus `#` and that ID;
`trace_sha256` hashes the exact UTF-8 bytes beginning with the begin delimiter
and ending with the end delimiter, including both delimiter lines and every
intervening line but excluding a following line break. Historical referenced
trace bytes are immutable; corrections append a newly marked trace.

The final Record step states one of:

- the exact canonical memory delta and dependent-review disposition;
- `Memory delta: None` with the reason; or
- a blocked/pending delta with the exact unmet authority or evidence gate.

A trace written after reliance does not satisfy the rule. A changed premise, dependency, scope, authority, environment, or counterexample re-enters the earliest invalidated TRACER stage. Mechanical reuse is allowed only after the exact governing trace is cited and all material reuse conditions are rechecked.

### Closed output variance

Protocol sections 27, 28, section 29's exact ordinary Participant checkpoint,
and section 31 retain their fixed setup, phase-one completion, semantic A/B/C,
source-only, bounded local-save, correction/recovery, and readiness outputs and
attached stop/no-extra-question behavior. Their complete trace remains
inspectable, but those enumerated user-facing messages are the only
owner-authorized variance from TRACER’s ordinary consequential-output minimum.
No other output inherits this variance.

Outside that closed set, consequential user-facing output exposes naturally or with labels: conclusion or decision, scope, confidence, decisive reasons, principal challenge or uncertainty, and what would change the result.

### Durable-claim profile

`current/claims.jsonl` is the sole CLM-scoped authority. It is one component of current state, not a replacement for decisions, owner preferences, open loops, source records, dossiers, or artifacts. Each nonblank physical line is one immutable UTF-8/LF JSON record version. The empty register is exactly zero bytes.

Required properties, in serialization order:

```json
{
  "id": "CLM-0001",
  "record_version": 1,
  "claim": "One precise, nonblank, single-line proposition with material scope and time.",
  "stance": "accept",
  "confidence": "moderate",
  "record_status": "current",
  "contention_status": "uncontested",
  "created_at": "YYYY-MM-DD",
  "last_assessed_at": "YYYY-MM-DD",
  "recorded_at": "YYYY-MM-DDTHH:mm:ss.fffZ",
  "basis": [],
  "depends_on": [],
  "relations": [],
  "caveat_or_review_when": "A material limitation or review trigger.",
  "supersession_events": [],
  "trace_ref": "dossiers/active/YYYY-MM-DD__task.md#TRC-YYYYMMDD-01",
  "trace_sha256": "64 lowercase hexadecimal characters",
  "current_views": [],
  "authority_refs": [],
  "labels": [],
  "aliases": []
}
```

Optional properties are `confidence_note` and, only when analytically useful, `claim_type` with `factual | causal | predictive | interpretive | normative | procedural | mixed`.

One stable ID denotes one materially unchanged proposition. In schema version 1,
the exact `claim` string is immutable across versions of that stable ID; even a
nonsemantic wording correction receives a new ID because no reviewed correction
authorization exists. IDs are ledger-local, monotonic, never reused after
canonical inclusion in an exact protected commit, and final only through the
exclusive staged-tree claim procedure. Versions start at 1 and are
contiguous. A material assessment, warrant, dependency, contention, review,
lifecycle, relation, or visibility change appends the next version. A material
proposition, meaning, scope, condition, or time change receives a new ID. Every
prior register byte remains an exact prefix.

A stable claim ID is `CLM-` plus one ledger-global positive integer rendered as
unsigned base-10, left-padded with zeroes to a minimum width of four and never
truncated: `CLM-0001`, `CLM-9999`, then `CLM-10000`. Existing canonical IDs
remain unchanged. Under the exclusive writer, freeze the greatest valid
committed global claim ordinal M once immediately before candidate allocation,
or 0 for an empty register. Sort all new exact claim proposition strings in the
candidate by ordinal UTF-8 bytes, reject duplicates, and assign M+1, M+2, and
so on in that order, counting earlier provisional rows in the same candidate.
No assigned ID becomes canonical unless that exact staged tree commits; an
abandoned candidate's provisional IDs remain reusable.

`stance` is `accept | reject | suspend | unassessed`. Confidence measures warrant for that stance, not probability that the proposition is true. `record_status` is `provisional | current | superseded | legacy`; `contention_status` is independently `uncontested | contested`. Unassessed rows have null confidence and null `last_assessed_at` and are only provisional, legacy, or a historically preserved superseded unassessed row. Assessed provisional/current rows have nonnull confidence and assessment date. `recorded_at` is the Seal time in exact UTC millisecond form and never the completion time.

Every assessed row has at least one durable `basis` entry with truthful role `evidence`. Meaning and context sources do not become evidence by citation. Authority references record governing authority and never substitute for factual evidence. Source classification, retention, permission, and original-use gates remain independent.

A claim-valued basis reference is pinned exactly as `claim:<stable-claim-id>@vN`, where the stable ID uses the minimum-four-digit, never-truncated grammar above, and includes Boolean `load_bearing`. Role remains truthfully `evidence | meaning | context`, independently of that Boolean. Set `load_bearing: true` only when revision of the cited claim could materially affect this row’s stance, confidence, scope, interpretation, caveat, review condition, or warranted reliance. The stable IDs in `depends_on` equal exactly the IDs of load-bearing claim-basis entries. Each dependency is uniquely `necessary-dependence` or `defeasible-support`; self-edges, dangling targets, and support cycles are invalid.

Core relations are `strict-inconsistency`, `broader-conflict`, `identity`, `alias`, `equivalent`, `version-of`, `clarification-of`, and `related-to`. Symmetry, direction, storage, and effect follow the schema-1 binding table below. Specialized relations require nonblank semantics and never silently establish support, identity, or propagation.

For this table, **owner** means the stable ID of the row containing the relation
object and **target** means its `id`. A symmetric relation is stored as one edge
on exactly one endpoint; exact incoming search supplies the reverse view, and a
reciprocal duplicate of the same typed/semantic edge is invalid. A directed
relation is stored only as owner to target. Retrieval exposes both stored
directions and derived incoming routes without manufacturing a second edge.

| Relation | Closed schema-1 meaning and direction | Identity and propagation effect |
| --- | --- | --- |
| `strict-inconsistency` | Symmetric: the two propositions cannot both hold under their recorded scopes, conditions, and times. | No identity cluster and no warrant transfer. Expose the conflict and review both endpoints and affected uses. |
| `broader-conflict` | Symmetric: the propositions materially conflict or pull against each other, but strict joint impossibility is not established. | No identity cluster and no warrant transfer. Expose the conflict and review both endpoints and affected uses. |
| `identity` | Symmetric, explicitly adjudicated identity of proposition. | Joins the supersession/identity routing cluster, which has at most one active member. Route to that member; do not transfer warrant silently, and review affected dependents. |
| `alias` | Directed: owner is an alternate or legacy identity route to the target canonical identity. | Joins the same routing cluster and active-member constraint as `identity`. It does not itself establish evidential support or transfer warrant. |
| `equivalent` | Symmetric: the propositions have equivalent truth conditions for the recorded scope while their stable identities remain distinct. | Does not join an identity cluster, merge records, establish support, or transfer warrant. |
| `version-of` | Directed: owner is a scoped or derived version of target. | Does not imply identity, supersession, support, or warrant transfer. |
| `clarification-of` | Directed: owner makes target more explicit without replacing it. | Does not imply identity, supersession, support, or warrant transfer. |
| `related-to` | Symmetric relevance only. | Never establishes identity, support, dependency, or propagation. |

No ordinary relation substitutes for `depends_on`; only the exact load-bearing
dependency model carries claim support and its reverse-dependent closure. A
material relation change still requires review of both endpoints, incoming and
outgoing uses, identity routing where applicable, and any operational reasoning
that relied on the relation. A specialized relation is mechanically directed
owner to target unless a later schema defines a closed symmetric type; its
nonblank `semantics` states the task-relevant meaning but cannot create an
identity cluster, dependency, or automatic propagation.

Every row has `supersession_events: []`. An assert event introduced on a row has an immutable row-derived event ID, targets the exact pre-candidate active `<stable-claim-id>@vN` under the minimum-four-digit, never-truncated grammar above, and cites its trace and trace hash. At most one assert may be introduced per row. A later immutable retract event cites one earlier unretracted assert, gives a reason, and either installs an exactly matching replacement ordinary relation in the same reviewed staged tree or records null plus a nonblank replacement reason. A mistaken relation is retracted, never erased. Current routing and identity clusters use effective asserts; chronological reconstruction retains every assertion and retraction. The effective graph is acyclic and has at most one active member per cluster.

A retract event normally appears in a later version of the stable claim ID that
introduced its assert. Cross-ID retraction is valid only when the protected
candidate records explicit identity authority and rationale and reviews both
stable IDs plus affected dependents. Multi-predecessor consolidation is outside
schema version 1 and stops for a later explicit schema/semantic decision.

### Projections, references, and retrieval

Only these five canonical Markdown current files may contain full startup
projections: `current/context-pack.md`; `current/decisions.md`;
`current/open-loops.md`; `current/technical-preferences.md`; and
`current/context-map.md`.

```text
- **Claim CLM-0001@v1 [accept; moderate; current; contested]:** <exact claim>
  - **Confidence note:** toward the high end
```

The note line is omitted when absent. Every path in `current_views` has exactly one byte-equivalent metadata projection, and no unlisted path has one. Rejected, suspended, unassessed, legacy, or contested claims are never presented as unqualified assertions.

Registry-only supporting claims have no full projection. They remain discoverable through an incoming dependency, an exact typed operational reference, or a meaningful label/alias. Typed references use these exact field labels:

```text
Load-bearing claims: CLM-0002 (evidence), CLM-0007 (meaning)
Related claims: CLM-0009
TRACER overlay: CLM-0010
```

A decision without independently durable claim support uses `Load-bearing claims: None — <reason>; trace: <trace_ref>`. Stable IDs float to the latest row unless an explicitly historical reference pins `@vN`.

The schema-1 operative text-surface set is closed. Full projections are valid only in the five current Markdown files above. The three exact field labels form operative typed fields only when their bodies match the complete grammar above and they appear in ordinary text in: those five current files; the exact initialized `dossiers/active/YYYY-MM-DD__slug.md` dossier and any exact active dependent dossier authorized by the protected staged-tree candidate; ledger-authored `sources/contained/<source-id>/extract.md` and `sources/green/<source-id>/extract.md` in a declared claim-bearing profiled phase two; and an exact path under `artifacts/` ending in `.md` or `.txt` that the protected candidate explicitly authorizes. An operative full projection in any non-current surface is invalid, not an alternate projection.

Lines inside fenced code blocks, indented code, or block quotes are examples or data rather than operative projections or typed fields. For this closed parser, a block-quoted paragraph and every following nonblank continuation line remain nonoperative until a blank line; begin operative claim syntax after that blank boundary. A CLM ID in ordinary prose is not a typed reference. Raw intake and retained source originals—including `.md` and `.txt` originals—and manifests, pointers, profiles, state, CSV, Office/PDF, image, and other structured or binary artifacts are not claim text surfaces. This parsing boundary does not make their content epistemically irrelevant or waive TRACER; after authorized reading, it retains its truthful evidence, meaning, or context role. When inert data needs an operational claim link, place the exact typed field in an authorized companion `.md`/`.txt` artifact, source extract, current file, or dossier.

A supported text surface is BOM-free strict UTF-8 with LF-only line endings and is protected as one exact byte sequence. If either its committed preimage or candidate operative text contains a full projection or syntactically complete typed field, every byte change to that file—including surrounding-prose changes, relocation, or removal with unchanged field text—uses the applicable protected staged-tree procedure and its accepted unchanged tree. An incomplete or malformed legacy label in an otherwise nonoperative file is inert. Once either image contains a complete field or projection, the raw whole file is validated and every malformed exact typed-field or projection line is invalid. This is stricter than comparing parsed fields alone and closes recontextualization and time-of-check/time-of-use gaps.

Exact-ID retrieval returns the latest row, complete effective and historical supersession path, the unique active cluster member or literal `no active member`, incoming and outgoing material relations, direct dependencies and reverse dependents, typed operational references, and relevant trace/basis routes. Similarity proposes candidates only and never merges them.

### Prospective cutover and sparse recording

Pre-cutover history remains valuable legacy memory: not yet TRACER-substantiated, not false or unusable. Do not mass-assign IDs, rewrite history, or imply retrospective validation. When a legacy item becomes load-bearing, retrieve the best permitted original evidence, distinguish source statement from prior and present inference, create the smallest reviewed record or overlay, qualify proof gaps, and leave unrelated history untouched.

For a migrated generation-zero cutover, the operative adoption-decision section references every reserved seed exactly once, and that sole typed occurrence is `Related claims: CLM-…@v1`. The section contains no additional pinned or floating occurrence of a reserved seed under any typed field and never cites a reserved seed through `Load-bearing claims` or `TRACER overlay`; newly created seed claims are results of the decision that activates them, not premises or legacy overlays for that decision.

Create a claim row only when the proposition must be stable independently of one task, artifact, decision, or source entry and future reliance benefits from explicit assessment or change propagation. Do not turn every trace sentence, task result, citation, or practical decision into a claim.

### State, staged-tree review, and recovery binding

`current/tracer-state.json` is the startup-visible state record. It retains
activation status, ledger instance, claim generation, exact raw register
SHA-256, and native or migrated cutover metadata. Missing, malformed,
identity-mismatched, hash-mismatched, or `pending` state blocks ordinary
protected work. A neutral unbound seed permits only exact profile setup until
its ledger ID is bound. Git object identity supplements but never replaces the
raw content SHA-256.

Every write touching the register, a full projection, a typed claim reference,
or a TRACER overlay uses one exact protected candidate under Protocol section
29. The coordinator records canonical root, branch and base HEAD, complete
sorted declared paths, path preimages, intended transition, governing trace
reference and raw hash, authenticated Standard/Deep mode, and any provisional
ID/version mapping. The index is empty before those exact paths are staged.

After the final semantic draft, the coordinator captures one `sealed_at` in
exact UTC-millisecond form and makes every appended row's `recorded_at` equal
it. Any later candidate-byte change requires a fresh `sealed_at`. The output of
`git write-tree` then gives the seal its immutable complete-candidate identity.
Candidate validation resolves the one governing delimited
trace, derives its mode, rejects Light laundering, verifies every appended row
cites that trace/hash, verifies register prefix/graph/projections/references and
the next state generation/hash, and preserves a retrieval route for every
registry-only claim. Any changed staged byte, path set, trace, rubric, base
HEAD, or declared dependency surface invalidates the tree's review.

A protected artifact addition/change is an exact declared `.md` or `.txt`
path. A deletion requires explicit path-level deletion authority, keeps the
tracked regular preimage available through review, and binds the absence plus
every removed typed reference in the staged tree. Other artifact formats stay
under ordinary task/Git authority; Participant ordinary save permits no
deletion.

Every protected candidate binds exactly two roles:
`coordinator-authorization` and `claim-reviewer`. The reviewer applies the
tracked rubric to the frozen staged tree and returns disposition, finding,
decisive reasons, principal challenge/result, dependency/relation review,
confidence, required change/blocker, and per-review independence note. `accept`
requires no blocker; `reject | inconclusive` requires one.

The reviewer response repeats exact base HEAD, staged tree, `sealed_at`, declared
paths, add/modify/type-change/delete identities, review-materials hash, reviewer identity,
governing trace reference/hash/mode, rubric hash, and review iteration. The
coordinator preserves the exact response bytes by SHA-256 and base64 in a
process-evidence wrapper with coordinator identity/authority and exact pre/post
mutation snapshots. Mismatched, replayed, changed, unauthorized, stale,
reason-free, rejected, or inconclusive evidence blocks commit. A tracked
evidence file cannot contain its own tree OID, so the exact wrapper bytes and
hash are carried durably in the commit message; the ignored sidecar is only a
local convenience copy.

Deep requires reviewer identity distinct from the coordinator and a genuinely
fresh separate pass. Claude may use harness-enforced read-only tools. Codex uses
fresh context, requested read-only posture, byte-identical required snapshots,
and the mutation-event surface actually available. A mismatch or observed
mutation invalidates review. Every independence note says that tool absence and
unobserved transient mutation cannot be proved, and discloses shared model,
prompt, evidence, and framing limits.

One Deep non-accept may drive one reviewer-directed repair: exact-path unstage
without deleting working bytes, one revision, a new staged tree, and fresh
review. A second Deep non-accept blocks further revision in that checkpoint and
requires owner cancellation/rollback or maintainer recovery; it never
authorizes another revision or bypass. Pre-review or accepted-tree corrections
do not count as that repair, but every byte change invalidates prior review.

Commit only an accepted unchanged tree and verify the commit tree equals its
OID. Each claim-bearing or projection/reference/overlay-only protected commit
increments `claim_generation` exactly once and updates raw register SHA-256,
including a protected surface change with zero new register rows. Setup, phase
one, source-only, and zero-body paths reserve no IDs and cannot modify claims or
generation.

On interruption, committed HEAD remains canonical. Preserve incomplete bytes
first and resume only when exact paths match recorded prior, partial, intended,
staged, or committed state. An exact completed commit resumes only verification
and authorized cleanup; it is not rolled back. Never broad-reset, clean, stash,
amend, rebase, pull, switch branches, force, or delete recovery evidence.
Source/intake bytes survive until committed blobs verify.

A task checks the small state record before consequential action and final
Establish. A generation or hash change triggers bounded relevance review and
re-enters substantive Revisit only for a potentially load-bearing change.

### Workers, ingestion, gardening, and validation

The coordinator owns the shared Target, final stance, integration, action, ID mapping, and canonical memory write. Workers receive a bounded written envelope, use local handles, return mini-traces, and remain provisional. Agreement is not independent evidence merely because several workers say the same thing.

Profile setup, ingestion phase one, semantic-card construction, owner choice, source-only, and zero-body paths each receive the proportional trace required by Protocol. Storage approval, owner meaning, or contextual relevance never launders a source or worker output into evidence.

The first garden question in every routine or heavy interactive garden is Protocol section 26's bounded owner-facing card for the exact included latest claims, assessments, dependencies, reverse dependents, conflicts, identity/equivalence, supersession/reassessment, other material relations, suspected gaps, and retrieval/coverage limits. Empty categories say `none recorded`; no relevant registered claims uses the explicit zero-claim question and distinguishes legacy or unregistered prose. Confirmation does not churn versions, and an owner correction establishes the owner's meaning rather than factual truth. Every actual graph or claim change remains protected and substantively reviewed. A heavy garden always uses Deep TRACER and, independently, Protocol section 26's frozen-baseline three-lens semantic-conservation audit. Ordinary Challenge, passing validation, and getting below the 40,000-token context limit never replace that stronger bounded audit. A conserved result at or above the limit remains blocked rather than authorizing semantic pruning. Every semantic change still requires an owner answer; `No answer = no semantic change`.

## Work Ledger software-validation binding

The following requirements are copied from the integration directive and are operative for material software work. They state acceptance evidence, not permission to change requirements or external systems.

## Software development and validation

Where the integration requires material software changes, treat tests, linters, type checks, reproduction procedures, formal checks, and evals as evidence bearing on whether the implementation satisfies the intended product behavior. Do not treat them as the source of the requirement or as establishing more than their design, scope, execution environment, and results warrant.

A test may function as an authoritative executable specification when an authorized product, standards, or conformance process explicitly gives it that role. Its authority then derives from that process, not merely from the fact that the test exists.

Before a material behavior change, state concisely:

Required behavior and scope:
Source or reason for the requirement:
Acceptance criteria:
Validation standard: what evidence and residual risk are sufficient for completion?
Relevant existing tests or evals:
Repository-defined validation commands:

Identify the validation standard before using results to declare completion. The standard may be repository-defined or task-specific and need not be numerical. Do not relax it merely because the implementation or existing tests fail. Revise it only for a requirement-level reason, and record that reason.

Determine intended behavior from the best available owner instructions, product documentation, user-facing expectations, standards, and architecture. Existing code and tests are important evidence about current expectations, but they may be incomplete, stale, overspecified, environmentally dependent, or wrong. Use characterization tests when current behavior needs to be preserved or compared, but do not mistake characterization of existing behavior for a product requirement.

Assess separately:

whether the acceptance criteria adequately operationalize the required behavior within the relevant scope;
whether the tests and other validation methods are fit to evaluate those criteria under the stated validation standard, including the adequacy of their oracles, fixtures or mocks, execution environment, and coverage of material failure modes; and
whether the implementation passes the resulting validation package.

Passing validation is one premise in the completion judgment, not the whole judgment.

Use the smallest reliable validation loop while iterating, then run the broader applicable repository checks proportionate to the scope and risk of the change before completion. Follow repository-defined commands where available.

For a bug fix or newly specified behavior, add or update a focused regression test, eval case, or reproducible check. When practical, confirm that it fails before the fix and passes afterward. An already-existing check that reliably distinguishes the defective or missing behavior from the intended behavior may satisfy this requirement.

When direct automated validation is unsafe, infeasible, unavailable, or not meaningful, use the strongest repeatable alternative. State the remaining proof gap and compare it with the validation standard. If the gap exceeds what that standard permits, report the work as partially validated, blocked, or incomplete rather than successful.

Do not weaken, delete, skip, or rewrite a test merely because the implementation fails it. A test may be changed when the available product evidence shows that it is wrong, obsolete, overspecified, incomplete, or no longer aligned with an accepted requirement; record the requirement-level reason. When the code, test, and stated requirement conflict, determine which should change rather than automatically privileging either the code or the test.

Inspect the relevant diff and behavior, not merely the process exit code. Passing checks warrant only the claims those checks adequately evaluate. When reporting completion, state the scoped conclusion that the available evidence supports and any material residual uncertainty. Do not convert “the relevant checks passed under these conditions” into “the product is guaranteed correct.”

For nondeterministic LLM or agent behavior, supplement conventional tests with representative eval cases, explicit success criteria or rubrics, repeated trials where variability matters, and human, domain-expert, or product-owner calibration, as appropriate, where automated scoring is insufficient.

Report:

the checks and evals actually run and their results;
the scoped conclusion those results support;
relevant checks that were not run;
material untested risks or proof gaps and whether they remain acceptable under the validation standard; and
environmental or evidential limitations.

Do not claim more validation than the available evidence supports. Encode stable test commands and mechanically checkable invariants in repository-local guidance and enforcement rather than repeating them in every task prompt.

## Source-fidelity receipt

- Supplied attachment SHA-256: `35ea7afa15484733bd5183f8466512e7dff89fb9da4d9ddb0e2bc77e96c61184`.
- Copied Document (ii) body boundary: the nonblank body after `[BEGIN DOCUMENT (ii)]` through the nonblank body before `[END DOCUMENT (ii)]`.
- Normalized body representation: UTF-8 without BOM, LF line endings, one final LF.
- Copied Document (ii) body SHA-256: `9ce10219656f7e91816efe3f037562807c28b70f2a8260e6cacae3b5813753e1`.
- Formatting-only transformations: line endings normalized to LF; no wording, ordering, correction, insertion, or deletion inside the body delimiters.
- Semantic comparison disposition: exact normalized-body equality is required and is mechanically verified by the repository tests.

The Work Ledger binding material outside the delimiters is repository-authored integration text. Changing it or the copied body requires an explicitly authorized TRACER-maintenance task, exact clause comparison, and owner adoption.
