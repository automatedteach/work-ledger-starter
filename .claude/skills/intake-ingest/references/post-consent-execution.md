# Claude Post-Consent Work Ledger Procedure

## Loading gate

Load this file only after either:

- a complete direct reply to the current-chat first-setup card; or
- a participant's current task request that presupposes an established ledger.

Loading grants no action authority. For first setup, the card reply supplies
only the choices and actions it explicitly confirms. For an established
ledger, the current request permits validation and routing. A saved 5A profile
supplies only its selected automatic mode within the participant's direct
ingestion request or semantic-review reply; it is not current-task authority by
itself. Any other saved authority applies only after its exact ledger ID,
profile ID, profile version, scope, checkpoint-contract version, and current
recovery state validate.

When the applicable entry route below directs it, read
`.agents/skills/intake-ingest/SKILL.md` completely, then `PROTOCOL.md` and only
the `PROTOCOL-REFERENCE.md` sections routed by the core and active task. Those
files are the canonical shared procedure. This file supplies Claude-specific
execution shapes and sequencing only; it adds no alternate source, claim,
save, recovery, retrieval, publication, or external-action authority. The
`.claude` adapter and `.agents` canonical skill are intentional layers, not
competing installations.

Use dependent operations serially: receive and assess each tool result before
issuing the next dependent call. Only independent reads explicitly allowed by
the canonical procedure may share one assistant turn. Never issue a mutation
beside a validation on which it depends.

## Platform and local-policy gate

After the loading/card gate, establish the execution platform from explicit
current-session OS metadata or direct participant attestation already in this
conversation, before ledger-data/state reads, policy validation, commands,
Agent calls or mutations. Retain the attestation across replies unless
superseded or contradicted. Never infer OS from shell choice or a settings file.
If unknown/conflicting, ask only for platform clarification without tools.
Linux is outside this desktop route; stop without activating either template.

On Windows select
`.claude/policies/desktop-windows-standard.settings-local.example.json`.
On macOS select
`.claude/policies/desktop-macos-standard.settings-local.example.json`.
Use native Read to compare only the selected template and
`.claude/settings.local.json` before any other project read/tool action.

Perform this pre-command comparison with complete native Read results and
reasoning: check JSON syntax, duplicate keys and every setting/ordered entry.
Do not launch a JSON parser, Python, Node, PowerShell validation code or another
shell command for this gate. If the complete comparison cannot be validated,
stop unchanged using the correction below; do not guess or request broader
permission.

The active file must be valid JSON and match the selected template's complete
settings and ordered permission arrays, with no added/removed/changed entry.
A bare `Bash`, `Bash(*)`, `PowerShell` or `PowerShell(*)` allow is invalid.
File equality proves only those local bytes. Permission arrays can merge with
project/user/managed settings; actual effective behavior requires positive
zero-dialog evidence and the bounded unlisted-command control.

On missing/malformed/different active policy, stop before every command or
mutation. Give the applicable correction:

> Claude Desktop setup is incomplete, so I have not run a command or changed a
> file. Close this task. In this ledger folder, run the one-time command in
> START-HERE.md using PowerShell on Windows or Terminal on Mac. If
> `.claude/settings.local.json` already exists, leave it unchanged and ask for
> help comparing it. Reopen this exact folder, confirm **Accept edits**, and
> start a new task.

The owner activates the profile before first opening the folder; never rely on
a mid-task reload. Shared settings alone do not replace this gate. Once the
selected platform/policy is established, continue the applicable entry route.
For Mac, load the complete shared
`.agents/skills/intake-ingest/references/macos-primitives.md` before commands.

## Entry routes

### Fresh setup after card

The project startup Skill routes a complete current-chat setup-card reply to
`references/fresh-setup-execution.md`. That concise reference is the sole
Claude-specific fresh-setup execution route. This all-workflows reference does
not supply a second fresh-setup algorithm. When choice 5C requires the exact
owner handoff, or the fresh reference names an exact Windows command-shape
paragraph below, load only that named material.

### Owner-managed 5C handoff and resume

After candidate validation, classify whether section 29 requires protected
review and show the exact declared paths. For every candidate, use section 23's
exact owner-staging handoff, leave the receipt `drafting`, and stop. Only after
the participant reports staging and the exact staged tree is read-only verified
and recorded may an unprotected owner-commit handoff or protected review begin.
Prepare/hash the exact commit message and bind its path/hash at the point
section 23 requires; 5C never waives message or protected-review evidence.

For a participant-reported staged set, enter recovery and use only
read-only checks to verify the complete index, modes/blobs, worktree bytes/
types, base, and intended states. On an exact match, transition to `staged` and
for unprotected work produce section 23's exact owner-commit handoff. For
protected work, run section 29 review without changing the tree. Only an
accepted exact review may transition to `reviewed` and produce its owner-commit
handoff. A nonaccept appends the exact attempt, enters `blocked`, and uses the
owner-managed one-repair route; the assistant never unstages for 5C.

After either owner-commit handoff, enter recovery when the participant reports
saving. Apply section 23's exact actor-appropriate oracle, including prior
accepted-tree evidence for protected work and the bound committed message for
every owner commit. Run exact
`git --no-replace-objects rev-list --parents -n 1 HEAD` and require exactly two
space-separated full lowercase OIDs in the repository object format: the first
equals current `HEAD` and the second equals the recorded base. Then require the
exact complete committed path/tree/bytes, empty index, and
empty complete porcelain worktree status. Run the exact four-line HEAD author/
committer query and require every line to match the owner-attested local-save
credit. Transition to `committed`; complete
only after every applicable post-commit action or explicit defer/decline and
final count is recorded. Do not continue to a dependent phase before that.
Any mismatch or ambiguous history stops for maintainer recovery. Never stage,
unstage, amend, rewrite, or repair the owner's Git state.

### Established ledger

Complete the platform and local-policy gate. Then complete canonical loading and full exact
state/profile/recovery binding before applying saved choices or authority. Do
not repeat the setup card for a valid confirmed profile. A stale, malformed, or
mismatched profile or authority record never enlarges authority. For 5A
ingestion, still require the participant's applicable direct ingestion request
or semantic-review reply before any edit, checkpoint, or intake handling. An
old schema-1 5A or 5B choice lacking checkpoint contract v1 receives one combined
disclosure and renewal; do not split it into two asks. Declined or stale records
remain untouched. When exact old ordinary-save authority is renewed, bind its
prior and intended hashes in the strict receipt, keep it untouched through
commit verification, then perform only section 23's recovery-preserved
postcommit authority rebind before completing the receipt. An old 5C choice
remains manual. Ordinary task save still
uses section 29's separate exact phrase once per valid ledger/profile binding,
except that a current 5C choice makes that phrase inapplicable until a direct
profile revision changes the choice.

For an explicit bounded read-only consultation, use the canonical consultation
lane. Useful analysis is allowed only after the safety state needed for that
consultation validates, with no dossier, profile, artifact, receipt, staging,
commit, durable adoption, canonical write, downstream/external action, later
reliance as saved ledger memory, or false initialized claim. It may analyze and
cite validated committed material in the current answer. A recovery gate stops
affected reliance truthfully and remains untouched.

## Checkpoint notice and contract

Before every checkpoint's staging begins, show a bounded notice containing the
exact sorted paths or a bounded diff, operation `one local checkpoint`, exact
proposed commit subject and concise body or purpose, and why the save is needed.
Checkpoint contract v1 means the commit is local and unsigned, hooks and signing
are disabled only for that invocation, no saved Git configuration changes, and
no push or upload occurs. Repeat those contract details only when the contract
version changes or the participant asks. Under 5A or valid ordinary-save
authority this is a notice, not a second approval; 5B asks; 5C performs no Git
mutation. Full technical detail remains available on request.

## Platform operation map

The ordered algorithms below are shared. On Windows use the displayed Windows
command forms unchanged. On macOS use the complete shared
`.agents/skills/intake-ingest/references/macos-primitives.md` for the same
operation, path family, precondition and result obligation. Do not run a
PowerShell form on Mac or substitute GNU Windows utility syntax.

The map applies throughout receipt creation/transitions, profile setup,
ingestion, owner-managed handoffs, protected review, recovery and post-commit
verification. Strict Get-Item maps to native stat; missing-tolerant Get-Item to
separate test -e and test -L; directory creation/listing to mkdir/ls;
copy/move/delete to cp -n/mv -n/rm; raw hashing to shasum; GUIDs to uuidgen;
UTC/local dates, environment counters, byte encoding and committed-message
verification to their exact named appendix forms. Keep finite Git forms and
their options unchanged. Mac file operands use quoted ./ prefixes; actual
wildcards remain forbidden. The existing Windows path/name grammar and closed
receipt schema remain in force. The active Mac message oracle measures N from
the already-bound live message. Its historical-complete-receipt oracle derives
N from the immutable formatted stream's byte count minus one. Neither adds a
receipt field.

## Windows platform and stable command shapes

Claude ordinarily uses PowerShell on Windows and Bash on macOS/Linux. This
Windows Desktop profile uses Git Bash only for the exact analyzer-safe
primitives and pipelines named below, including UTC time, both Git-environment
detectors, protected-status encoding, exact review-file base64, and commit-
message byte verification.
Shared procedure text specifies operations; the platform appendix in the
canonical intake skill supplies syntax for copy, per-file same-volume move,
symlink/reparse checking, byte count, and raw SHA-256. Git operations and
semantic obligations are identical. The Windows local profile contains the
same enumerated Git families for Bash and PowerShell because Desktop has emitted
both tool shapes; that compatibility list grants no broader shell authority.

The standard local profile allows only stable ledger command families so Tier
0 can work without routine prompts. Common destructive-Git and native `.git`
edit denies reduce accidents; they are not an adversarial security boundary,
and native Windows has no Claude shell sandbox. Runtime capability never grants
task, Git, publication, retrieval, or external-action authority. Push and
remote changes remain separately ask-gated.

The following forms are compatibility constraints, not requests or authority.
Use a form only when the participant's current request and applicable in-chat
gate authorize that operation. For an ordinary single-checkout task opened at
the exact ledger root:

- Except for the exact Git-environment detector pipelines, protected-status
  encoding pipeline, current-HEAD and historical commit-message byte-oracle pipelines, and applicable GUID-only batch named below, make exactly
  one listed shell primitive per tool call. Never prepend or append `echo`, a
  label, `2>&1`, `$?`, an exit-code probe, fallback, or another command.
  Outside those exact named exceptions, do not
  chain commands, separators, shell variables, redirects, command substitution,
  pipelines, or heredocs. Do not split, rewrite, wrap, or extend any named
  exception.
- Do not prepend `cd`, use `git -C`, or depend on persistent shell state.
- Use native Read, Edit, and Write tools for ordinary text reads and writes.
- Shared text sometimes names a Git operation in abbreviated form. Map it
  to the existing complete command before calling a tool. In particular:
  - object format: `git --no-replace-objects rev-parse --show-object-format`;
  - full machine-readable status: `git --no-optional-locks --no-replace-objects -c core.quotePath=false status --porcelain=v1 -z --untracked-files=all --ignored=no`;
  - staged tree: `git --no-replace-objects write-tree`.
  Preserve each operation's existing gates and result oracle. Do not run bare
  `git write-tree`, shortened porcelain status, an ignored-status pipeline,
  or add redirects/fallbacks to get equivalent-looking output. Use only the
  existing named forms for other Git operations. Before each command, check
  the complete proposed form against this syntax source and the validated
  local profile. Permission denial or an approval-required tool failure stops
  the affected route; do not repeat it or experiment with alternate commands.
- Before substituting any dynamic path or segment into a Bash or PowerShell
  command, validate it in reasoning. Generated UUIDs, checkpoint IDs, source
  IDs, versions, and slugs must match their canonical closed grammar. Every
  generated path therefore uses only command-safe segments. Before a committed
  legacy or other preexisting declared path is placed in a quoted Bash or
  PowerShell command, reject `..`, any dollar sign, backtick, double quote,
  control character, backslash-as-segment-content, any configured hard-deny
  token, or other syntax that the active shell can expand, substitute, split,
  or force a prompt/deny. In particular, case-insensitively reject the
  permission-reserved substrings ` -Force` and ` -Recurse`; stop for exact owner or maintainer
  action rather than escaping, rewriting, or broadening the command. A participant-supplied
  direct intake basename must match exact ASCII grammar
  `^(?!.*\.\.)[A-Za-z0-9][A-Za-z0-9 ._()-]{0,119}$`, must not end in a space or period,
  and must not have a whole name or the portion before its first period that
  case-insensitively equals a Windows reserved device name (`CON`, `PRN`,
  `AUX`, `NUL`, `COM1` through `COM9`, or `LPT1` through `LPT9`), `.gitkeep`,
  or any section-28 noise name. Case-insensitively reject the permission-
  reserved substrings ` -Force` and ` -Recurse`. Reject `$`, backtick, quotes,
  slash/backslash, colon, wildcard/metacharacter, control character, nested
  path, and `..`; give one plain rename instruction and do not interpolate or
  escape the name. For `<ext>`, take the characters after the basename's final
  period only when that suffix is 1–10 ASCII alphanumeric characters, convert
  ASCII letters to lowercase, and otherwise use `bin`, exactly as Reference
  section 4 requires. Apply the same closed-segment rule to recovery;
  an affected path outside it stops for maintainer recovery.
- A newly generated ledger/profile UUID must match exactly
  `^[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}$`. A new
  direct-ingestion source ID is exactly
  `<classification-prefix>-<rendered-ordinal>__<slug>`: classification prefix
  `contained`, `green`, `yellow`, or `red`; a positive per-classification
  ordinal rendered unsigned base-10 to a minimum width of four and never
  truncated; slug
  `[a-z0-9]+(?:-[a-z0-9]+)*`; complete segment at most 120 characters.
  Under the single writer immediately before candidate allocation, capture each
  used classification prefix's greatest valid committed ordinal M once, sort
  that classification's stable input group by normalized forward-slash path
  using ordinal UTF-8 bytes, and assign M+1, M+2, and so on while counting
  earlier provisional IDs in the same candidate. Duplicate or unstable input
  keys stop; an uncommitted candidate's provisional IDs remain reusable.
  Legacy/test namespaces do not advance a new direct-ingestion classification
  prefix's counter.
  A newly allocated dossier path is exactly
  `dossiers/active/YYYY-MM-DD__<slug>.md`, with the real valid local task-start
  calendar date, the same slug grammar, and a complete filename at most 120
  characters. Preserve valid committed legacy IDs/paths and an already
  initialized active dossier path; never rewrite them merely to normalize.
- Before the first Git call, inspect the selected root and `.git` separately
  with exact PowerShell calls `Get-Item -Force -LiteralPath "."` and
  `Get-Item -Force -LiteralPath ".git"`. Stop before mutation if current session
  metadata reports `isWorktree: true`, either item is a reparse point/link, the
  root is not a directory, or `.git` is not a normal in-root directory. After
  the Git-environment detector, require the exact `rev-parse --git-dir` and
  `rev-parse --git-common-dir` results to resolve to that same `.git` directory.
  This Windows participant profile does not support a linked worktree or
  junction/symlink root; canonical maintainer concurrency remains a separate
  qualified route.
- Before the first mutation through any named path family, walk that target's
  finite ancestor chain from the verified root to its parent, one exact
  `Get-Item -Force -LiteralPath "<ancestor>"` call at a time. Require every
  existing ancestor to be a real directory, not a link/reparse point, with its
  reported full path resolving beneath the same root. A missing tracked or
  participant-supplied ancestor stops. For an absent generated ancestor that
  this appendix explicitly permits, first prove that exact path absent with
  the matching `-ErrorAction SilentlyContinue` form, create only that one level
  with its listed `New-Item` form, then recheck it strictly before proceeding.
  Never use `-Force`, create multiple levels at once, or traverse an unchecked
  parent. Apply the same gate on recovery or whenever continuity is not
  established. The local profile enumerates only the supported parent/path
  families; unlisted ancestry stops rather than prompting for broader shell
  authority.
  The fixed generated parent levels are only `caches`, `caches/checkpoints`,
  `caches/claim-reviews`, `caches/participant`, `caches/recovery`, `profiles`,
  `profiles/operating`, and `add-files-here/reviewed-not-stored`. After the
  exact absence check, create one with the complete standalone command
  `New-Item -ItemType Directory -Path "<that-exact-level>"`; substitute no
  other level or option. Dynamic child forms are named separately below.
- Before each checkpoint staging/review sequence or any earlier
  identity-sensitive Git operation, run one Bash call with exact command
  `printenv --null GIT_INDEX_FILE GIT_OBJECT_DIRECTORY GIT_ALTERNATE_OBJECT_DIRECTORIES GIT_DIR GIT_WORK_TREE GIT_COMMON_DIR | wc -c`.
  Proceed only when trimmed stdout is exactly `0`, stderr is empty, and the tool
  reports no error. A positive integer, missing or malformed output, stderr, or
  tool error stops the checkpoint; never infer cleanliness from the pipeline's
  exit code. This sanctioned pipeline does not expose environment values. Use
  the listed `rev-parse --show-object-format` form and
  `git --no-replace-objects ...` for every identity-sensitive command. This is
  the Windows equivalent of disabling replacement objects without persistent
  shell state.
- During first profile setup on exact native generation-zero state with null
  ledger ID, generate the three required values with one PowerShell call whose
  complete command is `New-Guid; New-Guid; New-Guid`. Map them in order to
  ledger ID, profile ID, and checkpoint-ID entropy seed. Only when an already-
  bound valid ledger has no profile and the current task is creating its first
  profile, preserve the ledger ID and use complete command `New-Guid; New-Guid`
  for the new profile ID and checkpoint seed. A profile revision or migration
  preserves both existing IDs and generates only one checkpoint seed with exact
  `New-Guid`. An ordinary task checkpoint likewise generates only its one
  checkpoint seed with exact `New-Guid`. Require exactly the expected number of
  distinct valid GUIDs with no tool error or stderr. Do not add variables,
  labels, strings, pipes, properties, or methods, and never use
  `[guid]::NewGuid()`.
  Form the checkpoint suffix in reasoning by removing seed hyphens, lowercasing,
  and taking the first 12 hexadecimal characters; prepend `cp-YYYYMMDD-` using
  the captured UTC date. Do not transform it in the shell.
- Obtain UTC milliseconds through Windows Git Bash with exact command
  `date -u +%Y-%m-%dT%H:%M:%S.%3NZ`.
- Inspect the exact checkpoint-receipt directory with native Glob or exact
  PowerShell command
  `Get-ChildItem -Force -LiteralPath "caches/checkpoints" -ErrorAction SilentlyContinue`.
- After the participant gives the exact ordinary-task save phrase and before
  writing its authority record, establish `caches/` and
  `caches/participant/` one level at a time under the ancestor gate, using each
  listed `New-Item` form only for a proved-absent level. Then run the exact
  missing-tolerant `Get-Item` for
  `caches/participant/task-save-authority.json`. Absence permits one native
  Write. An existing target must first pass the strict `Get-Item` as one regular
  in-root non-link/non-reparse file and be raw-hashed alone. Reuse exact valid
  current bytes without rewriting; after a new direct phrase, a stale or
  malformed regular record may be replaced only after its prior hash is
  rechecked with no intervening or parallel mutation. Any other type stops.
  After the one exact Write, strictly retype, raw-hash, reread, and validate the
  complete expected bytes/schema. A partial, missing, linked, or mismatched
  result grants no authority and stops; never infer success from the direct
  phrase alone or silently retry the write.
- For a profile snapshot, substitute either the newly generated canonical
  lowercase profile ID or a preserved legacy profile ID matching the same
  hyphenated hexadecimal UUID groups case-insensitively. Retain a legacy ID's
  exact spelling; braces and every other form stop for maintainer action. Also
  substitute the positive profile version rendered as unsigned base-10, left-padded with
  zeroes to a minimum width of four and never truncated, into PowerShell commands
  `New-Item -ItemType Directory -Path "profiles"`,
  `New-Item -ItemType Directory -Path "profiles/operating"`,
  `New-Item -ItemType Directory -Path "profiles/operating/<profile_id>"`
  and
  `Copy-Item -LiteralPath "current/operating-profile.json" -Destination "profiles/operating/<profile_id>/v<rendered-version>.json"`,
  one call each, with forward slashes and no other option. Before creating a
  generated directory or copying/moving to any destination, use its listed
  missing-tolerant `Get-Item -Force -LiteralPath "<destination>" -ErrorAction
  SilentlyContinue` form and proceed only on exactly no output and no tool
  error; a preexisting destination stops rather than being overwritten. This
  is a single-writer check, not an atomic filesystem guarantee. Dynamic local
  rules reduce routine prompting but do not enlarge the authorized path.
- Hash exactly one file per PowerShell call with the corresponding bare
  `Get-FileHash -Algorithm SHA256 -LiteralPath "<path>"` form listed in the
  template. Use the returned `Hash` and normalize its case in reasoning. Never
  combine hash commands or append `.Hash`, `.ToLowerInvariant()`, a pipeline,
  property access, or method call.
- For Windows intake, use one literal source or destination per call and only
  these PowerShell shapes after the applicable semantic and choice-5 gates:
  `New-Item -ItemType Directory -Path "sources/contained/<source-id>"`
  or `New-Item -ItemType Directory -Path "sources/green/<source-id>"`;
  `Copy-Item -LiteralPath "add-files-here/<filename>" -Destination "sources/contained/<source-id>/source.<ext>"`
  for CONTAINED or
  `Copy-Item -LiteralPath "add-files-here/<filename>" -Destination "sources/green/<source-id>/original.<ext>"`
  for GREEN;
  `New-Item -ItemType Directory -Path "add-files-here/reviewed-not-stored/<checkpoint-id>"`,
  `Move-Item -LiteralPath "add-files-here/<filename>" -Destination "add-files-here/reviewed-not-stored/<checkpoint-id>/<filename>"`,
  and `Remove-Item -LiteralPath "add-files-here/<filename>"`. The move is only
  for an approved reviewed-but-unstored file after its checkpoint; the removal
  is only for a byte-verified duplicate after its checkpoint. Before and after
  copying or moving, use the listed direct-child/destination `Get-Item` and
  one-file `Get-FileHash` shapes; never recurse, dereference, use force, or
  overwrite an existing path. The tracked `sources/`, selected mode parent,
  and `add-files-here/` chains must pass the ancestor gate. If
  `reviewed-not-stored/` is absent, create and recheck that one level before
  creating its checkpoint child.
- When canonical ingestion requires the Git blob identity of one file, use
  exactly `git --no-replace-objects hash-object --no-filters -- "<option-safe-path>"`
  with one validated forward-slash in-root path.
  The `--` is mandatory; never add `-w`, an output option, a second path, or
  another argument. This read-only identity does not replace raw SHA-256.
- Only when an authentic consistent existing dossier and strict section-23
  receipt plus applicable direct or saved authority admit mutating recovery,
  establish `caches/` and `caches/recovery/` one level at a time under the
  ancestor gate, then create only `caches/recovery/<checkpoint-id>/`, and only for event 1 after the
  listed missing-tolerant `Get-Item` proves it absent, with exact
  `New-Item -ItemType Directory -Path "caches/recovery/<checkpoint-id>"`.
  For later events, require the same regular non-link/non-reparse directory and
  use exact `Get-ChildItem -Force -LiteralPath "caches/recovery/<checkpoint-id>"`
  to prove its complete direct-child inventory equals every flat leaf already
  bound by the receipt. Follow section 29's contiguous positive sequences and
  minimum-four-digit, never-truncated filename rendering exactly. Before
  each regular-path copy, prove its exact
  `caches/recovery/<checkpoint-id>/event-<rendered-sequence>-file-<rendered-ordinal>.snapshot`
  destination absent with the listed missing-tolerant `Get-Item`. Require the
  source to be one regular non-link/non-reparse file of the recorded type; copy
  it with one listed source-family `Copy-Item` call to that flat destination,
  then hash source and copy separately and compare bytes. Record absent paths
  without a copy. Bind the manifest's complete raw status with the exact
  standalone/pipeline/standalone porcelain-v1-z sequence specified for
  `status_porcelain_v1_z_base64` below; never serialize rendered NUL output or
  substitute line-oriented status. Write and verify the deterministic manifest last at
  `caches/recovery/<checkpoint-id>/event-<rendered-sequence>-manifest.json`,
  then serially retype/rehash every affected source and flat copy, reverify the
  complete recovery-directory inventory, HEAD, index tree, and canonical status
  against the manifest. With no intervening or parallel call, append its
  immutable entry to `recovery_snapshots` before any governed
  index/candidate mutation. A partial, unbound, extra, or mismatched leaf stops;
  the newest complete event may resume only its same interrupted transition.
  The local profile covers only its enumerated mutable-ledger source families;
  an affected path outside them stops for an exact owner action and read-only
  verification rather than widening or improvising a rule.
- For a pending profile-renewal authority rebind, use only the listed tolerant
  and strict `Get-Item` plus one-file `Get-FileHash` shapes for exact
  `caches/participant/task-save-authority.json`. Preserve its verified prior
  bytes with the exact listed source-fixed `Copy-Item` recovery shape. Keep the
  file unchanged until the renewal commit passes every oracle; then bind the
  continuation-preservation event, recheck the prior hash with no intervening
  or parallel mutation, use native Write once for the exact intended UTF-8/LF
  record, and retype/rehash it. Exact intended bytes after the bound event may
  finish the pending receipt; any missing, linked, partial, or other bytes stop
  for maintainer recovery and grant no ordinary-save authority.
- For assistant-save staging, require the index empty and process the sorted
  declared paths serially, one call per path, using exactly
  `git add -- "<one-option-safe-declared-path>"`. Never name multiple paths or
  put a wildcard in the actual path. After the required `reviewer-repair` or
  other recovery event is bound, unstage by the same one-path serial rule using
  exactly `git --no-replace-objects restore --staged -- "<one-option-safe-declared-path>"`;
  never add `--worktree`, a source, wildcard, multiple paths, or unrelated path. Under 5C, enter
  `blocked`, ask the owner to run the exact-path unstage, and use only read-only
  verification before returning to `drafting`.
- For rollback of one path recorded present in the base, an assistant-save route
  first resolves current `HEAD` and proves its full OID equals the receipt base
  immediately before each restore, then uses one call exactly shaped
  `git --no-replace-objects restore --source=HEAD --worktree -- "<one-option-safe-declared-path>"`.
  Never substitute another ref/OID, omit the quotes, use a wildcard in the
  actual path, add `--staged`, or name multiple paths. For one path recorded absent at the
  base, use one exact `Remove-Item -LiteralPath "<one-validated-path>"` only in
  the local profile's enumerated current-profile, active/completed dossier,
  task-artifact, operating-profile snapshot, contained/GREEN source, or
  imported-legacy family, and only after a non-tolerant type check proves that
  exact target is a regular non-link/non-reparse file. Newly created empty
  directories may remain; never broaden deletion to remove them. Never use
  `-Force`, `-Recurse`, a wildcard in the actual path, or delete intake or
  recovery evidence. Under 5C, run neither rollback shape: give the owner the
  exact one-path commands and resume only after read-only verification.
- Use only the finite listed Git forms for ledger mechanics. Never add output,
  external-diff, text-conversion, execution, or configuration options. A
  no-output/nonzero result from either exact `git config --local user.name` or
  `git config --local user.email` query means the value is absent; never add a
  redirect, `echo`, or fallback. Run those as separate calls. Optional remote
  and hooks-path queries likewise use only their exact listed forms. The tool
  already reports status and stderr: never append `$?`, `echo`, or another
  probe. For exact `git config --get remote.origin.url` and
  `git config --local --get core.hooksPath`, no value with exit 1 means not
  configured and is expected. Stderr, a tool error, or any other nonzero exit
  stops.
- Before any mutation intended for a 5A/5B or other assistant checkpoint, and
  again immediately before its commit, run exact
  `printenv --null GIT_AUTHOR_NAME GIT_AUTHOR_EMAIL GIT_COMMITTER_NAME GIT_COMMITTER_EMAIL | wc -c`
  and apply the same exact-zero, empty-stderr, no-tool-error oracle. A present
  identity override stops; do not run this gate for 5C's owner-managed no-commit
  draft. Then run separate exact
  `git --no-replace-objects var GIT_AUTHOR_IDENT` and
  `git --no-replace-objects var GIT_COMMITTER_IDENT` calls. Parse the returned
  identities without a shell transformation and require both name/email pairs
  to equal the owner-attested local save credit. After commit, use exact
  `git --no-replace-objects log -1 --format=%an%n%ae%n%cn%n%ce HEAD` and require
  all four lines to match before reporting success, including after a 5C owner
  commit even though 5C skips the precommit identity gates. A mismatch is a
  failed checkpoint and stops; never rewrite history.
- After every assistant commit and every participant-reported 5C owner commit,
  run exact `git --no-replace-objects rev-list --parents -n 1 HEAD`. It must
  exit zero with empty stderr and exactly two space-separated full lowercase
  OIDs in the repository object format: token one equals current `HEAD` and
  token two equals the receipt's `base_head_oid`. Any additional or missing
  token, uppercase or abbreviated OID, different current HEAD, or different
  parent stops. This is the required one-parent oracle; neither `HEAD^` nor a
  base-to-HEAD diff can rule out a merge commit.
- Do not inspect an earlier commit body merely to imitate its message format.
  For current-`HEAD` checkpoint verification, never render its untrusted body.
  Run exactly
  `git --no-replace-objects log -1 --format=%B HEAD | tail -c 1 | base64 -w0`
  and require zero exit, empty stderr, no tool error, and stdout exactly `Cg==`.
  With no intervening or parallel call, run exactly
  `git --no-replace-objects log -1 --format=%B HEAD | head -c -1 | sha256sum`
  and require zero exit, empty stderr, no tool error, and the first output token
  to be exactly the receipt's lowercase prepared-message SHA-256. These stream
  oracles prove the one formatter LF and remaining raw bytes without exposing
  message content. For these active verification forms, never substitute an
  OID. Never trim the hashed stream, add an option/segment, or run the Git
  command standalone.
- For a historical terminal `complete` receipt only, first validate its
  `commit_oid` as a full lowercase OID in this repository's object format.
  Keep section 23's immutable parent/tree/path checks and all separate current
  state gates. Run exactly
  `git --no-replace-objects log -1 --format=%B <commit-oid> | tail -c 1 | base64 -w0`
  and require zero exit, empty stderr, no tool error, and stdout exactly `Cg==`.
  With no intervening or parallel call, run exactly
  `git --no-replace-objects log -1 --format=%B <commit-oid> | head -c -1 | sha256sum`
  using the same validated OID. Require zero exit, empty stderr, no tool error,
  and the first output token exactly equal to `commit_message_sha256`.
  Substitute only that validated OID. Never render the body, trim or reencode
  bytes, add an option/segment, or run the message-producing command standalone.
  This route does not require the historical scratch message to remain live.
- Never use Python, Node, `sh -c`, nested PowerShell, or another interpreter for
  ledger bookkeeping. Codex on Windows has only the shared intake skill's
  narrow Git Bash launcher exception for its seven listed forms;
  it does not permit arbitrary interpreter code. Claude keeps its existing
  native Bash tool route and prepared policy unchanged.

## Receipt and checkpoint implementation

On Mac, apply the Platform operation map to every named Windows operation
below. Keep the full transaction, evidence and transition rules unchanged.

Inspect the receipt path read-only with the missing-tolerant form above; absence
means no receipts. Before creating a receipt, prove its exact generated
`caches/checkpoints/<checkpoint-id>.json` path absent with the listed missing-
tolerant `Get-Item` form. Validate every existing receipt against section 23's
strict schema, transition graph, actor/authority/scope matrix, review-attempt
history, append-only recovery-event array and flat-manifest inventory, evidence-
path grammar, authority-rebind lifecycle, and action/count cross-fields before
relying on it. Complete the TRACER, exact-root, Git-environment,
HEAD/index/worktree, and recovery gate before mutation. Allocate the checkpoint
ID before meaningful dossier initialization and record it there. After the
dossier is initialized and fully reread, immediately establish and strictly
recheck `caches/` and `caches/checkpoints/` one level at a time under the
  ancestor gate, using each listed `New-Item` command only after its exact
  missing-tolerant check, then write the `drafting` receipt. After every receipt
  write, run the exact strict `Get-Item` for that receipt leaf, require one
  regular in-root non-link/non-reparse file, then raw-hash, reread, and validate
  its complete expected bytes/schema before relying on it. This is not a pre-
  recovery cache bootstrap and precedes every non-dossier task mutation.

Append each protected review wrapper to `review_attempts` before acting on its
disposition and retain every prior attempt across repair. For phase-one intake,
append exactly one verified post-commit action for each source input: a verified
delete, verified holding move, explicit defer/decline, or exact
`leave-in-place: completed`. Recompute the three counts from the recorded array
at every write; never infer completion from prose or omit a retained 5C input.
For profile renewal, a nonnull pending `authority_rebind` keeps the receipt
`committed` after the tracked commit verifies. Complete its one recovery-
preserved ignored-file replacement and exact hash/type/schema check before
marking either the rebind or receipt complete. Precommit cancellation leaves
the old record byte-identical and marks the rebind cancelled; postcommit
cancellation is unavailable.

For every local checkpoint, use native Write to prepare the complete BOM-free
strict UTF-8/LF message with exactly one final LF at ignored
`caches/commit-message.txt`, hash that file alone, and bind its fixed path/hash
in the receipt before handoff or commit. Never prepare it under
`current-chat-draft`. While a nonterminal receipt contains the pair, the live
regular non-link/non-reparse file must match that sole receipt at each completed
boundary and no other nonterminal receipt may bind it. A complete receipt does
not reserve the scratch forever. The sole active drafting receipt may replace
it only when every other receipt is terminal. For a new checkpoint, match an
existing scratch to either the completed receipt for the active base `HEAD`
whose commit-message oracle passes or a terminal `cancelled` receipt at that
base with exact rollback and the same retained pair. For a reaccepted tree in
the same receipt, first match the superseded pair. Write, hash, bind, and
immediately revalidate the new pair. An interruption between write and binding
stops for maintainer recovery. Use exact missing-tolerant
`Get-Item -Force -LiteralPath "caches/commit-message.txt" -ErrorAction SilentlyContinue`
before creation and exact non-tolerant
`Get-Item -Force -LiteralPath "caches/commit-message.txt"` for the existing-file
type check. Otherwise stop rather than overwrite it. Immediately
before an assistant commit, recheck the hash and run exact
PowerShell command
`Get-Item -Force -LiteralPath "caches/.no-hooks" -ErrorAction SilentlyContinue`.
Any returned object stops the checkpoint; the path must be absent. Never create
or delete it. An assistant commits only with exact form
`git --no-replace-objects -c core.hooksPath=caches/.no-hooks -c commit.gpgSign=false commit --cleanup=verbatim -F caches/commit-message.txt`.
Verify the tree with exact quoted form on either platform
`git --no-replace-objects rev-parse "HEAD^{tree}"`. Command-local hooks and
signing suppression implement checkpoint contract v1 and do not persist a Git
setting. Under 5C, never run the assistant commit command above or prescribe
the owner's hook/signing policy; do run the read-only post-owner-commit tree and
message verification. Apply section 23's exact message-bound handoff and fail
closed if the owner's resulting parent-count/base oracle, tree, message, paths,
complete status, or recorded identity differs.

## Setup, ingestion, and ordinary save

Follow the canonical intake skill exactly for setup, phase one, phase two,
task-scoped adds, ordinary checkpoints, recovery, and fixed participant
messages. There is no privileged Participant command, request file,
transaction pointer, or helper-owned staging tree; the visible Claude
coordinator performs Tier 0. Broad shell capability changes capability only;
authority still comes from shared governance and the participant.

The adapter does not invent a manifest schema. For every new direct-ingestion
row, apply Reference section 9's exact 19-key order, types, mode/disposition
variant, body/path/hash/null bindings, profile/checkpoint identity, and
deterministic append rules. Preserve committed legacy rows at their historical
bytes and schema boundary as that section requires.

A task-scoped add may complete both semantic gates and continue the original
task in the same conversation; neither gate is skipped. After a confirmed
plain-brief profile, keep routine mechanics concise while remaining
transparent. Show required choices, bounded checkpoint notices, meaningful
participant-actionable blockers, and the final result. Provide full details on
request.

Do not use connectors, web retrieval, remote synchronization, publication, or
external action under this skill unless the participant separately requests
the action and canonical governance authorizes the route.

## Protected claim review

Use only the project `claim-reviewer` agent for the separate Claude semantic
review. Before dispatch, the visible coordinator:

1. with assistant-save authority, requires an empty index before staging; under
   5C, requires the already owner-staged, read-only-recorded complete index and
   makes no staging mutation;
2. with assistant-save authority, stages only the sorted declared paths; under
   5C, read-only reverifies the recorded owner-staged tree;
3. proves every working-tree surface the reviewer reads matches its bound
   staged-tree or base-tree blob;
4. captures `base_head_oid`, `staged_tree_oid` from `git --no-replace-objects write-tree`, the single
   UTC-millisecond `sealed_at`, declared paths, exact add/modify/type-change/
   delete entries, trace reference/hash/mode, rubric hash, reviewer identity,
   review iteration, and exact review-materials hash;
5. records the deterministic pre-review snapshot bytes and hash; and
6. provides only the exact candidate, governing material, rubric, and routed
   dependency/relation surfaces bound by that materials manifest.

The reviewer has harness-enforced Read, Grep, and Glob tools only. It has no
shell, Git, write, recovery, staging, or commit capability. A deletion is an
exact delete entry with base mode/blob and null candidate mode/blob. Its bound
inert review material includes the complete base text and exact staged deletion
diff. Treat a rename as delete plus add.

After return, independently create the post-review snapshot. Any byte mismatch
or observed mutation invalidates the response. Capture the exact returned UTF-8
JSON bytes without parsing or reserializing them; store their SHA-256 and base64
in the final evidence wrapper. Put the exact wrapper base64 and SHA-256 plus
base and tree OIDs in the prepared commit body. Save only an accepted unchanged
candidate: commit and verify under assistant-save authority, or under 5C bind
the message, issue section 23's owner-commit handoff, stop, and later apply its
read-only owner-commit recovery oracle. Verify the resulting commit parent,
tree, and base-to-commit path delta. A nonaccept
uses the actor-conditioned route above: the assistant unstages only with
assistant-save authority, while 5C enters blocked owner-unstage recovery. Both
preserve working files. Never substitute
`ledger-worker`, a built-in agent, or coordinator self-acceptance when Deep
requires a distinct reviewer.

On either supported desktop platform (using its operation map), review attempt 1 first requires exactly no output
and no tool error from missing-tolerant
`Get-Item -Force -LiteralPath "caches/claim-reviews/<checkpoint-id>" -ErrorAction SilentlyContinue`,
establishes and strictly rechecks `caches/` and `caches/claim-reviews/` one level
at a time under the ancestor gate, then creates and strictly rechecks one
ignored working directory with exact
`New-Item -ItemType Directory -Path "caches/claim-reviews/<checkpoint-id>"`.
For a later attempt or continuation in the same authenticated receipt, require
that directory to pass the exact strict `Get-Item`, then use exact
`Get-ChildItem -Force -LiteralPath "caches/claim-reviews/<checkpoint-id>"` and
require its complete direct-child inventory, types, and raw hashes to equal the
receipt-bound prior-attempt evidence. Any extra, missing, linked, changed, or
  unbound leaf stops. Keep review-materials, pre/post snapshots, the verbatim
  reviewer response, and the final wrapper there as strict UTF-8/LF files.
  Render the positive iteration to minimum width four, never truncated, and use
  exactly `r<iteration>-materials.json`, `r<iteration>-pre-snapshot.json`,
  `r<iteration>-response.json`, `r<iteration>-post-snapshot.json`, and
  `r<iteration>-evidence.json`; the last is the wrapper path bound by the
  receipt attempt. The wrapper's embedded bytes/hashes derive and authenticate
  the other four leaves. Prove every new leaf absent before one Write; never
  overwrite or reuse a prior-attempt leaf. After every Write,
run its exact strict `Get-Item`, require one regular in-root non-link/non-reparse
file, then hash/reread it before binding or use.
The `caches/checkpoints/` directory remains receipt-only. Hash one review file
per listed `Get-FileHash` call. Encode any such complete file with one exact Git
Bash call
`base64 -w0 -- ./caches/claim-reviews/<checkpoint-id>/<safe-leaf>`; require canonical base64,
empty stderr, and no tool error. Do not compute or reserialize its bytes in
reasoning. Immediately write the reviewer's JSON-only response exactly as
delivered, without a Markdown fence or normalization, and hash/encode that
file before parsing a working copy of its text.

For `status_porcelain_v1_z_base64`, do not rely on the rendered NUL-bearing
tool result. First run the exact standalone status command and require success;
with no intervening mutation or parallel call, run exactly
`git --no-optional-locks --no-replace-objects -c core.quotePath=false status --porcelain=v1 -z --untracked-files=all --ignored=no | base64 -w0`,
then rerun the exact standalone status command and require success. The pipeline
stdout is the snapshot field only when it is canonical base64, stderr is empty,
the tool reports no error, and the surrounding status calls and derived path
inventory agree. This is the one protected-status encoding pipeline sanctioned
above; never add another segment, option, redirect, or path.

## Concurrent batches

- The visible originating Claude session is the sole coordinator and canonical
  integrator.
- Freeze the logical roster, base OID, exact owned paths, validation, and
  publication policy before launching workers.
- Use only the project `ledger-worker` for write-capable workers.
- Workers write only allocated paths, perform no mutating Git, and quiesce at
  `Content-ready; awaiting coordinator finish`.
- The coordinator owns worktree operations, staging, commits, serial exact-OID
  integration, validation, and any authorized publication.
- Run every coordinator Git mutation with an explicit exact workdir and assert
  expected top-level root, branch, HEAD, and cleanliness boundary. Never rely
  on persistent shell CWD after entering worker worktrees.
- Keep the canonical checkout reserved while workers run. Stop and preserve
  evidence if recovery would require reset, force, destructive cleanup, or
  scope expansion.
- Never let a worker mutate `current/**`, `sources/**`, intake, governance,
  adapters, tools, hooks, configuration, or sibling paths.

The repository cannot grant itself Claude Auto mode. Auto changes capability,
not authority. Dangerous bypass remains forbidden.

## Qualification boundary

Each desktop platform is release-qualified only after section 31's applicable
native acceptance evidence passes. An explicitly authorized native qualification
journey may exercise its candidate adapter. The supported desktop route copies
the tracked standard template for that operating system to ignored
`.claude/settings.local.json` exactly as `START-HERE.md` directs. For each
qualified workflow, expect zero or one workspace-trust dialog for a new root
and zero routine Tier 0 permission dialogs afterward. Setup plus an ordinary
checkpoint does not itself qualify ingestion. Distribution alone does not
qualify Cowork, Chat, connectors, another account, another materially relevant
version, another platform, worktrees, or general ingestion.

Project auto-memory remains off. Built-in Explore and Plan agents remain denied
because they do not load project instructions. The active local settings file
is ignored runtime state, never ledger authority. Each tracked platform template
is an inert activation source and never acts as local settings under its shipped
name.

For profile and release evidence, owner-facing permission description
`standard editing inside this workspace` maps to exact Claude value
`acceptEdits`. Record the candidate/version, hashes of applicable settings,
effective permission value, never-before-used-root trust prompt, and permission
transcript. A materially changed surface or version expires only that
qualification; do not ask the participant to interpret the technical value.

Keep three evidence kinds distinct:

- participant-attested client surface in `harness_surface_asserted`, such as
  `Claude Desktop (Local) on Windows`;
- any execution identity Claude reports, without asking it to deny or rewrite
  that identity; and
- directly available session metadata recorded separately during qualification.

A Desktop client surface and Claude Code execution identity can coexist.
Neither shell choice nor the participant's client description proves or
disproves the execution identity.
