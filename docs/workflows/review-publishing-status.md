# Review publishing status without duplicate posts

**Purpose:** establish what is drafted, scheduled, published or unresolved
without creating another copy of the same post. **Trigger:** checking a campaign,
returning after a break, reviewing a due job, or investigating a failed/ambiguous
result. **Owner:** GEEZ; ChatGPT can perform the read-only review.
**Output:** a sourced status table and one next action per unresolved item in
the existing private project chat or content plan.

Follow [Tool ownership](tool-ownership.md): Zernio owns automated publication
and job outcomes; native Instagram owns manual Story execution; Scheduler is
a planning reference. NoxReach and GEEZ Social supply booking context, not the
publishing ledger. Use [Prepare a GEEZ gig promotion](prepare-geez-gig-promotion.md)
for new promotion preparation.

## Review boundary

This procedure is read-only. Do not create, edit, delete, cancel, retry, reschedule,
publish, graduate a Trial Reel, reconnect an account or trigger an import/sync.
Do not “fix” a draft's date or internal instructions while reviewing it.
An existing scheduled job may publish normally during inspection; preserving
it means leaving it alone, not pausing it to keep a snapshot unchanged.

If the user separately authorized a corrective action, finish the review first
and perform only that specific action in a distinct execution step. Do not
request the same authorization again. This document is not authorization for
republishing, switching tools, sending messages or installing a monitor.

## 1. Establish scope and time

Identify the intended account, campaign/event, relevant date range and existing
job references from the private plan. Resolve the account through the connected
account list; display names and an account's old connection ID are not sufficient.
If the intended account remains ambiguous, ask one precise question before
attributing records. Inspect other accounts only when they are in scope.

Fetch current Europe/Berlin time and begin the review with:

> Today is [weekday] DD.MM.YYYY, Europe/Berlin.
> Current local time in Europe/Berlin: HH:MM CET/CEST.

Convert stored timestamps explicitly and label displayed job times **Berlin
time (CET/CEST)**. Preserve source timestamps in the private evidence. If current
time cannot be fetched, request confirmation; do not infer whether a job is late
or propose a schedule. A user-stated date/weekday conflict needs clarification.

## 2. Read current records, not old totals

Read the account-scoped authored queue across relevant states, including drafts,
scheduled, published and failed records, plus cancelled records if exposed.
Read the relevant externally published history separately. Follow pagination
until the chosen scope is covered; record page coverage and any limits. Do not
trigger a platform sync merely to make this review appear complete.

Use the actual tool's documented filters. If results do not appear to honor a
search filter, inspect/filter the returned records and record that limitation.
Do not claim an exhaustive duplicate check from the first page or a text search.
Expired Stories, deleted posts and unsynced history can be absent.

Read full details for campaign matches: account, job ID, aggregate status,
per-platform status, scheduled timestamp, attempts/error, content, media/cover,
first comment, collaborators, Trial settings, recycling and outcome URL when
available. An aggregate status can hide a failure on one platform; assess the
specific account/platform separately. Do not overwrite an older snapshot.

## 3. Interpret the evidence

| Observed evidence | Report | Next action in this review |
| --- | --- | --- |
| Draft, even with a past `scheduledFor` timestamp or pending platform field | Draft; not a scheduled commitment | Preserve it; distinguish planning date from execution |
| Scheduled job with pending platform status, time still ahead | Scheduled; publication unverified | Retain the existing job and its exact settings |
| Time passed, still pending/processing | Outcome pending or delayed; not yet proven failed | Inspect the same job, attempts and platform history; do not submit another |
| Provider reports published and destination is accessible with matching content | Published and platform-verified | Retain job reference, permalink and observation time |
| Provider reports published but destination cannot be inspected | Provider-reported published; platform verification unavailable | Record the access limitation; do not repost |
| One platform succeeded, another failed | Partial success, named per platform/account | Preserve successful outcome; identify only the failing destination |
| Failed, cancelled or timeout/unknown result | Exact observed state; outcome may need reconciliation | Inspect history and the existing job before proposing recovery |
| Manual Story reference/draft | Manual action needed, unless there is completion evidence | Never infer publication from a draft timestamp |
| User reports manual publication; not independently visible | User-reported published | Attribute the report; record time/evidence without claiming direct observation |

No universal lateness threshold is assumed. Compare scheduled time, the
provider's observed processing state and current documentation if needed.
A collaborator invitation is not acceptance; a published Trial Reel is not
proof of follower-feed distribution or graduation. Preserve special settings.

## 4. Match identity before calling something a duplicate

Compare account, event, format, intended slot, caption, exact media version,
cover and existing job/platform identifiers. Different titles or URLs can point
to the same content. Where accessible and necessary, compare media checksums:
a renamed file with identical bytes is the same asset. Matching filenames alone
do not prove identity or approval; different hashes can reflect transcoding and
do not by themselves prove different creative content.

Distinguish these cases:

- **Same job seen in two tools:** reconcile references, not two publications.
- **Provider record plus externally synced copy:** match platform post ID or
  permalink before counting two published posts.
- **Reel plus intentional Story share/reminder:** different campaign pieces,
  not automatically duplicates. Confirm the purpose and authorization.
- **Two jobs for the same account/asset/slot:** suspected duplicate; identify
  both and their states. Do not delete or cancel either during this review.
- **No match found:** state the searched scope and limitations, not a guarantee
  that nothing exists. Never create a replacement to resolve uncertainty.

## 5. Check the manual Story handoff

For each manual piece, distinguish approved asset, proposed slot, named operator
and actual completion. Internal “MANUAL…” instructions are not public captions.
Draft storage timestamps are not execution commitments.

For a published Story, inspect the actual visible Story/archive where available,
or retain attributed user evidence. Check the intended artwork and ticket-link
destination where accessible. No active Story does not prove it was never posted:
it may have expired. If a ticket destination is rate-limited or inaccessible,
report **checkout/link availability unverified**, not “broken” or “safe to retry.”
Never switch to Scheduler to publish a manual Story or duplicate a Zernio job.

## 6. Record findings and preserve state

Use this table in the existing private project chat or plan:

| Piece / account | Existing job or platform reference | Expected asset/version | Observed job + platform state | Intended time (Berlin time, CET/CEST) | Evidence + checked time | Next action / owner |
| --- | --- | --- | --- | --- | --- | --- |

Separate newly observed facts from earlier records and proposals. Keep account
IDs, queue snapshots, private media paths and operational details out of this
public repository. Do not create another tracking database.

When checking preservation, reread the relevant records and compare content,
media, timing, account and settings. Classify differences: normal provider
progress, a change by another actor, or unexplained. A status transition does
not mean this review edited the post. If no second read is possible, state the
limitation and the fact that no write tools were used; do not claim byte-for-byte
preservation. Keep the scope finite; record future verification as pending
rather than setting up an automation implicitly.

## Recovery decision

If an item failed or is ambiguous, the review's output is a concrete proposal:
the existing job, observed error, evidence that publication did/did not happen,
and the smallest next diagnostic or corrective action. Uncertainty remains
explicit. A retry, edit, cancellation or replacement belongs to separately
authorized execution; never retry blindly or resend a successful platform.
When access or rate limits block inspection, retain records and disclose the
gap. Do not claim failure solely from inaccessible evidence.

## Completion check

- Correct account and review scope are explicit; pagination/coverage is stated.
- Draft, scheduled, provider-reported, platform-verified and manual states remain distinct.
- Potential duplicates are evaluated by identity and purpose, not titles alone.
- Each unresolved item has one next action, owner and evidence gap.
- Existing posts/drafts are untouched by the review; preservation claims match
  the comparisons actually performed.

## Ask ChatGPT

> Review [campaign] for [account] using the Rackagentur “Review publishing status
> without duplicate posts” playbook. Inspect current account-scoped authored jobs
> and relevant published history, follow pagination, and compare exact versions
> with the existing private plan. Distinguish manual Stories, drafts, scheduled
> jobs and verified outcomes. Return evidence, coverage limits and one next action
> per unresolved piece. Preserve all posts, drafts and settings; do not schedule,
> publish, retry, cancel, edit, sync or create monitoring.

## Evidence and roadmap

Source review: Sunday 15.11.2026. Derived from the GGD preparation pilot retained
in DJ Clone: live totals had changed, Story drafts carried placeholder timestamps,
hosted/local asset hashes matched despite differing filenames, and ticket checkout
was rate-limited. The pilot's publishing fields matched on a final reread.
These are historical observations, not current campaign status. Private details
remain in that project. Additional failure/partial-success cases above are
procedure guidance, not claims that the GGD pilot observed them.

PR #5 was merged and its deployment and workflow links verified on 15.11.2026.
The first live read-only status-review session was completed that day against
GGD. Its private DJ Clone record documents account-scoped queue/history coverage,
evidence limits and identical authored records before and after inspection.
The Reel was still scheduled; manual Stories remained drafts. This validates
the initial read-only review, not future publication, manual execution or recovery
from a publishing failure. This documentation update does not refresh those facts.

**Next:** after the existing Reel's scheduled publication, inspect that same job
and its Instagram permalink, then confirm the native Story handoff. Publication
verification and manual Story execution remain pending until supported by their
own evidence. Follow the [roadmap checkpoints](README.md#roadmap-checkpoints).
Once the complete manual cycle is validated, decide whether any recurring check
merits automation; do not add one by default.
