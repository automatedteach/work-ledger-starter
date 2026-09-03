# Source-Review Profile

Status: draft intent; retrieval disabled

Do not store secrets, OAuth material, sensitive account identifiers, raw source bodies, signed URLs, or credentials here. A connected source is capability, not authority.

This is a structured record, not a questionnaire to hand to the owner. Ask only the applicable owner-choice questions in short rounds; populate technical evidence during qualification and leave future branches deferred.

## Lifecycle

1. **Draft intent; retrieval disabled:** the owner chooses desired sources, jobs, bounds, memory, and no-action posture. Technical capability facts remain `pending qualification`.
2. **Qualification pending; retrieval disabled:** the owner has approved the exact installation/connection operation and minimal identity/capability check. This still grants no search or content access.
3. **Owner-qualified:** only an exact qualification row supported by observed adapter/account/surface/mechanism/version evidence and explicit owner confirmation may be reused. Every substantive run still needs an equal-or-narrower per-run card.

## Interview contract

The setup assistant asks no more than three short questions per round, uses plain-language A/B/C choices with the recommended conservative option first where feasible, and accepts `default`, `not sure`, or `decide later`. It branches first between `ad hoc only` and `consider recurring later`; schedule-only controls stay deferred for an ad hoc profile. It asks the owner only for policy and intent. The assistant, not the owner, fills scopes, tool/version details, indexing behavior, write-tool inventory, permission behavior, coverage, and exact working paths from observed qualification evidence. Each stage ends with a short summary and explicit confirmation.

Plain-language terms:

- **Exact item:** one named message, event, page, or file and only expressly included children.
- **Bounded discovery:** a search limited by source, selectors, dates/cursor, and result caps.
- **Recent/change review:** a bounded look for items added or changed since an approved point.
- **Minimal receipt:** the smallest provenance needed for an accepted consequential claim.
- **Tracked pointer:** safe metadata and a handle for a later separately authorized re-read, not stored content or future access authority.
- **Adopted conclusion:** a concise current fact or decision accepted by the owner, not a copy of the upstream item.

## A. Owner intent: sources, accounts, and jobs

- Owner (a non-secret label is sufficient):
- Supported harness/surface:
- Intended connector mechanism: native / MCP-backed / plugin-backed / pending qualification
- Source families enabled now:
- Source families deferred or disabled:
- Non-secret account/workspace label for each enabled source:
- Jobs this profile may perform:
- Exact-item fast paths and expressly included child scope:
- Bounded-discovery selectors:
- Review mode: ad hoc only / consider recurring after useful manual runs
- Repository reach or manual candidate hand-carry:

## B. Owner intent: inspection boundary

- Owner-initiated trigger:
- Lookback/look-ahead window or supported cursor:
- Metadata/result cap:
- Full-content fetch cap:
- Attachments: excluded unless separately approved
- Sensitive-topic exclusions:
- Account/tenant exclusions:
- Stop-on-unexpected-material rule:
- Expiry or reconfirmation event:
- Stop/revoke procedure:

## C. Owner intent: review, memory, provenance, and action

- Review destination:
- Candidate cap: 3 unless narrowed or deliberately changed
- Materiality threshold:
- Default memory disposition: ephemeral
- Allowed promotion modes:
- Raw-body retention: none
- External action authority: none
- Receipt rule:
- Tracked-pointer refresh/staleness rule:
- Coverage caveats:

## D. Schedule-only controls

Complete only after manual runs are useful and predictable. Otherwise mark this section `deferred`.

- Standing-review trigger:
- Timezone:
- Cadence:
- Lookback or change-cursor behavior:
- Quiet hours:
- Skip and catch-up behavior:
- Expiry/reconfirmation:
- Failure destination:

Standing authority covers bounded retrieval and candidate synthesis only. It never authorizes repository changes, durable memory, or external action.

## E. Qualification row

Create one row block per exact adapter, account, surface, and materially relevant version. Do not generalize evidence across rows.

### Qualification Q001

- Status: unqualified / qualification pending / owner-qualified / expired / disabled
- Source family:
- Adapter/tool identity and materially relevant version:
- Agent surface:
- Connector mechanism:
- Non-secret account label:
- Account identity verified at:
- Provider scopes and indexing/synchronization behavior observed:
- Available write-capable tools:
- Connector-specific permission mode:
- Provider-enforced or behavioral read-only:
- Minimal identity/capability check performed:
- Exact search/fetch paths that worked:
- Failed or unqualified paths:
- Coverage limits:
- Repository reach or manual hand-carry behavior:
- Tested date:
- Expiry/reconfirmation condition:
- Operational stop/revoke steps:
- Owner activation confirmation:

Operational revocation should, as applicable, pause any standing job, mark this row disabled or expired, disconnect or narrow connector permissions, verify that the qualified path no longer runs, and preserve the rule that a tracked pointer never grants future access.

## F. Profile confirmation

- Owner-reviewed draft confirmed:
- Active route: `- Active source-review profile: artifacts/source-review-profile.md`
- Qualification rows activated:
- Deferred controls:
- Next review condition:
- Owner confirmation:

## Per-run card

For a first qualification, use the guide's two approval cards, set the proposed row to `qualification pending`, and keep the run within the owner-confirmed draft. After activation, complete and show this card before every content run, expired profile, capability change, or materially different task; it must be equal to or narrower than an owner-qualified row:

- Present job/question:
- Qualified row:
- Source subset and non-secret account label:
- Exact item or bounded query:
- Dates/cursor:
- Metadata/result and full-content caps:
- Attachment and sensitive exclusions:
- Output and memory default:
- External action authority:
- Capability/coverage changes:
- Success condition:
- No-go condition:
- Owner approval:
