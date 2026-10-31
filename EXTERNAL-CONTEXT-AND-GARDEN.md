# External Context And Garden

**Candidate feature:** Work Ledger can govern external context exposed by a supported agent surface and can run a human-controlled internal garden. This repository does not contain an OAuth client, provider index, background service, or external-action engine.

Codex is the established connector-dogfood surface. Claude Desktop Code in a Local session may run the same staged qualification only after its fresh-start smoke, first ledger value, and exact Claude preflight; no Claude connector is prequalified by this package. Chat, Cowork, another Claude session type, another user's account, and local Claude CLI evidence do not automatically qualify the Desktop adapter.

The protocol is portable, but it is not a universal connector driver. Each adapter, account, agent surface, connector mechanism, and materially relevant version must pass its own capability gate and receive owner approval. Qualification of Gmail does not qualify Calendar, Notion, Slack, another user's account, or a later adapter whose mechanism, scopes, tools, indexing behavior, or revocation path changed.

## 1. Create a source-review profile

From a verified clean tree, start a fresh task in the selected supported surface and send:

```text
Create artifacts/source-review-profile.md from templates/source-review-profile.md and interview me to prepare a draft intent. Ask no more than three short questions per round. Use plain-language A/B/C choices with the recommended conservative option first wherever feasible; accept “default,” “not sure,” and “decide later.” Branch first between ad hoc only and considering recurring review later; skip schedule-only questions for ad hoc use. Ask me only for policy and intent. Mark scopes, indexing, tool/version details, write-tool inventory, permission behavior, coverage, and working paths “pending qualification.” Before marking the draft owner-confirmed, show my choices, inherited defaults, deferred items, the exact current/context-map.md route to this profile, and the next authorization boundary. After I confirm, write the draft and its exact active route as the only approved semantic operations. Do not install, connect, or read any external source during setup.
```

Creating the artifact inside the initialized task preserves a clean starting preflight. The owner-reviewed draft remains retrieval-disabled. It records the desired account labels, jobs, bounds, retention, no-action posture, expiry, and stop path, while technical facts remain pending. It becomes reusable only for exact qualification rows supported by observed adapter/account/surface/mechanism/version evidence and explicit owner activation. Future tasks resolve only the exact active path named by `current/context-map.md`; they never search `artifacts/` for a profile. Do not place secrets, account identifiers that should remain private, OAuth material, or raw source content in it.

## 2. Qualify one exact adapter and account

Qualification has two approvals before source content is read.

### Approval 1: installation, connection, and minimal verification

Before installing or connecting anything, the active supported Work Ledger assistant shows:

1. the exact adapter/tool, native/MCP-backed/plugin-backed connector mechanism, agent surface, and non-secret account label;
2. the intended jobs and expected source boundary;
3. expected permissions and the preferred connector-specific permission mode;
4. the exact installation/connection operations;
5. the minimal account-identity and capability check allowed after connection;
6. the stop/revoke path; and
7. success and no-go conditions.

The owner approves only those setup operations. This approval grants no search, message/event/file listing, or content access.

### Approval 2: bounded source-content run

After connection, the active supported Work Ledger assistant performs only the approved minimal identity/capability check. It then shows:

1. the verified agent surface, adapter/tool, connector mechanism and materially relevant version, non-secret account label, and repository reach;
2. actual provider scopes, indexing or synchronization behavior, coverage limits, and available write-capable tools;
3. whether read-only is provider-enforced or behaviorally enforced by not using write tools;
4. the source subset, purpose, selectors or exact item, dates or cursor, result cap, full-content cap, attachment rule, and sensitive exclusions;
5. the default ephemeral output and allowed memory dispositions;
6. any manual candidate hand-carry step if the retrieval surface cannot read the repository;
7. the stop/revoke path; and
8. the run's success and no-go conditions.

If the surface exposes connector-specific permission controls, use the narrowest mode that still permits the approved job. For a behaviorally read-only review, prefer a mode that allows reads but requires a fresh approval before any change, then verify that setting after it is applied. This is defense in depth, not provider-enforced read-only, and it does not authorize a draft, test event, label, or other external mutation merely to prove that the approval prompt exists.

For a first Claude Desktop qualification, keep every connector write-capable tool `Blocked` and every proposed read tool `Needs approval`. Record the exact displayed tool inventory and do not infer read versus write behavior from a tool name. The mechanism must leave `.claude/settings.json` unchanged and must not require `.mcp.json`, `enabledPlugins`, another `.claude/` child, or another project override; if it does, it is unsupported in this prerelease. A later permission change is itself a capability change that expires the affected qualification.

The owner must approve this second displayed card before source-content access. Editing the card approves only the edited bounds. Silence, prior connector use, a connected account, or Approval 1 is not content authority.

After the bounded no-action run, record the exact search and fetch paths that actually worked, the paths that failed, and the coverage caveats. Similar tool names or overlapping read aliases are not interchangeable evidence. The owner then chooses whether to activate that exact qualification row. Evidence never transfers to a different adapter, account, surface, connector mechanism, or materially relevant version. Enabling an approved connector never relaxes repository-root, retention, action, subagent, or one-writer boundaries.

## 3. Run an ad hoc question or review

A qualified row supports two triggers. A first qualification uses the two-approval sequence above, not the prompts below.

### Ad hoc task

Use this when there is a question now:

```text
Using the owner-confirmed profile at artifacts/source-review-profile.md, as routed by current/context-map.md, answer this question: <question>. Stop if the route and path do not match. Show any unresolved per-run variables and the capability gate before access. Use an exact item if I name one; otherwise use bounded discovery, shortlist by metadata, and fetch only the best supporting items. Keep the result ephemeral unless I choose what should survive. Take no external action.
```

### Retrospective review

Use this when the exact items may be unknown:

```text
Using the owner-confirmed profile at artifacts/source-review-profile.md, as routed by current/context-map.md, run the authorized review job for <purpose and window>. Stop if the route and path do not match. Show the capability gate before access. Return at most the profile's candidate cap with locators and coverage caveats. Do not update the ledger or take external action until I accept specific candidates.
```

A standing schedule is optional and should be considered only after manual runs are useful and predictable. Its approved delivery destination may be an external digest or an ephemeral in-surface result; neither is durable ledger state.

Standing or scheduled review authority covers bounded retrieval and candidate synthesis only. It never authorizes durable memory, repository mutation, or external action. This is true even when the adapter can read or write the repository. Every candidate remains ephemeral until the owner accepts that specific candidate and memory disposition in a later interactive task. If a scheduler cannot read the repository, it may deliver its digest on the approved scheduling surface; copying that digest into the ledger is a separate reviewed operation.

## 4. Choose what survives

Retrieval, memory, and action are separate:

| Choice | What it means |
| --- | --- |
| Ephemeral | Use the live evidence for this answer or review, then retain no item-level record. This is the default. |
| Minimal receipt | Retain only the smallest provenance needed for an accepted consequential claim. |
| Tracked pointer | Retain safe metadata and a handle for a later separately authorized re-read; no source body is stored. |
| Governed snapshot | Preserve eligible historical evidence through ordinary guarded intake and provenance rules. |
| Adopted conclusion | Record a concise, human-reviewed current fact, decision, preference, or open loop without mirroring the upstream item. |

An external create, edit, send, label, move, or delete is never one of these memory choices. It requires a separate exact preview and approval, and external action defaults to `none`.

## 5. Run the garden

Start a fresh task and say:

```text
Run the garden.
```

That phrase authorizes only the internal ledger scout. Classify the run before
inspection. Measure the exact Protocol section-7 joined startup corpus with the
pinned published `o200k_base` tokenizer. It is heavy at 40,000 measured tokens
or after a documented consequential mandatory-context failure. If exact
tokenization required to determine cap compliance cannot run, leave that gate
incomplete; a word or byte count cannot decide whether the corpus is above or
below the cap or make a candidate adoptable. A documented consequential failure
still selects heavy mode. The routine
byte warning is only the threshold derived from the post-split corpus at 36,000
tokens. It prompts exact measurement and is never the limit. Routine and heavy
runs may return up to eight
short, evidence-routed questions per reviewable batch about decisions,
unreported events, staleness or contradictions, and safe compression or
routing. The first garden question, question 1, always presents a bounded TRACER card for owner confirmation
or correction: exact included latest claims, assessments, and retrieval/coverage limits; load-bearing
dependencies, reverse dependents, conflicts, identity/equivalence,
supersession/reassessment, other material relations, `none recorded` categories,
and suspected gaps or misrepresentation. If there are zero relevant registered
claims, it says so, distinguishes legacy or unregistered prose, and asks whether
that absence is expected. The card counts within the eight and
must say `No answer = no semantic change`. Confirmation alone need not create a
new version; an actual claim or relationship change uses the protected
staged-tree procedure and substantive review.

Immediately after the claim card, check workstream staleness through a bounded
metadata/field search. Dossier declaration remains deliberately permissive. A
row is stale only when a declaring dossier has an exact `complete` UTC-millisecond
status later than the row's exact `Last reviewed` timestamp, records nonempty
material impact on its status, next action, routes, or claims, and the row does
not reflect that effect. Mere declaration,
consultation, or mechanical work does not fire the check. When several rows are
stale, combine them into one numbered question when useful.

A heavy run uses Deep TRACER and, independently, freezes the complete pre-edit
baseline, preserves the accepted answer map, and completes all three section-26
semantic-conservation lenses, affected reruns, route/retrieval checks, and the
unconditional final whole-candidate audit. Validation, worker agreement, or
getting below the 40,000-token context limit never substitutes for that audit or
owner adoption. A conserved result at or above the limit remains blocked rather
than authorizing semantic pruning. Use `templates/garden-prompt.md` and, when heavy,
`templates/heavy-garden-review.md`.

The garden may read the garden-control section of `artifacts/ledger-setup-profile.md` only when `current/context-map.md` names that exact active profile. On a repeat run, it reads a prior accepted garden record only when the context map names its exact path. If either route is absent, the record is treated as absent; the garden does not search dossiers or artifacts to find one.

If a separately authorized external review already produced an agenda, provide it explicitly:

```text
Run the garden. Also consider these separately authorized external-review candidates as ephemeral input: <paste the normalized candidates, or name one exact already-governed internal artifact>. Do not launch another external review.
```

Do not copy raw external output into the repository merely to hand it to the garden. If the owner explicitly names one outside-root file, access remains limited to that exact path under the root adapter, and its content remains untrusted ephemeral input. The garden deduplicates internal and external candidates but preserves their different authority. It does not change durable state until the owner answers. Before editing, it shows the accepted-answer-to-path mapping; after editing, it validates and reports the exact diff.

## 6. Optional reminder-only schedule

`templates/garden-prompt.md` contains a safe reminder and the interactive instructions. The unattended occurrence must stop after the reminder. It must not inspect the repository, initialize a dossier, access an external source, or prepare an agenda.

Scheduling is a user/surface capability, not repository-shipped authority and
not evidence that a project-attached task exists. Configure the reminder only
on a surface that can reliably stop after delivery. A human calendar reminder
is an equivalent fallback.

Quiet controls for any later external review are explicit: `skip once`, `snooze until <date>`, `pause profile`, `disable <source/job>`, `run now within profile`, and `review profile`. A missed run never silently expands the next lookback.

## 7. Stop and revoke

The profile's stop procedure should cover, as applicable:

1. pause any standing job;
2. mark the exact qualification row disabled or expired;
3. disconnect the connector or narrow its permissions;
4. verify that the formerly qualified path no longer runs; and
5. preserve the rule that a tracked pointer never grants future access.

Revocation does not require deleting valid historical ledger conclusions. It does end future retrieval authority.

## 8. Continuity with public web research

A bounded public-web task requested by the owner is the public-source instance of the same retrieval/memory/action model. It does not need a reusable private-source profile when the task, public source boundary, and purpose are clear. Its answer remains ephemeral by default, any durable conclusion still requires ordinary human-reviewed promotion, and any external action remains separate.

Authenticated or private web access and standing public-web reviews use the full profile and qualification controls above.
