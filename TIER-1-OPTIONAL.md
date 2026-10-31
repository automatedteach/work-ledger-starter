# Optional Tier 1 Helper

Tier 0 is the Work Ledger default. It needs Git and the assistant's ordinary
file tools, runs no ledger executable, and remains fully supported when Tier 1
is absent.

Tier 1 is one optional, unsigned POSIX-shell file for people who want an
additional byte-verification and per-file replacement backstop. It is never
part of the starter clone or zip, never fetched or installed by an assistant,
and never enabled merely because source code exists in a repository.

## Explicit activation

A human may activate the helper only after all of these steps:

1. Obtain `ledger-tier1.sh` separately from the matching release, or use the
   reviewed `optional-tools/ledger-tier1.sh` source in a maintainer checkout.
2. Compare its SHA-256 with the exact release receipt, then read the file.
3. Copy it deliberately to the fixed local runtime path
   `tools/ledger-tier1.sh`. That path is ignored by Git and is not distributed.
4. Run `sh tools/ledger-tier1.sh --version` and
   `sh tools/ledger-tier1.sh --self-test` in Git Bash on Windows or in a native
   POSIX shell on macOS/Linux.
5. Record the version, SHA-256, `self_test_result: pass`, self-test time,
   activation time, and human activator in the fixed local file
   `caches/tier1/activation.json`, using the exact Protocol Reference schema.
   The cache is process evidence, not ledger authority.

Until every step passes, use Tier 0. An assistant may use Tier 1 only when the
owner has explicitly activated it for this installation and the runtime file's
version and SHA-256 still match that local record and its self-test result is
exactly `pass`. A missing, stale, changed, or
inconclusive record falls back to Tier 0; it does not trigger installation.

## Commands and boundary

`verify <path> <sha256>` rejects a symlink or non-file and checks raw SHA-256.

`install <source> <destination> <sha256>` verifies the source, copies it to a
same-directory temporary file, verifies that temporary file, then renames that
one file into place and verifies the result. The rename is an atomic
replacement only for that individual file on the same volume. A multi-file
change becomes canonical together only at its Git commit.

`--self-test` proves that a changed file is rejected, an interruption before
rename leaves the old destination intact, and a real symlink is refused. It
uses a private test symlink when the host permits one, otherwise a known host
symlink. If neither exists, the proof fails rather than passing silently.

Tier 1 does not stage, commit, recover, push, allocate claims, approve semantic
meaning, or replace the claim reviewer. The same Protocol authority and exact
Tier 0 review boundary still apply.
