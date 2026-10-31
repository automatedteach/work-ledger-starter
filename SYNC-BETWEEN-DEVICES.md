# Sync Between Devices

Use private Git as a handoff between devices, never as background or live
filesystem synchronization. Only one device writes the ledger at a time.
Ignored `caches/tier1/activation.json` is device-local and is never synced or
inferred on another device.

`remote_sync.mode: off` means that no helper or unattended agent may fetch,
pull, merge, or push. It does not forbid an exact owner-directed operation.
Every remote mutation still needs the separate authority required by Protocol
section 15; ordinary local-save authority never includes a push.

## Before leaving a device

1. Finish or explicitly stop the active task. Do not hand off a partial claim
   review, ingestion phase, or ambiguous recovery state.
2. Verify that the index and worktree are clean and that every intended local
   commit is present on the expected branch.
3. Inspect the configured remote and branch. Do not silently add, replace, or
   repoint a remote.
4. With exact owner authority for this push, use a non-force push and verify
   that the intended remote branch reaches the local commit.

If the tree is dirty, the index is nonempty, or the branch/remote is not the
expected one, stop and resolve that evidence on the current device.

## On arriving at another device

1. Verify the expected repository, branch, clean index, and clean worktree.
2. Fetch from the recorded remote. Fetching is an external retrieval and uses
   the applicable owner authority.
3. Inspect the local and fetched branch relationship.
4. Advance only by a fast-forward. Verify the resulting `HEAD` and clean state
   before starting work.

If both sides have commits, or if any unexpected dirt or branch state exists,
stop for explicit review. Do not automatically merge, rebase, reset, clean,
stash, force-push, or discard either history.

Never live-sync the `.git` directory through OneDrive, Dropbox, or another
filesystem service. Never schedule unattended repository synchronization.

## Rehearsal

Before relying on this procedure, rehearse with two disposable clones:

1. make and push one commit from clone A, then prove clone B advances by a clean
   fast-forward; and
2. create different unpushed commits in A and B, then prove the procedure stops
   without changing either side.

Record the rehearsal result as release evidence. Do not put a private remote
URL in a distributed guide or receipt.
