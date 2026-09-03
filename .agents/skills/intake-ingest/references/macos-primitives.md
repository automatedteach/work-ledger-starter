# macOS native primitives

This appendix supplies macOS syntax for the existing ledger procedures. It
does not change authority, editable paths, transaction ordering, review,
receipt schemas or saved outcomes. Follow the shared skill and Protocol for
the complete procedure.

Load after the applicable startup/card gate and before Mac commands. Claude
first completes its platform and Mac local-policy gate; Codex uses standard
workspace editing. Use the native shell supplied by the harness. Do not install
GNU utilities, Homebrew, PowerShell, Python, Node or a repository script for
these operations. These candidate forms do not assert native qualification;
an explicitly authorized qualification journey may exercise and record them.

## Command discipline

One primitive per call, except the exact pipelines below. Preserve the finite
Git forms and options in the active procedure. Do not append variables,
substitutions, diagnostics, redirects, fallback clauses, loops, wrappers,
`cd`, `git -C` or extra pipeline segments. Substitute placeholders only with
validated exact paths, IDs or positive decimal byte counts. Filesystem paths
are quoted and prefixed `./`; all existing ASCII safe-name, generated-ID,
allowed-parent and declared-path rules apply. No actual wildcard operand.

Native file tools are permitted only where the procedure authorizes them.
Except for the explicit false/absence results below, require completed status
0, no command diagnostic and the exact expected output. Denial, launch failure,
missing/truncated output or any unexplained result stops the affected action.
Do not broaden permissions or improvise substitute commands.

## Paths and files

Strictly inspect one existing path, without following its final symlink:

`/usr/bin/stat -f '%HT|%d|%z|%m' "./<path>"`

Fields are type, filesystem device ID, byte size and modification time. Use
this validated regular-file byte size wherever the common procedure needs an
intake/source/receipt file byte count; do not add a file-operand wc command.
The separate prepared-commit-message wc oracle below is unchanged. Require
the expected regular-file or directory type; a link or other type stops.
Do not add `-L`. Check the root, `.git` and each applicable ancestor separately
before descendant access/mutation; a safe leaf does not prove safe ancestors.

Where the procedure permits absence, make two separate calls:

`/bin/test -e "./<path>"`

`/bin/test -L "./<path>"`

Absence requires both completed statuses 1, empty output and no command
diagnostic. These expected false results are not execution failures. Either
status 0 establishes presence, including a dangling symlink; use the existing
presence rule. Every other result stops.

Create only a permitted, proved-absent directory with a verified parent, one
level at a time, then strictly recheck it:

`/bin/mkdir "./<directory>"`

No `-p`. List direct children of one validated existing directory with:

`/bin/ls -A1b "./<directory>"`

Hidden entries are included and nonprinting characters escaped. Reject names
outside the existing grammar, including escaped names; never decode escapes
into a new path. Check required children's types/hashes separately. A listing
error is not an empty inventory. Establish allowed directory absence before
treating its inventory as absent.

These are the exact replacements for strict/missing-tolerant `Get-Item`,
directory `New-Item` and `Get-ChildItem` at the Windows procedure's same call
sites and permitted paths.

## Private environment-presence counters

Before the first Git command and each checkpoint staging/review sequence, run
all six exact pipelines separately. Native printenv takes one name; do not use
Windows GNU `--null` or multiple names.

`/usr/bin/printenv GIT_INDEX_FILE | /usr/bin/wc -c`

`/usr/bin/printenv GIT_OBJECT_DIRECTORY | /usr/bin/wc -c`

`/usr/bin/printenv GIT_ALTERNATE_OBJECT_DIRECTORIES | /usr/bin/wc -c`

`/usr/bin/printenv GIT_DIR | /usr/bin/wc -c`

`/usr/bin/printenv GIT_WORK_TREE | /usr/bin/wc -c`

`/usr/bin/printenv GIT_COMMON_DIR | /usr/bin/wc -c`

Require exactly one nonnegative decimal integer line, allowing only native
horizontal padding around it, a known completed exit status, and no command
diagnostic or permission denial. Count 0 with status 0 or 1 means absent.
Count 1 or greater with status 0 means present. Every other result stops.
Proceed only if all six are absent. Never display a present value.

Native printenv returns 1 for absence. Pipeline settings determine whether the
whole pipeline returns 1 or 0 while wc returns count 0. A tool's mechanical
exit-code-1 label is expected only for that valid zero-count case. Do not retry,
append `|| true`, change shell options, request permission or discard status.
A present-empty variable emits one LF: count 1, therefore present.

Before any mutation intended for 5A/5B or another assistant checkpoint,
including dossier initialization, and again immediately before commit, apply
the same procedure to all four identity overrides:

`/usr/bin/printenv GIT_AUTHOR_NAME | /usr/bin/wc -c`

`/usr/bin/printenv GIT_AUTHOR_EMAIL | /usr/bin/wc -c`

`/usr/bin/printenv GIT_COMMITTER_NAME | /usr/bin/wc -c`

`/usr/bin/printenv GIT_COMMITTER_EMAIL | /usr/bin/wc -c`

All four must be absent. Preserve 5C's exception for owner-managed no-commit
drafts and its recorded-identity verification after an owner commit. All
effective/recorded author and committer identity checks remain unchanged.
Never run printenv standalone or without a name, enumerate the environment,
print values or substitute shell-dollar expansion.

## IDs and time

Generate one UUID per call:

`/usr/bin/uuidgen`

Make exactly the number required by the procedure: three for unbound native
first setup, two for first profile setup in an already-bound ledger, or one
for checkpoint entropy alone. Require distinct valid UUIDs; lowercase and
derive the checkpoint suffix in reasoning. Remove entropy hyphens, take the
first 12 lowercase hexadecimal characters and use the captured UTC date for
`cp-YYYYMMDD-`. Do not transform IDs in the shell.

Obtain UTC milliseconds with this sole fixed clock expression:

`/usr/bin/osascript -l JavaScript -e 'new Date().toISOString()'`

Require exactly `YYYY-MM-DDTHH:mm:ss.sssZ`. Capture a protected delta's sealed_at
once and retain the existing seal rules. This is the sole interpreter exception:
no other JavaScript, application automation, input, script file, argument or
bookkeeping program is authorized.

For an explicitly required local calendar date:

`/bin/date +%Y-%m-%d`

Never substitute it for UTC time.

## Hashing, copying, moving and cleanup

Hash one exact regular file:

`/usr/bin/shasum -a 256 "./<path>"`

Require one valid SHA-256 result for that path and normalize its digest to
lowercase in reasoning. Raw SHA-256 and Git-object hashes remain distinct.

After existing source, ancestor, destination-absence and authority checks:

`/bin/cp -n "./<source>" "./<destination>"`

Recheck source and new destination types and raw bytes. A success status alone
does not prove copying occurred. Preserve partial/conflicting results and use
existing recovery.

For a reviewed-but-not-stored intake holding move:

`/bin/mv -n "./<source>" "./<destination>"`

Require source and destination-parent device IDs from stat to match and the
destination to be absent. Afterward prove source absence and destination
type/raw-byte equality. No cross-volume copy-and-delete substitute.

Only after the applicable verified checkpoint, duplicate-byte checks and owner
authority, remove one exact direct intake duplicate:

`/bin/rm -- "./<exact-intake-file>"`

Recheck its type and bytes immediately before deletion, then prove absence.
Never apply this to a directory, `.gitkeep`, holding-folder file, unreviewed
input or broader family. Preserve selected 5A/5B/5C behavior: a command form
grants no authority. No force, recursion, overwrite or metadata-changing
options. All existing path-family exclusions and recovery obligations apply.

## Authenticated rollback removal

This is separate from post-checkpoint intake cleanup. For an owner-authorized
rollback under an authentic receipt and preserved recovery record, follow the
existing actor, base-HEAD, declared-path and prior-state checks. For a path
recorded absent at the base, after proving the target is the exact regular
non-link file in the validated root/ancestor chain, use:

`/bin/rm -- "./<one-validated-prior-absent-path>"`

Only the existing enumerated current-profile, active/completed dossier,
task-artifact, operating-profile snapshot, contained/GREEN source or
imported-legacy families are eligible. Keep every existing rollback
precondition, preservation requirement and final verification; this paragraph
grants no rollback authority. Newly created empty directories may remain.
Never delete intake, recovery evidence or another family through this route.
Under 5C, the assistant does not execute rollback commands: provide the
existing exact one-path owner handoff and resume by read-only verification.
A prior-present path retains the original exact Git restore form and its
immediately preceding full base-HEAD check.

## Review-byte encoding

Keep existing review directories, numbered leaves, strict UTF-8/LF, absence
checks, one-write boundaries, hashes and immutable attempt evidence. Use the
Mac path primitives at the same call sites. Encode a complete validated file:

`/usr/bin/base64 -i "./caches/claim-reviews/<checkpoint-id>/<safe-leaf>" | /usr/bin/tr -d '\n'`

Require canonical base64, successful execution and no diagnostic. Do not
normalize or reconstruct bytes in reasoning. Preserve the exact delivered
reviewer response before parsing a working copy.

For raw protected status, retain successful exact standalone status calls
immediately before and after this pipeline, without intervening mutation or
parallel call:

`git --no-optional-locks --no-replace-objects -c core.quotePath=false status --porcelain=v1 -z --untracked-files=all --ignored=no | /usr/bin/base64 | /usr/bin/tr -d '\n'`

Accept only canonical base64 with success/no diagnostic and matching
surrounding status observations and derived path inventory. Never rely on
rendered NUL-bearing output. Frozen bindings, snapshots, reviewer identity,
independence, wrapper and commit-body requirements remain unchanged.

## Prepared and committed message bytes

Use the existing receipt's `commit_message_path` and `commit_message_sha256`.
Strictly validate the live prepared file and confirm its raw hash, then count:

`/usr/bin/wc -c "./caches/commit-message.txt"`

Require one positive decimal count for that exact file. Call it N in reasoning;
it is a transient measured value, not a new receipt property.

Keep every existing current-HEAD parent/tree/path/identity/receipt check. Never
render the committed message. Without intervening mutation or parallel call,
run these pipelines in order, substituting only the validated positive N:

`git --no-replace-objects log -1 --format=%B HEAD | /usr/bin/wc -c`

Require exactly N + 1 bytes.

`git --no-replace-objects log -1 --format=%B HEAD | /usr/bin/tail -c 1 | /usr/bin/base64 | /usr/bin/tr -d '\n'`

Require stdout exactly `Cg==`, the formatter's final LF.

`git --no-replace-objects log -1 --format=%B HEAD | /usr/bin/head -c <N> | /usr/bin/shasum -a 256`

Require the prepared-message hash. All three require status 0 and no
diagnostic. Together they verify exact message bytes plus one formatter LF
without displaying the body. In these active verification forms, do not
substitute an OID. No trimming, GNU negative-byte head, added pipeline segment
or standalone message-producing Git call. These oracles supplement all other
checkpoint/recovery conditions.

### Historical complete-receipt message bytes

For an already terminal `complete` receipt, validate its `commit_oid` as a full
lowercase OID in the repository's object format. Keep section 23's immutable
parent/tree/path checks and all separate current-state gates. Do not require
an old live scratch file or render the historical message. Run exactly:

`git --no-replace-objects log -1 --format=%B <commit-oid> | /usr/bin/wc -c`

Require one decimal byte count K of at least 2. Derive positive N = K - 1 in
reasoning; do not use shell arithmetic or add a receipt field. With the same
validated OID and no intervening mutation or parallel call, run in order:

`git --no-replace-objects log -1 --format=%B <commit-oid> | /usr/bin/tail -c 1 | /usr/bin/base64 | /usr/bin/tr -d '\n'`

Require stdout exactly `Cg==`, proving the final formatter LF. Then run:

`git --no-replace-objects log -1 --format=%B <commit-oid> | /usr/bin/head -c <N> | /usr/bin/shasum -a 256`

Require the hash token to equal the receipt's `commit_message_sha256`. All
three calls require exit 0, empty stderr and no tool error. Substitute only
the validated OID and measured positive N. No trimming, reencoding, GNU
negative-byte head, extra pipeline segment or standalone message-producing
Git call is permitted. This proves the immutable message's exact raw hash
after removing only its one formatter LF; no other receipt gate is relaxed.
