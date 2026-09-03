# Migrate An Existing Ledger

Use this guide only for a maintainer-assisted upgrade of a healthy ledger that
will keep its existing Git lineage. It is not a self-service overlay recipe:
the maintainer must first supply an exact frozen v1 candidate whose source
commit/tree, manifest, paths, and hashes have passed the release gate. Do not
copy starter-ZIP files over an existing ledger. A fresh participant rebuild is
a different route described below.

Existing sources, manifest rows, extracts, dossiers, decisions, current
context, technical preferences, claims, TRACER state, and Git history remain
valid. Migration is prospective: do not reingest sources, mass-assign claim
IDs, replay historical chats, compress current state merely for migration, or
describe pre-cutover material as TRACER-validated.

## Pre-activation legacy receipt archive

Do this before applying any v1 governance or adapter byte. It is a bounded
human/maintainer-terminal cutover, not an assistant checkpoint and not a route
covered by the v1 Desktop permission profile. First finish every authorized
prior-protocol checkpoint and close the assistant task. The last such commit
may create one final legacy receipt; include it in the archive below. No further
prior-protocol assistant save occurs afterward, which breaks the otherwise
circular requirement to archive the receipt created while recording the
archive.

Older ledgers may have ignored `caches/checkpoints/*.json` receipts whose shapes
are not the new closed schema and may retain the prior protocol's exact ignored
scratch file `caches/commit-message.txt`. Against the exact last prior-protocol
HEAD, inventory every direct checkpoint child plus that one exact scratch path
when present, including byte count and raw SHA-256. Require `caches/`, the
checkpoint parent when present, and the legacy-archive parent to be real in-root
directories, not links/reparse points. Every receipt must be one direct regular
non-link/non-reparse file with a portable safe unique `.json` leaf and must have
provable prior-format terminal success/Git binding. The optional scratch file
must be one regular non-link/non-reparse file at that exact path; do not parse or
adopt its bytes under the new receipt rules. Any extra checkpoint entry, unsafe
leaf, nonterminal receipt, ambiguity, conflict, or invalid type blocks the
migration unchanged.

When at least one receipt or the scratch file exists, explicit owner approval of
this exact terminal cutover permits creating one absent ignored
`caches/legacy-checkpoints/pre-v026-YYYYMMDDTHHmmssfffZ/` directory, deriving the
filename-safe suffix from one captured UTC-millisecond timestamp. Before moving
anything, write and raw-hash a BOM-free UTF-8/LF `archive-plan.json` there. It
binds the prior HEAD, archive root, timestamp, and the complete sorted
kind/old-path/new-path/byte-count/raw-SHA-256 entry list. A receipt's destination
retains its unique `.json` leaf. The scratch destination is the fixed distinct
leaf `legacy-commit-message.txt`. Every destination must be absent. Move each
listed file literally and individually without overwrite, then verify source
absence, destination regular-file type, and byte/hash identity. On interruption,
resume only when the exact union of source and destination paths matches the
immutable plan and every present byte matches; otherwise stop without another
move.

`archive-plan.json` is one strict JSON object with no duplicate, missing, or
extra key and exact property order `schema_version`, `kind`, `prior_head_oid`,
`archive_root`, `captured_at`, `entries`. Require integer `schema_version: 1`,
exact `kind: work-ledger-pre-v026-archive-plan`, the full lowercase prior-HEAD
OID in the repository object format, the exact archive-root path, and strict
UTC-millisecond `captured_at`. `entries` is a nonempty array sorted uniquely by
`source_path` using ordinal UTF-8 bytes. Every entry has exact property order
`kind`, `source_path`, `destination_path`, `bytes`, `raw_sha256`; kind is
`receipt` or `scratch`, paths are the exact validated forward-slash relative
paths above, bytes is a nonnegative integer, and the hash is 64 lowercase hex.
The kind/path/destination cross-fields must agree with the receipt-preserved-leaf
or fixed-scratch-leaf rule above.

After all moves verify, active `caches/checkpoints/` is empty, and
`caches/commit-message.txt` is absent, write once a BOM-free UTF-8/LF
`archive-manifest.json` beside the plan, binding the plan hash, prior HEAD,
completion time, identical entry list, and successful source/destination
checks. Hash it and retain both ignored files. Never delete a receipt or scratch
file. If neither a receipt nor the scratch file exists, make no archive directory
and treat the later adopted inventory as explicitly empty for both classes.

`archive-manifest.json` is one strict JSON object with no duplicate, missing, or
extra key and exact property order `schema_version`, `kind`, `plan_path`,
`plan_sha256`, `prior_head_oid`, `archive_root`, `completed_at`, `entries`,
`sources_absent`, `destinations_verified`. Require integer `schema_version: 1`,
exact `kind: work-ledger-pre-v026-archive-manifest`, exact plan path and
64-lowercase-hex raw plan hash, the plan's exact prior HEAD and archive root,
strict UTC-millisecond completion time, an entry array deeply identical to the
plan's array, and exact JSON booleans `true` for both final checks. Serialize
both documents as BOM-free UTF-8 with LF only and exactly one final LF. Once the
plan is hashed, never rewrite it; once the manifest is hashed, never rewrite it.

The human maintainer then applies and manually commits only the exact already-
reviewed, manifest-bound v1 product bytes. That exceptional commit contains
no source, claim, profile, current-state, active-dossier, or other participant
content and creates no prior- or new-schema receipt. Verify its parent, entire
path delta, blobs, tree, and message against the frozen cutover candidate. Once
those bytes are active, the first strict v1 migration checkpoint records
the archive plan/manifest paths and hashes (or the proven empty inventory) in
its migration dossier. Immediately before its first mutation, revalidate that
each named plan/manifest is the same regular non-link/non-reparse file at the
same safe ignored path, that its raw hash and bound prior-HEAD/archive identity
match, and that the complete source/destination union still reconciles to the
recorded entry list; an empty inventory must be reproved against the same
cutover baseline. Until that checkpoint commits, the ignored manifest is
recovery evidence, not canonical history.

## In-place healthy-ledger upgrade

1. Before any Git command, reject every present section-15 Git redirector,
   including an empty or default-equivalent value. Then finish or preserve all
   active work. Require the expected repository, branch, clean index, and no
   ambiguous protected dirt. Run Reference section 27's exact non-shallow check
   and sole-root oracle; a shallow repository or anything other than one full
   lowercase object-format root OID blocks migration unchanged.
2. Validate current/tracer-state.json and the raw SHA-256 of
   current/claims.jsonl. Preserve activation, ledger identity, generation,
   register hash, and native/migrated cutover metadata.
3. Review the product/governance update as one isolated complete candidate.
   Account for every prior guarantee family before retiring old transaction
   scripts.
4. Apply and locally commit any separately authorized protected current-state
   adoption through the ledger's still-qualified prior save route; retain an old
   helper and its trust surfaces only when that ledger actually has one. A clean
   no-protected-delta no-scripts ledger skips this step. When used, this is an
   explicit transition checkpoint and contains no new governance, adapter,
   rubric, tool, test, or configuration bytes. Complete it before the terminal
   archive; its terminal receipt is part of the archive inventory.
5. Perform the human-terminal archive and exact manual product-cutover commit
   above. It contains no protected claim surface. Retire the old transaction
   helpers and tests, active-transaction-pointer grammar, and marker state only
   after the protected cutover is verified with no retired active transaction
   pointer. This does not authorize deleting or rewriting legacy source pointer
   rows or files; preserve those under the legacy source rules below.
6. Under active v1, use the first strict migration checkpoint to adopt the
   archive manifest evidence, renew the profile/contract when needed, and record
   the migration dossier without combining unrelated work.
7. Verify final HEAD, state generation/hash, register bytes, projections,
   references, index/worktree, and absence of a retired active pointer.
8. Treat the new decision as locally operative only when the cutover and strict
   migration checkpoint verify, then use Tier 0 for the bounded local pilot/soak. Release qualification remains a
   later gate.

A leftover caches/transactions/active.json after the cutover is recovery
evidence. Preserve it and stop for maintainer recovery; never delete it merely
because the new protocol no longer creates one.

## Claude Desktop local-policy upgrade

Close Claude Desktop before changing local permission settings. If
`.claude/settings.local.json` already exists and is not byte-identical to the
v1 tracked template, never overwrite or silently merge it. First copy its
exact bytes to an owner-chosen recoverable location outside this ledger, or to
an ignored `caches/manual-settings-backup/` path, and record where the backup
is. Then have the owner compare the old file with
`.claude/policies/desktop-windows-standard.settings-local.example.json` and
explicitly choose whether to replace it. The assistant does not infer that
choice from this guide. A supported replacement is byte-identical to the
tracked template and happens while Desktop is closed, before a new task opens.
Retain the backup until the migrated ledger passes its acceptance checks.

For 5A, 5B, or any other assistant-created commit, checkpoint contract v1 also
requires an explicit repository-local Git identity, even when a global identity
would otherwise be effective. With Desktop closed,
run `git config --local user.name` and `git config --local user.email` in the
exact ledger root. If either is blank or not the intended local-save credit, the
owner sets the intended repository-local values before opening the renewal task,
using the commands and substitution pattern in `START-HERE.md`. The renewal card
must name those same values. The assistant validates but never guesses or changes
them. Under 5C the owner manages Git identity and saving, so this local-config
prerequisite does not block a no-commit migration draft.

## Profile upgrade

Only a schema-1 profile that first passes Reference section 27's closed legacy
validator is eligible for renewal. Schema-1 profiles and profiles without
`checkpoint_contract_version: 1` cannot authorize a v1 assistant commit.
Preserve the ledger ID, profile ID, claim IDs/generation, source IDs, history,
and all prior snapshots. Increment the profile version once and create the
matching immutable snapshot; never regenerate those identities. A malformed,
identity-mismatched, non-off-remote, snapshot-mismatched, or lineage-mismatched
legacy profile blocks renewal without rewriting its bytes.

Schema 2 stores all five exact setup codes in `setup_choices` as well as their
consistent operational values. Reconstruct a code only from an exact valid
legacy value. A legacy `contained` source mode maps to 1A. A legacy `separated`
mode cannot distinguish 1B from 1C, so the owner must include exactly 1B or 1C
in the same renewal reply; never guess. Other valid legacy operational values
map uniquely through Reference section 27. Any unknown or inconsistent value
blocks renewal.

For an old 5A or 5B profile, show one combined renewal instead of a profile ask
followed by a separate commit ask:

    Your saved local-save choices predate checkpoint contract v1. Under v1,
    each assistant save is one unsigned local Git commit; hooks and signing are
    disabled for that commit only; no saved Git setting changes; nothing is pushed or
    uploaded. Your recorded source/setup choice is <5A|5B>, and completed-task
    automatic save is <on|not previously granted>. If it is on and you renew it,
    its local authority record is rebound only after this checkpoint verifies.
    Reply `RENEW LOCAL CHECKPOINT AUTHORITY` to keep
    exactly those choices under v1 and authorize this one profile-renewal
    checkpoint, or state changes. Choose manual saving if hooks or signed
    commits are required.

For an old `separated` profile append to that same disclosure: `Your old
profile does not record whether separated source handling was 1B or 1C. Include
1B or 1C with the renewal phrase.` This is part of the one combined ask.

No reply or a decline makes no profile, authority, staging, or commit change.
If the owner states changes instead of the exact renewal phrase, restate the
corrected choices and contract and wait for exact `RENEW LOCAL CHECKPOINT
AUTHORITY`. A correction by itself authorizes no write or checkpoint.
A valid v0.2.5 task-save record is a plain JSON object with exactly matching
`ledger_id`, `profile_id`, and positive `profile_version` and no other property.
The chat renewal itself supplies authority for the renewal checkpoint. When the
valid old record's `on` state was displayed and renewed, bind its raw hash and
the deterministic intended current-record hash in the drafting receipt's
`authority_rebind`. The new record uses the new profile version, the renewal
confirmation time, and exact `RENEW LOCAL CHECKPOINT AUTHORITY`, which is the
phrase the owner actually supplied. Keep the old record byte-identical until the
renewal commit fully verifies. Then preserve it in the required recovery event,
replace and verify it as the receipt's one postcommit authority rebind, and only
then complete the receipt. If it did not exist, do not invent it; the ordinary
save phrase remains necessary later. Cancellation before commit leaves the old
record unchanged. Interruption after commit leaves the receipt nonterminal and
the old bytes recoverable; no stale, partial, or unbound replacement grants
authority.

An old 5C profile remains manual for every assistant Git operation. Leave any
old task-save token untouched but inapplicable; it cannot override 5C. Require
a new direct current-contract choice before any assistant commit. For a 5C
draft, do not stage or commit it: leave one `drafting` receipt, give section
23's exact owner-managed handoff, and resume only through its exact owner-commit
recovery oracle.

When other profile facts are missing or stale, prefill only owner-attested
recorded facts and mark unavailable facts `not yet supplied`. The owner confirms
or corrects them directly, including harness, account/organization, provider
processing, local-save identity, and contract v1. Save the profile, immutable
snapshot, and dossier only through the ordinary Tier 0 checkpoint and its
bounded notice.

The profile governs future ingestion. It does not retroactively reclassify
legacy GREEN/YELLOW/RED rows or legacy pointer rows/files. New direct ingestion
uses the v1 metadata-only manifest-row pointer and creates no pointer file.

## Prospective claim use

Keep existing current files and claim projections in place. Whole-file
protection remains: a byte change to a supported file whose committed or
candidate text contains an operative projection or complete protected typed
field uses the staged-tree claim review.

When an older proposition later becomes load-bearing, review the best permitted
original evidence and add only the smallest linked claim, projection, or typed
reference needed for reliable use. Do not create a claim merely to backfill
history.

Every protected commit retains raw register SHA-256 and increments claim
generation exactly once, including a protected zero-row surface change.

## Fresh rebuild with historical references

Use a fresh rebuild when the old installation should remain untouched and the
new ledger intentionally begins a new native lineage.

1. Install the qualified neutral starter in a new folder.
2. Remove the starter origin or record the participant's future private remote
   locally. Do not push as part of rebuilding.
3. Run first profile setup and bind the new ledger ID.
4. Confirm native generation 0, empty-register SHA-256, no migrated baseline or
   adoption reference, and no retired transaction pointer.
5. Complete one ordinary initial two-phase ingestion from the participant's
   deliberately supplied initial files, including its semantic review and
   local checkpoint. Do not mix historical-ledger task files into this group.
6. Inventory only the exact participant-approved historical task files from the old ledger.
   Check regular-file/link status, byte length, raw SHA-256, original relative
   path, and protected-looking syntax. Before presenting the copy map, require
   every destination to be a forward-slash relative path beneath the one import
   root and every dynamic segment to satisfy the Desktop adapter's exact closed
   Windows command-safe ASCII grammar
   `^(?!.*\.\.)[A-Za-z0-9][A-Za-z0-9 ._()-]{0,119}$`: no empty, `.` or `..`
   segment; no leading hyphen; and no trailing space or period.
   Case-insensitively reject a segment whose whole name or the portion before
   its first period is a Windows reserved device name: `CON`, `PRN`, `AUX`,
   `NUL`, `COM1` through `COM9`, or `LPT1` through `LPT9`; also reject
   `.gitkeep`, every section-28 noise name, and, case-insensitively, the
   permission-reserved substrings ` -Force` and ` -Recurse`. The regex excludes
   dollar signs, backticks, quotes, colons, slash/backslash within a segment,
   wildcard/metacharacters, and control characters. If the original relative path
   cannot be retained under that grammar, stop before copying and use a
   separately qualified maintainer harness; never silently rename it.
7. Before copying or writing anything, allocate one section-23 checkpoint ID;
   initialize and fully reread a reconciliation dossier that declares every
   knowable import, README, inventory, dossier, and proposed current path; then
   create and validate its `drafting` receipt. Use exact current-chat
   `maintenance` authority for an assistant save or the validated 5C owner-
   managed route. Do not treat ordinary-task save authority as import authority.
8. On the supported Claude Desktop narrow-policy route, Claude does not issue
   an external-source copy or invent broad filesystem permission. It presents
   the exact approved source-to-destination inventory and waits while the owner
   or maintainer manually installs only those bytes beneath
   `imported-legacy/<owner-and-date>/`. A different harness may facilitate this
   mechanical step only after its exact external paths and copy primitives are
   separately qualified. In either route, revalidate the complete source and
   destination inventories, every existing destination ancestor as a real in-
   root non-link/non-reparse directory, regular file types, byte lengths, and
   raw hashes before accepting the copy boundary; any mismatch stops.
9. Preserve exact bytes under
   imported-legacy/<owner-and-date>/{dossiers,artifacts}/, retaining original
   relative paths beneath the matching inert category. Add a README and
   inventory declaring them historical references—not sources, active
   dossiers, operative artifacts, current state, claim surfaces, or native history.
10. Through that initialized dossier, draft proposed current state, but the
   participant is the sole semantic adopter. A
   maintainer may facilitate mechanics without becoming a second semantic
   approver.
11. Reread and validate the complete declared candidate. Apply protected review
    to any semantic current/claim surface, save through the actor-appropriate
    section-23 route, and verify profile, state/hash, commit, and clean tree. Do
    not push unless separately authorized.

Never copy an old current/, profile, claims register, state file, active dossier
tree, tool, or transaction cache wholesale into the fresh ledger.

## Retired intake location

intake/drop-verified/ remains retired and is not a compatibility input. Review
any local-only files there before a human removes the old folder. Move only
files deliberately intended as a new group into add-files-here/. The assistant
must not read, move, or delete files from the retired location automatically.

## Context gate and remote boundary

After migration, run exact joined-corpus o200k_base measurement. The canonical
limit remains strictly below 40,000 tokens. A byte warning is derived from the
post-split corpus and triggers exact measurement; it is not the limit. If a
semantically conserved candidate cannot pass, report the blocked over-limit
state rather than pruning meaning.

Local save and remote synchronization remain separate. remote_sync.mode: off
blocks helper/agent automation, not an exact owner-directed push. Use
SYNC-BETWEEN-DEVICES.md for a separately authorized device handoff.
