# AGENTS.md — Work Ledger MVP

This repository is a harness-neutral context ledger. Codex and Claude Code are
execution harnesses, not sources of truth or authority.

Use the Git top-level directory containing this file as the default repository
boundary described in `PROTOCOL.md`. Access outside it only when the user
explicitly names the exact external path for the active task; that does not
authorize adjacent discovery.
After the applicable startup gate, resolving an already-installed command
executable by the shared platform adapter's bounded metadata-only procedure
is permitted execution setup. It grants no access to external user/project
content, neighboring folders, or configuration changes.

For an explicit first-setup or readiness request, use the startup-safe card
below before repository inspection. Before the participant's complete direct
reply, make no repository Read, shell, Git, Agent, retrieval, external, Edit,
Write, or mutating call. Prepare values only from the participant's message or
explicit current session context, and use `not yet supplied` for unavailable
facts. Never infer account/organization from Git identity or a remote. Present
exactly, with only the bracketed prepared values substituted. When current
session context or direct participant attestation explicitly establishes them,
Codex uses `Codex Desktop (Local) on Windows` or `Codex Desktop (Local) on macOS`
and `OpenAI processes selected content under the account and organization
settings used for this workspace.` as its prepared workspace and provider lines.
Retain the attested OS across replies unless superseded or contradicted;
account/organization and local-save credit remain `not yet supplied` until the
owner supplies them:

    Quick setup: five choices

    Reply "recommended" to use all A choices, reply with letters such as
    "1A 2B 3A 4A 5A," or answer naturally. You can change these later.

    - **Workspace I will record:** <prepared value or not yet supplied>
    - **Account/organization label:** <prepared value or not yet supplied>
    - **Workspace permissions:** <prepared value or not yet supplied>
    - **Provider processing:** <prepared statement or not yet supplied>
    - **Local save credit:** <prepared name and email or not yet supplied>

    Your reply confirms these five lines as well as the choices below. If a line
    is wrong, include the correction in the same reply. If a line says
    "not yet supplied," supply it in this reply. Local save credit is the name
    and email recorded on local Git commits; it is not inferred from your
    provider account.

    **1. What kinds of files will you add?**

    - **A.** Work files already approved for this company AI workspace.
      Adding them means I may use and store them here. (Recommended)

    - **B.** A mix of work, personal, or client files. Ask once before each new group.

    - **C.** Not sure; start with the safeguards in B.

    **2. What should become reusable understanding?**

    - **A.** Stable goals, decisions, constraints, and open questions. (Recommended)

    - **B.** Broader useful summaries too.

    - **C.** Nothing reusable unless I approve specific items.

    **3. How detailed should source notes be?**

    - **A.** Balanced: key context with source links. (Recommended)

    - **B.** Lean: essentials only.

    - **C.** Detailed: preserve more background and nuance.

    **4. How should I communicate?**

    - **A.** Brief and nontechnical; handle workspace mechanics for me. (Recommended)

    - **B.** Plain language with short reasons for important choices.

    - **C.** Technical detail is welcome.

    **5. How should this workspace save setup, added files, and approved reusable understanding?**

    - **A. Automatic local saves.** Save setup when I confirm this card.
      Later, when I ask to add a specific file group, store that group. Save
      its reusable understanding or sources-only choice after my A/B/C reply.
      No separate saving or file-handling confirmation is needed. (Recommended)

      After the save succeeds and the stored copies are verified byte for byte,
      permanently delete only matching duplicate copies from the add-files
      folder. Move reviewed files not stored as sources into its
      reviewed-not-stored holding folder.

    - **B. Ask each time.** Ask before the setup checkpoint, each later source
      checkpoint, each permanent deletion of a verified duplicate intake copy,
      and each move of a reviewed-but-unstored file into the holding folder.

    - **C. I manage saving and file handling.** I will manage local Git saving
      and post-review intake handling myself. Do not stage, commit, move, or
      delete intake copies for me.

    Local saving details for A and B: each checkpoint is one unsigned local Git
    commit in this folder. Under A, my setup reply, later ingestion request, or
    semantic-review reply authorizes its respective checkpoint and the handling
    above. Under B, my separate approval authorizes the applicable checkpoint
    or handling. Git hooks and commit signing are disabled only for that commit
    invocation; no saved Git setting changes, and nothing is pushed or uploaded.

    Always true: the provider-processing line above describes where the selected
    content is processed. This setup does not authorize web, connectors,
    external actions, public sharing, or remote backup. I will preserve
    conflicts rather than guess, and I will ask once before making extracted
    understanding reusable.

`recommended` selects all A choices, confirms populated lines, acknowledges
provider processing, and accepts checkpoint contract v1. It does not fill a
`not yet supplied` line. Obtain every missing value in the same reply or one
compact no-tool follow-up. After a complete reply, load the detailed shared
procedure and complete every normal validation and recovery check before the
first mutation.

### Established-ledger startup gates

When the existing routing selects ordinary task initialization or bounded
read-only consultation, evaluate each gate's result before any dependent
command. Do not batch validation with ordinary current-view, manifest, source
or artifact reads. Use the exact prescribed platform forms; do not invent an
equivalent validator. The fresh-card route, exact native generation-zero
consultation exception, and frozen-reviewer route remain unchanged. Ordinary
mutable work requires trusted initialization; consultation uses Reference
section 2's bounded lane.

Perform the applicable checks in order:

1. Before any Git command, run section 15's exact active-harness redirector
   presence detector and reject every present Git redirector, including an
   empty or default-equivalent value. On Codex on Windows, use only section
   15's canonical PowerShell count form; do not improvise `Get-ChildItem Env:`,
   `Get-Item Env:`, `Test-Path Env:`, or `[Environment]` alternatives. Before
   any mutation intended for an assistant-created checkpoint, including
   meaningful dossier initialization, and again immediately before its commit,
   run section 15's separate four-variable identity-override detector.
2. Narrowly read and validate `current/tracer-state.json`.
3. Verify its ledger identity, active status, generation, and raw SHA-256
   binding to `current/claims.jsonl` without loading the whole register.
4. Inspect exact `HEAD`, staged paths, working-tree status, and the exact
   `caches/checkpoints/` receipt directory.
5. Treat a nonempty index; nonterminal, malformed, unknown, or conflicting
   checkpoint receipt; or unexplained dirty protected path as a continuation/
   recovery gate under section 29. Mutating preservation is permitted only
   when an authentic, internally consistent dossier and strict receipt plus
   applicable direct or saved authority admit it. Otherwise stop unchanged.
   Within the bounded read-only consultation lane, apply only its exact
   participant-named noncanonical-candidate exception or report the gate and
   stop without mutation. Never treat uncommitted protected state as
   authoritative.

A missing, malformed, inactive, identity-mismatched, or register-hash-mismatched
TRACER state blocks ordinary initialization and bounded read-only consultation. Say
`Ledger protocol loaded, but task initialization is incomplete: TRACER state or recovery is required.`
For example, if the stored and computed register hashes differ, give that
incomplete-initialization response and stop. Do not read ordinary current views,
try a `git show` fallback, summarize the workspace, or repair the binding.

The exact active native generation-zero state with null ledger ID permits no
ordinary mutable work other than first profile setup until the ID is bound; the
bounded read-only consultation exception remains available. A leftover retired transaction
pointer is recovery evidence and also blocks ordinary work; never delete or
guess it away.

Classify TRACER materiality and provisional Light/Standard/Deep mode before
applying the simple-task exemption. Standard or Deep is substantial. A material
Light task still carries the compact section-32 trace.

Outside the bounded read-only consultation lane, substantial work completes
trusted initialization before protected work.
It consists of the required canonical reads, a full read of
`dossiers/templates/task-dossier.md`, selection of the exact canonical path
under `dossiers/active/`, one low-noise visible update, creation or update of a
meaningful task dossier at that path, and a full reread after its final
initialization write. The update must be visible no later than the confirming
reread. A blank or unchanged template is not meaningful initialization.

An explicitly requested read-only consultation may instead use Reference
section 2's bounded lane. Perform its narrow read-only state/recovery gate, then
read only the exact routed material needed to answer. Create no dossier or
receipt; make no workspace mutation, recovery-preservation write, stage,
commit, durable adoption, canonical write, downstream/external action, or later
reliance as saved ledger memory; and never claim full initialization. It may
analyze and cite validated committed material in the current answer. A profile is validated when present; exact native generation-
zero/null-ID state without one remains consultation-eligible but grants no
setup/save authority. Exact participant-named dirty/staged candidate paths may
be read after a snapshot only as noncanonical review targets. Any other
recovery gate is reported and left unchanged.

Use `Ledger protocol active; initializing dossier: <path>.` by default. For a
confirmed `plain-brief` profile, or an explicitly requested clean setup/direct
ingest with no profile yet, use
`I'm preparing the ledger and opening a dossier for this update.` Record the
normalized dossier path and an immediately inspectable update receipt inside
the dossier.

A valid newly allocated dossier path uses forward slashes and is exactly
`dossiers/active/YYYY-MM-DD__<slug>.md`, using the real local task-start date,
a slug matching `[a-z0-9]+(?:-[a-z0-9]+)*`, and a complete filename no longer
than 120 characters. Reject an invalid calendar date, absolute path,
backslashes, empty/`.`/`..` segments, `.agents/`, and other prefixes. Preserve
an already initialized active dossier's exact previously validated path for
continuation/recovery and never normalize a committed historical path in place.

Outside the bounded read-only consultation lane, before initialization
completes, do not read manifest, source, intake-content,
artifact, or unrelated-dossier content; broadly scan the repository; perform
task-specific substantive analysis; or make a non-dossier task mutation. If
initialization cannot complete, say
`Ledger protocol loaded, but task initialization is incomplete: <reason>.`,
halt protected work, and do not imply success.

During trusted initialization, read:

- `PROTOCOL.md`
- exact `PROTOCOL-REFERENCE.md` sections routed by the core
- `current/context-pack.md`
- `current/decisions.md`
- `current/open-loops.md`
- `current/technical-preferences.md`
- `current/context-map.md` when routing source extracts or workstreams
- `current/operating-profile.json` when it exists
- `current/tracer-state.json`
- `dossiers/templates/task-dossier.md`

For first profile setup or profile renewal only, after the participant's
complete direct card/renewal reply and never before it, also read
`templates/operating-profile.example.json` in full as section 27's
nonauthoritative schema skeleton.

Operating rules:

1. Do not scan the repository broadly by default.
2. Outside the bounded read-only consultation lane, create, update, and confirm
   a meaningful task dossier before protected work.
3. Treat summaries as navigation aids, not sources of truth.
4. Cite source IDs or exact paths when relying on old material.
5. Apply the saved source mode. `contained` uses confirmed workspace authority;
   `separated` retains the GREEN/YELLOW/RED boundary.
6. Do not read a legacy `sources/pointers/` file unless explicitly instructed;
   new YELLOW pointers are metadata-only manifest rows, not separate files.
7. Record context insufficiency in the dossier, or in the final response for a
   bounded read-only consultation.
8. Update only current files whose meaning changed.
9. Follow section 15 for staging, commits, and publication. Before any
   assistant commit, require checkpoint contract v1 through the current chat or
   an exact valid ledger/profile/version/contract binding, then show the bounded
   checkpoint notice before staging. Review, audit, advice, and status work
   remain uncommitted unless the owner authorizes a checkpoint. Local-save
   authority never includes remote sync or publication. A renewed valid legacy
   ordinary-save record is not replaced until the renewal commit verifies; its
   ignored postcommit rebind must be receipt-bound and recovery-preserved.
10. Follow section 25 for external retrieval. Capability is not authority.
11. `Run the garden` invokes only section 26. Question 1 is the bounded TRACER
    claim-and-relationship card, including the zero-claim form.
12. For direct file adds, use only `add-files-here/`; exclude
    `reviewed-not-stored/` and never probe an older intake location.
13. Preserve an incomplete tree only when section 29's authentic-evidence and
    authority prerequisites admit mutating recovery; otherwise stop unchanged.
    Resume only when exact `HEAD`, staged tree, declared paths, and affected
    bytes match recorded state. Never use broad reset, clean, stash, amend,
    rebase, force, branch switching, remote mutation, or deletion of recovery
    evidence.
14. Tier 0 is the default. The ordinary checkpoint is: draft; reread;
    byte-check when warranted; verify exact dirt; establish the staged tree
    through the actor-appropriate route; verify the index/tree; save through
    the assistant-commit or 5C owner-handoff route; verify the commit. Under 5C
    the assistant never stages, unstages, or commits. Nothing is canonical
    before commit.
15. A protected claim delta captures one UTC-millisecond `sealed_at`, sets every
    appended row's `recorded_at` to it, and uses one actor-appropriate staged-
    tree seal: assistant-save starts from an empty index and stages exactly;
    5C uses only a read-only-verified owner-staged tree. Bind exact
    `base_head_oid`, `staged_tree_oid` from `git write-tree`,
    `sealed_at`, sorted
    `declared_paths`, add/modify/type-change/delete candidate entries, governing trace
    reference/hash/mode, rubric hash, reviewer identity, and the exact hashed
    review-material manifest. Dispatch the separate reviewer against that
    frozen candidate. Required pre/post snapshot bytes bind `HEAD`, index tree,
    declared changes, raw status, affected worktree bytes/types, and review
    materials. Any mismatch or observed mutation invalidates the review.
16. A non-accept preserves working files and appends its exact attempt to the
    strict receipt. With assistant-save authority, unstage only exact declared
    paths. Under 5C, enter blocked state and require the owner to unstage those
    exact paths, then verify the empty index read-only. One direct owner decision
    may consume one Deep non-accept for repair, fresh staging, and fresh review;
    a second blocks further revision in that checkpoint and requires owner-
    directed cancellation/rollback or maintainer recovery, never a bypass.
17. For Codex review, use a fresh reasoning context, request a read-only
    sandbox, compare byte-identical required snapshots, and monitor the runtime
    event surface actually available. A mismatch or observed mutating event
    invalidates the review. Repository policy cannot prove tool absence, and an
    equal end state cannot prove no transient mutation, so every
    `independence_note` discloses those limits plus shared model, prompt,
    evidence, and framing.
18. Apply `templates/claim-review-rubric.md` to every protected delta. Review
    evidence uses schema version 2 and repeats the exact frozen bindings plus
    the seven substantive fields in section 29. Preserve the exact response
    bytes by SHA-256 and base64. The exact final wrapper bytes, SHA-256, base
    OID, and tree OID are mandatory in the commit body; an ignored sidecar is
    only a convenience copy. Evidence is process evidence, not factual claim
    evidence.
19. Apply section 32 before consequential results/actions, canonical or durable
    writes, material source-state writes, and material reliance. Load all of
    `TRACER.md` for Standard/Deep, semantic canonical writes, ingestion
    adoption, software behavior, dependency revisit, garden claim changes, or
    TRACER maintenance. A truncated tool rendering or omitted range is not a
    complete read: measure the file and read bounded contiguous slices through
    EOF before relying or writing. A bounded read-only consultation puts its
    complete Standard/Deep trace in the final response as noncanonical,
    nondurable analysis.
20. Retrieve `current/claims.jsonl` selectively by exact claim, projection,
    dependency route, reverse dependent, material relation, or typed reference.
    Recheck generation and raw register SHA-256 before consequential action and
    final Establish.
21. An ordinary Participant checkpoint may contain only its initialized
    dossier, task-owned `artifacts/` files, and eligible current Markdown views
    named in section 29. If either committed or candidate operative text in a
    supported file contains a full projection or complete protected typed field
    and the bytes differ, route the whole file through protected review.
22. When section 24's concurrency-intent checkpoint applies, record request
    shaping before launching workers. The visible coordinator is the only
    stager, committer, and integrator. Workers are proposal-only for `current/`.

For an established ledger, the current task request permits read-only
validation and routing. A valid current profile does not repeat the setup card;
saved choices or authority apply only after exact ledger, profile, version,
contract, scope, and recovery bindings validate. Plain-brief means concise, not
concealed: show required choices, bounded checkpoint notices, meaningful
participant-actionable blockers, and results; summarize routine mechanics and
provide full detail on request.

For profile and qualification evidence, Codex Local's owner-facing standard
workspace-editing posture maps to exact `workspace-write`; record the prepared
value without asking the owner to interpret the technical spelling.

Parity invariant:

> For the same role and the same granted authority, Codex and Claude Code get
> the same editable paths, review obligations, retrieval and action authority,
> and saved outcome. Configuration syntax may differ; capability may not. A
> genuine harness limitation is disclosed and declines the affected action
> rather than claiming compliance with a weaker substitute.
