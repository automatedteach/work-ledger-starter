# Work Ledger

Work Ledger helps your assistant carry useful context between tasks: your goals,
decisions, working material and unresolved questions. You keep that context in
a folder on your computer and use it through Claude Desktop Code/Local or Codex
desktop Local.

Start with [START-HERE.md](START-HERE.md) for a new ledger. See
[V1.1-UPDATE.md](V1.1-UPDATE.md) for the dedicated-writer workflow and the
existing-ledger boundary. It covers Windows and Mac, with
separate steps where the operating system or app requires them. Use the named,
self-contained release ZIP and extract it into a new folder. Keep its contents
together. GitHub's automatic source-code ZIP and an ordinary clone are different
artifacts.

The starter supplies no executable program. Your assistant uses its normal file
tools and Git. Local saves do not upload the ledger or turn on remote backup.
Your chosen AI provider still processes the content you use through its app.

## What is new in v1.1

Optional dedicated-writer mode lets you work in separate task conversations,
review their results, and release updates to one persistent ledger writer.
The writer reconciles current meaning and returns the actual save result.
Both Codex and Claude Code on Windows and Mac have the same roles. Keep a
writer destination in each harness if useful, with one active writer at a time.
Switch by telling the incoming writer that the previous one is done and stopped.
Actual runtime coverage and native messaging availability remain explicit in
the release notes. Ordinary serial use is still available without enrollment.
See the [update guide](V1.1-UPDATE.md) before enabling it.

## First use

1. Follow START-HERE to prepare the folder and request the setup card.
2. Review its five choices and answer them.
3. Add files you want this workspace to use to `add-files-here/`.
4. Say `Ingest these files.`
5. Review the assistant's proposed reusable understanding.

The assistant stores eligible sources, asks what should become reusable, saves
according to your choices, and ends with a readiness summary. Under choice 5A,
it removes only byte-verified duplicate intake copies after the applicable
checkpoint succeeds. The setup card states the complete saving and handling
contract.

Saving completed ordinary tasks has its own one-time confirmation. Automatic
saving for setup and ingestion does not also enable it for every task.

## Everyday use

Open the same folder and ask your assistant normally. List all known
requirements at the start of one ledger conversation. Add incoming work to that
same conversation while its work remains unfinished or unsaved. Once the work
is completed and saved, start the next conversation.

Without dedicated-writer enrollment, keep one active writing conversation per
ledger folder. With enrollment, use separate task chats as readers/proposers
and release selected results to the designated writer. They do not independently
change the ledger. Stop or refresh old writing chats before activating this mode.

Useful requests:

- `Update this workspace from the files I added.`
- `Show what this workspace currently understands.`
- `Run the garden.`

Gardening reviews unresolved, stale or conflicting context. It starts by
showing relevant recorded claims and relationships for your confirmation or
correction. If there are none recorded, it says so. You decide any changes to
reusable meaning; routine housekeeping does not silently rewrite your decisions.
See [EXTERNAL-CONTEXT-AND-GARDEN.md](EXTERNAL-CONTEXT-AND-GARDEN.md) for more.

## Connected apps and online work

Setup does not authorize web access, connectors, sending, publication or remote
backup. Having a connector available does not grant permission to use it.

A direct request can establish the bounded material you want the assistant to
read and use. Before storing connected material or making its conclusions
reusable, the assistant checks the applicable storage and review authority.
Sending a message, changing an external record or publishing needs explicit
authorization. Available services and capabilities can differ between apps;
the same authority and ledger rules apply to both.

## Files and local saves

- `current/`: the ledger's current understanding, decisions and open questions.
- `sources/`: eligible source copies and their provenance.
- `dossiers/`: context and reasoning for individual tasks.
- `artifacts/`: work produced for you.
- `add-files-here/`: files you deliberately add for ingestion.

Use the supported filename guidance in START-HERE. Company-contained work uses
one approved workspace; mixed-context work keeps the more cautious
GREEN/YELLOW/RED handling. Neither choice grants external-action authority.

Important conclusions receive proportional reasoning records. Changes to
protected claims receive review of the exact proposed saved tree. Local Git
history is the saved record; keep a backup of the folder too.

## Existing ledgers and other devices

This starter creates a new ledger. Do not copy it over an existing ledger.
This candidate provides no in-place v1 upgrade. Migration and synchronization
between devices remain separately scoped work. The maintained references are
[MIGRATE-AN-EXISTING-LEDGER.md](MIGRATE-AN-EXISTING-LEDGER.md) and
[SYNC-BETWEEN-DEVICES.md](SYNC-BETWEEN-DEVICES.md). Neither is activated by setup.

## Help and technical reference

For installation or everyday-use help, see the contact details on the release page.
Use GitHub issues for reproducible bugs. Include the release filename,
operating system, app, step and what happened; remove private material before
sharing.

Technical maintainers should read [PROTOCOL.md](PROTOCOL.md) and
[TRACER.md](TRACER.md). Support is
established by external acceptance evidence for the actual package and tested
environments; this text does not self-certify a runtime.

The optional unsigned helper described in [TIER-1-OPTIONAL.md](TIER-1-OPTIONAL.md)
is not bundled or activated. A person must deliberately obtain, inspect,
hash-verify and install it. The default route remains Tier 0 without it.
