# Workflow library

Start with what you want to accomplish. The dashboard remains the project
directory; this index points to reusable procedures and their owning sources.

| I want to… | Start here | When to use it |
| --- | --- | --- |
| Pick up a project again | [Resume a project](resume-a-project.md) | Returning after a break, changing tools, or handing work to another chat |
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

Index source review: Sunday 15.11.2026. Linked documents were inspected during
the operations audit; their procedures were not executed as part of this change.
Gig-promotion and publishing playbooks remain future work, not ready workflows.
