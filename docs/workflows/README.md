# Workflow library

Start with what you want to accomplish. The dashboard remains the project
directory; this index points to reusable procedures and their owning sources.

| I want to… | Start here | When to use it |
| --- | --- | --- |
| Pick up a project again | [Resume a project](resume-a-project.md) | Returning after a break, changing tools, or handing work to another chat |
| Choose the right booking or publishing tool | [Tool ownership](tool-ownership.md) | Before preparing promotion, updating booking facts, or scheduling content |
| Prepare promotion for a confirmed gig | [Prepare a GEEZ gig promotion](prepare-geez-gig-promotion.md) | A gig is confirmed, its details change, or its promotion window opens |
| Check publication without duplicating posts | [Review publishing status without duplicate posts](review-publishing-status.md) | A campaign needs a status check, a job is due, or a publishing outcome is unclear |
| Update the dashboard | [Portfolio maintenance](../../README.md#updating-the-portfolio) | A project, verified status, or next action changes |
| Check NoxReach booking intake | [Existing NoxReach runbook](https://github.com/rackagentur/NoxReach/blob/main/tasks/inbound-production-runbook.md) · private | An intake or notification problem needs investigation |
| Resume FOUND development | [Existing FOUND state](https://github.com/rackagentur/found-app/blob/main/tasks/state.md) · private | Establishing the current milestone and remaining gates |
| Understand Flight Control | [Existing project README](https://github.com/rackagentur/flight-control/blob/main/README.md) | Establishing the production/development distinction; then verify the actual working branch |
| Prepare a Big Brother GEEZ release | [Existing release procedure](https://github.com/rackagentur/big-brother-geez/blob/main/docs/release-process.md) · private | Planning an explicitly requested release |
| Understand GEEZ Social booking ownership | [Existing integration documentation](https://github.com/rackagentur/geez-social/blob/main/docs/noxreach-integration.md) · private | Checking integration stages before proposing another booking process |

Private links require repository access. If a source is unavailable, ask for the
relevant excerpt; do not reconstruct it from memory. Documentation describes a
process or recorded state, not proof that an integration is active today.

## Ask ChatGPT

Copy this into the relevant project chat and replace the project name:

> Help me resume [project]. Read the Rackagentur “Resume a project” playbook at
> https://github.com/rackagentur/roadmap/blob/main/docs/workflows/resume-a-project.md
> and the project's current state and handoff documents. Establish the working
> branch and distinguish local, committed, and deployed evidence. Give me the
> last verified checkpoint, open blocker, and one next action with source links.
> If a source is inaccessible or stale, say so. Start with inspection; do not
> interpret this request alone as permission to publish, deploy, or send messages.

ChatGPT retrieves these sources through available connected tools. This link
does not install an integration, synchronize chats, or grant repository access.

## Maintaining this library

- Owner: the repository maintainer; procedure owners remain with their projects.
- Keep one canonical procedure in its owning repository. Add pointers here,
  not copied runbooks or private working records.
- New playbooks include purpose, trigger, inputs, steps, output, verification,
  recovery, next action, owner, and a dated source-review note.
- Review a procedure when its tools, ownership, or outcome changes. Record an
  actual successful use separately from a documentation review.
- This repository and its website are public. Keep personal state, credentials,
  account identifiers, booking details, and private handoffs in their existing
  private homes. Never paste them into this index or public issues.

## Roadmap checkpoints

Checkpoint review: Sunday 15.11.2026. Based on the existing private DJ Clone
preparation pilot and completed publishing-status review; this documentation
update does not refresh live campaign evidence. Private records remain in DJ Clone.

| Milestone | Verified checkpoint | Next action |
| --- | --- | --- |
| Prepare a GEEZ gig promotion | Complete: preparation-only GGD pilot on 15.11.2026, with evidence limits retained privately | Reuse the preparation package and existing jobs |
| Review publishing status without duplicate posts | Complete: first live read-only GGD review on 15.11.2026; authored records matched before and after | Repeat the review against the same job after its scheduled publication |
| Verify publication | Pending: the reviewed Reel was scheduled, with its outcome and Instagram permalink unverified | Inspect provider outcome and the matching Instagram post; retain uncertainty if inaccessible or delayed |
| Complete manual Story handoff and execution | Pending: manual drafts are not proof of publication | After Reel verification, confirm the native Instagram handoff; record execution separately when observed or reported |
| Assess selective automation | Deferred: the complete manual publishing cycle is not yet validated | After publication and manual execution are reviewed, decide whether a recurring check would save effort |

**Next roadmap step:** verify the existing Reel's publication and Instagram
permalink, then confirm its manual Story handoff. Keep exact job references,
timing and execution evidence in the private campaign record. No replacement
posts, new tracker or automation are implied by this checkpoint.

Linked project procedures were inspected during the original operations audit;
the completed GGD sessions above do not establish that every linked procedure
has been executed or that all integrations are active.

### App Store Preparation & Launch

Recorded: Wednesday 18.11.2026. Strategic milestone: prepare several apps for
native iOS distribution **before** enrolling in the Apple Developer Program, so
they can be submitted within the same general launch window. No deadlines are
set. Dashboard data: the `milestones` entry in [`projects.json`](../../projects.json).

| Phase | Status | Scope |
| --- | --- | --- |
| 1 — App Store Readiness Audit | Planned (current) | Inspect each app's implementation, native iOS compatibility, actual App Store requirements and blockers; estimate effort; decide which apps justify publication |
| 2 — Native iOS Preparation | Planned | Prepare approved apps; reuse existing code; keep existing web deployments; only necessary native functionality |
| 3 — Device Testing | Planned | Native builds on iPhone; functionality, offline behaviour, data persistence, backup/migration; fix genuine release blockers |
| 4 — Apple Developer Enrollment | Deferred | Trigger: most selected apps are technically ready for submission. Not initiated automatically |
| 5 — App Store Submission | Planned | Metadata, screenshots and icons, privacy disclosures, App Store Connect, independent review submissions |

| Application | Readiness | Recorded state |
| --- | --- | --- |
| GEEZ FIT | Not audited | Production PWA deployed; exercise demonstrations and appearance selector implemented; latest reported tests 111 passing; native iOS preparation estimated at 3–7 working days (unaudited) |
| NoxReach | Not audited | Existing DJ booking/follow-up app; native iOS readiness unverified |
| Flight Control | Not audited | Existing flight-attendant app; native iOS readiness unverified |
| Placeback | Not audited | Existing review app project; implementation and iOS readiness unverified |

**Next action:** Conduct App Store readiness audits for the four candidate
applications. This entry does not start the audits, native development or
Developer Program enrollment.
