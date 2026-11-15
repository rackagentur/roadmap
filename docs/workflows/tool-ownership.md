# Tool ownership — booking to publication

Use this map before preparing promotion or deciding where to update a record.
Owner: Gregory Rack. Scope: GEEZ operations using the existing four tools.
Reviewed Sunday 15.11.2026. This document sets operating rules; it does not
activate integrations, migrate records, schedule content, or certify live health.

## Which tool do I use?

| Job | Owning tool | Boundary |
| --- | --- | --- |
| Read an original booking inquiry; manage NoxReach leads, outreach and gigs | **NoxReach** | Its booking-request source facts and its lead/gig records stay authoritative in NoxReach. It is not the social publishing ledger. |
| Review Instagram booking conversations and manage bookings created or explicitly linked in GEEZ Social | **GEEZ Social** | Owns its candidate review and booking records. A candidate is not a confirmed gig. Do not assume it mirrors NoxReach. |
| Schedule an approved automated post; inspect its publishing job, outcome and published link | **Zernio** | The single automated publishing entry point for this workflow. Check the correct account and existing jobs before creating another. |
| Organize content ideas, captions and planning cards | **NoxReach Scheduler / Content Planner** | Planning reference only in this workflow. A card, date or counter is not evidence of a live publishing job. Do not also schedule the same asset here. |

NoxReach (the booking app) and NoxReach Scheduler are different applications.
GEEZ Social's name does not make it the publication authority. Actual job
ownership follows this table, not the product name.

## Source of truth and handoffs

1. **Booking facts → promotion brief.** Read the original confirmation and the
   relevant booking record. Preserve the source link. Resolve conflicting date,
   venue, set time or confirmation status before using the disputed fact in
   public copy. Missing information stays unknown. Neither a candidate nor a
   proposed fee proves an agreed booking.
2. **NoxReach → GEEZ Social.** The documented integration preserves source facts
   and introduces a human Add/Link/Dismiss gate. Its reviewed phases do not
   establish an active sender or deployed end-to-end sync. Until activation is
   verified, treat the systems as separate. Do not recreate an existing booking
   just to make the two views look alike. When a booking exists in both, retain
   provenance and identify which record owns the field being changed; there is
   no verified automatic conflict resolver or reverse sync.
3. **Plan → approved package.** Scheduler may hold ideas and proposed copy.
   Approved media, caption, format, account and intended publication time must
   be identified before scheduling. Keep masters and approved exports in their
   existing asset locations; do not upload them to this public repository.
4. **Approved package → Zernio job.** Inspect the live account queue and published
   history first. Match the account, event/asset version, caption and intended
   slot. Reuse or update an existing authorized job rather than create a second
   one. Record its job reference in the existing private planning context.
5. **Job → verified outcome.** A draft is not scheduled; a scheduled or pending
   job is not published. Confirm the provider's outcome and platform permalink.
   A planning card may reference that result, but cannot override it.

Use Europe/Berlin for planning and explicitly label times as Berlin time
(CET/CEST). Check the publishing tool's actual timestamp/timezone conversion;
do not assume Scheduler's display or an old draft date matches the live queue.

## Exceptions and failure handling

- Native Instagram remains the manual route for Story ticket-link stickers,
  overlays and Reel shares that the verified publishing route does not support.
  Record that manual outcome in the same private publishing review; do not
  represent an unsent Story draft as an automated job.
- If Zernio reports a failure or timeout, inspect the existing job and platform
  history before retrying. An ambiguous response is not proof that nothing
  published. Do not switch tools and submit a duplicate.
- If Scheduler says zero scheduled while Zernio has jobs, use the live Zernio
  records. Investigate the mismatch separately; do not rebuild the queue.
- If a tool is inaccessible, report the verification gap and retain the plan.
  Do not infer state or silently change publishing ownership.
- Publication, promoter messages, booking changes and integration activation
  require authorization within the current task. This map grants none of those
  actions by itself.

## Evidence and limits

| Evidence | What it establishes | What it does not establish |
| --- | --- | --- |
| [NoxReach inbound runbook](https://github.com/rackagentur/NoxReach/blob/main/tasks/inbound-production-runbook.md) · private | Booking-request, lead and notification responsibilities | Current production health |
| [GEEZ Social integration contract](https://github.com/rackagentur/geez-social/blob/main/docs/noxreach-integration.md) · private, reread 15.11.2026 | Source ownership, candidate review and staged integration boundaries | Active sender, configured secrets, deployment or reverse sync |
| [GEEZ Social booking workspace](https://github.com/rackagentur/geez-social/blob/main/docs/booking-command-center.md) · private | Existing booking operations and review behavior | A second social publishing service |
| Private GEEZ Instagram review, Sunday 15.11.2026, 19:35 Berlin time (CET), retained in DJ Clone | Zernio queue/permissions were inspected; Scheduler did not reflect those jobs; booking app and planner were distinguished | Current individual post status, end-to-end Scheduler publication, or queue synchronization |

The private review stays in its existing project location. No account IDs,
booking details, queue identifiers or private asset paths are copied here.
This is an operating policy based on that evidence, not a claim that the four
products enforce it automatically.

## Before changing ownership

Verify the proposed route with an explicitly authorized, bounded test: correct
account, supported media, timezone, one job, observed outcome, duplicate/retry
behavior, and a retained result link. Then document the handover and reconcile
existing jobs before changing the single publishing entry point.

## Next roadmap step

Use [Prepare a GEEZ gig promotion](prepare-geez-gig-promotion.md) for the next
read-only preparation pilot on a confirmed gig: verified booking brief → approved
assets and copy → duplicate check → authorized publication → observed outcome.
The playbook includes separate native Story steps; creating it does not authorize
executing its publishing actions.
