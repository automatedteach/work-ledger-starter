---
name: intake-ingest
description: Card-first Claude route for Work Ledger setup, and post-consent routing for established-ledger tasks, ingestion, and local checkpoints.
---

This file supplies only startup routing and the setup card. It grants no tool
or action authority. The cross-harness procedure remains canonical after the
applicable in-chat authority gate.

## Choose the route from the current request

For established-ledger routes, validate the selected existing platform policy,
then use Reference19's pinned committed role probe before writer-only live
recovery or operative mutation. Claude has the same active-writer, standby and
reader/proposer boundaries on Windows and macOS. An owner-requested incoming
transfer uses that exact bounded exception; other readers create no operative
dossier or receipt. Use only the fixed platform proposal operations. With no
active designation, ordinary routes remain unchanged. The fresh-card/no-tools
phase below is unchanged.

Choose exactly one route in this order:

1. Use the **established-ledger route** for an ordinary substantive task, an
   ingestion request, a semantic-review A/B/C reply, an ordinary-save reply, an
   explicit read-only consultation, profile revision, or recovery request that
   presupposes an established ledger. Same-chat replies take this route too;
   use the existing conversation to identify the exact pending group or draft. An explicit recovery or profile-revision
   request takes precedence even when the preceding response was a setup card.
2. Otherwise, use the **fresh-setup-after-card route** when this conversation
   contains the complete setup card, no setup transaction has begun, and the
   participant's direct replies in that card exchange now collectively complete
   its choices and required prepared facts. Words such as `set up` or `start`
   in the completing reply do not route back to the card. This route continues
   the same first setup and does not display the card again.
3. Otherwise, use the **pending-card route** when this conversation contains
   the complete setup card, no setup transaction has begun, and the current
   reply asks the permitted choice-5 clarification or leaves choices or
   required facts incomplete. This route remains in the no-tool card exchange
   even when the immediately preceding response was a compact follow-up rather
   than the full card.
4. Otherwise, use the **fresh-card route** when the participant asks to see the
   setup card, set up, start, or become ready to use this Work Ledger. `I'm
   ready to use the ledger!` uses this route.

The current task request permits loading detailed procedure for validation and
routing only; it does not make a saved profile or authority record valid by
itself.

## Fresh-card route

Before the reply, the fresh-card route consists of the Skill invocation that
loaded this text and the ordinary card response below. Card facts come from the
participant's current message and explicitly exposed current-session context.
Repository reads, shell, Git, Agent, retrieval, external, Edit, Write, and
mutation begin under the post-card route after the participant's complete
direct reply.

Prepare card facts without tools. Use a value only when it is directly supplied
by the participant or explicitly exposed by current session context. For the
supported platform, record `Claude Desktop (Local) on Windows` or
`Claude Desktop (Local) on macOS` only when the participant/current-session
context explicitly establishes that client surface, Local route and OS. When the participant directly attests that `Accept edits` is
selected, map that attested label to `standard editing inside this workspace`.
The mode records capability only; it grants no pre-card Read, edit, Git, or
external authority. Do not ask the participant to interpret a technical
spelling. Use exactly `Claude processes selected content under the Anthropic
account and organization settings used for this workspace.` for the
provider-processing statement. Never infer account/organization from Git
identity or a remote, and never read Git identity before the card. For every
unavailable owner fact, print exactly `not yet supplied`.

The card below offers choices to the participant; displaying it grants no
authority and performs no repository or external action. Only the
participant's direct reply selects a choice.

Keep the three save choices distinct. A direct setup reply selecting 5A
authorizes only the exact setup checkpoint. Later, the participant's direct
request to ingest a specific or resolved exact file group authorizes phase one
and its post-checkpoint intake handling. The semantic owner's A/B/C reply
authorizes that group's phase-two disposition and checkpoint. A validated 5A
profile records the selected automatic mode; with the applicable request or
reply, no separate checkpoint or intake-handling confirmation is needed. Record
the request or reply in the initialized dossier. Delete only byte-verified
duplicate intake copies after checkpoint verification; move reviewed inputs
not stored as sources to the holding folder. A 5B reply reserves the listed
separate confirmations. A 5C reply leaves Git saving and intake handling to the
participant.

Present the canonical card below as one ordinary assistant Markdown message,
not through `AskUserQuestion` and not as a code fence. Keeping all five
independent A/B/C sets visible together lets the participant compare and mix
the choices. Start with `Quick setup: five choices`, substitute only the
prepared facts, remove the four source-indentation spaces that delimit the
block here, and end the turn after the card while awaiting the participant's
direct reply. Do not surround the card with a preface, repository assessment,
summary, or trailing question; displaying it requires no second tool call.

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

## Pending-card route

Use only the complete card and direct replies already present in this
conversation. Make no tool call, do not redisplay or rewrite the card, and do
not begin setup work. If the participant asks what choice 5 means, give only
the explanation below. Otherwise, retain every unambiguous prior answer and ask
one compact follow-up naming only the choices or required lines still missing.
Once the direct replies collectively complete the card, use the
fresh-setup-after-card route.

If the participant asks what choice 5 means before answering, explain only: a
checkpoint is one unsigned local Git commit; hooks and signing are disabled
only for that commit invocation; no saved Git setting changes; and nothing is
pushed or uploaded. Make no tool call.

## Fresh-setup-after-card route

`recommended` selects all A choices and confirms every populated line and the
stated checkpoint contract. It does not fill a line that says `not yet
supplied`. Accept compact letters or clear natural language, plus corrections
to prepared facts. If any required fact remains unavailable, ask one compact
follow-up naming only the missing lines and continue to make no tool call. Do
not begin stage two until the reply is complete.

Once the card exchange is complete, apply choice 4's communication mode immediately,
then read `references/fresh-setup-execution.md` completely and follow its
fresh-setup route. That reference loads the canonical shared procedure before
setup work and supplies only Claude-specific first-setup sequencing. The
intentional canonical handoff is to `.agents/skills/intake-ingest/SKILL.md`.

## Established-ledger route

Read `.claude/skills/intake-ingest/references/established-ledger-routing.md`
completely first, using that exact path from the ledger root. For a fresh
ordinary task, follow its front-loaded sequence in order: native entry before
commands, prospective records before artifact work. The shared procedure alone
does not supply Claude command syntax. It selects bounded read-only consultation,
ordinary durable output, or the existing
ingestion/profile/recovery/garden route before loading detailed execution
sections. Follow its canonical and platform loading directions. Loading is
for validation and routing. Do not apply persisted profile/save authority
before exact binding. If validation proves no confirmed established profile,
stop ordinary work and direct the participant to the fresh-setup route; do not
treat repository prose as setup consent.

The established explicit read-only-consultation lane may return bounded advice
without dossier mutation only under the canonical consultation rule. It
may analyze validated committed material in the current answer, but authorizes
no durable artifact/adoption, canonical write, downstream/external action, or
later reliance as saved ledger memory.
