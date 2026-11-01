# Start Here — Work Ledger v1.1

This guide starts a new ledger on Windows or Mac using Claude Desktop
Code/Local or Codex desktop Local. Download
[work-ledger-v1.1.zip](https://github.com/automatedteach/work-ledger-starter/releases/download/v1.1/work-ledger-v1.1.zip),
extract it into a new folder and keep its contents together. Do not copy it
over an existing ledger or substitute GitHub's automatic source-code ZIP.
The optional dedicated-writer mode uses the same roles in both apps on Windows
and Mac. Finish normal setup, then follow [V1.1-UPDATE.md](V1.1-UPDATE.md) if wanted.
The release notes distinguish implemented procedures from actual runtime checks.

## 1. Install the prerequisites

Install your chosen desktop app and Git, then restart the app.

- Windows: Git for Windows with Git Bash. Codex also requires PowerShell 7.5
  or later for the ledger's environment checks.
- Mac: macOS 14 or later, with Git available. In Terminal, running
  `git --version` may offer Apple's command-line-tools installation; complete
  that installation and retry.

Open a terminal in the exact extracted ledger folder. On Windows, right-click
an empty area in that folder and choose **Open in Terminal**, then select a
PowerShell tab. On Mac, open Terminal, type `cd ` (including the space), drag
the extracted folder from Finder into Terminal, and press Return.

Run:

```text
git --version
```

Continue when it prints a Git version. For help, use the contact details on the release page.

## 2. Prepare this folder

### Claude only: activate its local permission profile

Keep Claude closed. In the terminal opened in this ledger folder, run the
command for your operating system once.

**Windows — PowerShell**

```powershell
if (Test-Path -LiteralPath ".claude/settings.local.json") { throw "Stop: .claude/settings.local.json already exists; do not overwrite it." } else { Copy-Item -LiteralPath ".claude/policies/desktop-windows-standard.settings-local.example.json" -Destination ".claude/settings.local.json" }
```

**Mac — Terminal**

```sh
if [ -e "./.claude/settings.local.json" ] || [ -L "./.claude/settings.local.json" ]; then
  printf '%s\n' 'Stop: the local settings file already exists; leave it unchanged and ask for help.' >&2
else
  /bin/cp -n "./.claude/policies/desktop-macos-standard.settings-local.example.json" "./.claude/settings.local.json"
fi
```

Success normally prints no message. The active copy stays local and is excluded
from Git saves. If it already exists, leave it unchanged and ask for help
comparing it. Repeating a successful activation is expected to stop. Never use
the Windows profile on Mac. Codex does not need this Claude-specific copy.

### Both apps: choose the name on local saves

In the same terminal, check:

```text
git config --local user.name
git config --local user.email
```

If either value is blank or wrong, set it using your intended name and email:

```text
git config --local user.name "Your Name"
git config --local user.email "you@example.com"
```

These settings apply only to this folder. Use the same name and email on the
setup card. They identify local saves, not your AI-provider account.
Choice 5C lets you manage Git saving yourself; its no-commit draft does not
require the assistant-save identity check, but your later commit must still
record your attested name and email.

## 3. Open the ledger and request setup

Open the exact extracted folder as a **Local** workspace in your chosen app.
Select the folder itself, not its parent or a subfolder. Work directly in it
with worktree isolation off.

- Claude: select **Accept edits**. Do not use Auto or bypass mode.
- Codex: use normal editing inside this workspace (recorded as
  `workspace-write`).

An initial folder-trust or access prompt may appear. Routine ledger work should
not repeatedly interrupt you for permission. If a request is unclear, choose
Deny and ask for help. Do not use Always allow or broaden permissions to hide a
problem. Report recurring prompts with the app, OS, step and dialog text.

Send the message for your app, replacing `[Windows or macOS]` with your OS.

**Claude**

`I'm using Claude Desktop in Local mode on [Windows or macOS], and I have confirmed Accept edits is selected. This is my Work Ledger. Please use its setup instructions to show me the setup card first. I will answer the card before you take any setup action.`

**Codex**

`I'm using Codex desktop in Local mode on [Windows or macOS], with standard editing inside this workspace. This is my Work Ledger. Please use its setup instructions to show me the setup card first. I will answer the card before you take any setup action.`

The first response should show the five-choice card as an ordinary assistant
message. Claude invokes the project's intake-ingest skill to supply it; there
are no other project reads, commands or mutations before your reply. Codex may
already receive AGENTS.md from its harness, but likewise takes no repository
action before your card reply.

## 4. Answer the five choices

Correct any displayed fact that is wrong and supply lines marked
`not yet supplied`. To choose all recommended options, use this form with your
non-secret account/organization label and configured local-save identity:

`recommended; account/organization label: my-workspace; local save credit: Your Name <you@example.com>`

The recommended choices use approved company work, stable reusable
understanding, balanced source notes, brief communication and automatic local
saving for setup and directly requested ingestion.

A checkpoint is one unsigned local Git commit. Hooks and signing are disabled
only for that invocation; no saved Git setting changes, and nothing is pushed
or uploaded. Under 5A, your complete reply authorizes the setup checkpoint.
Later direct ingestion requests and semantic-review replies authorize their
respective checkpoints and the card's verified intake handling. Under 5B, the
assistant asks at each covered boundary. Under 5C, you manage Git and intake
handling: the assistant drafts and lists files; you stage and report back; it
verifies and, where required, reviews that exact tree; then you commit and
report back for verification.

The assistant validates the folder before creating setup files. If a real
prerequisite fails, it gives one corrective instruction. After setup is saved,
you can add context.

## 5. Add your first files

Place files you want the workspace to use directly in `add-files-here/`, then
say `Ingest these files.`

Use filenames of at most 120 characters, starting with a letter or number, with
only ASCII letters, numbers, spaces, periods, underscores, parentheses and
hyphens. Avoid consecutive periods and a trailing space or period. The same
conservative naming rules apply on Windows and Mac. If the assistant flags a
reserved or unsupported name, rename that file and try again.

The assistant stores eligible source copies with provenance, asks once what
understanding should become reusable, saves according to your choices, and
ends with a readiness summary. Under 5A, duplicate intake copies are deleted
only after the applicable checkpoint and byte verification; reviewed files not
stored as sources move to the holding folder. The card states the full contract.

## 6. Work normally

Without dedicated-writer mode, keep one active writing conversation per ledger
folder. List its known requirements at the start and add incoming work there
while its work is unfinished or unsaved. Start the next writing conversation
after completion and saving.

If you enable [dedicated-writer mode](V1.1-UPDATE.md), keep that writer
conversation and work in separate reader/proposer task chats. Release selected
results to the designated writer for reconciliation.

Saving completed ordinary tasks has a separate one-time opt-in. The assistant
will offer it when appropriate. Reply
`SAVE COMPLETED TASK FILES AUTOMATICALLY` only if you want that bounded local
saving behavior; the setup/ingestion choice does not supply it.

To inspect understanding, say `Show what this workspace currently understands.`
To review stale or unresolved context, say `Run the garden.` Gardening starts
with relevant recorded claims and relationships (or says none are recorded)
and asks for your corrections before changing reusable meaning.

## Connected apps, help and next steps

Setup does not authorize web, connectors, external actions, publication or
remote backup. A connector being available is not permission to use it. The
assistant first establishes the permitted reading/use, then separately checks
storage and reusable-understanding approval. Sending, editing an external
record or publishing needs explicit authorization. Existing qualified
permissions can be reused within their scope; see
[EXTERNAL-CONTEXT-AND-GARDEN.md](EXTERNAL-CONTEXT-AND-GARDEN.md) for the first
qualification and later-use procedures.

For help, use the [release page](https://github.com/automatedteach/work-ledger-starter/releases/tag/v1.1) contact details. Report reproducible bugs through
[GitHub Issues](https://github.com/automatedteach/work-ledger-starter/issues) with your release filename, OS, app, step and observed result. Remove
private content from anything shared.

Use the [release notes](https://github.com/automatedteach/work-ledger-starter/releases/tag/v1.1) for exact package and observed runtime coverage. Both
harnesses on Windows and Mac have implemented reader/writer procedures; source
inspection is not an executed native journey. Automatic cross-app/cross-host
messaging is not promised. Existing serial routes retain their evidence limits.

Existing-ledger migration and device synchronization are downstream; do not
overlay this starter on an existing ledger. The optional Tier 1 helper is not
bundled or enabled. Ordinary Tier 0 use requires no ledger-supplied executable.
