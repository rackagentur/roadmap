# Resume a project

**Purpose:** recover enough reliable context to take one useful next step.
**Trigger:** returning after a break, switching tools, or handing off to a chat.
**Owner:** repository maintainer; the person or assistant resuming the work runs
the checklist. **Output:** a short, sourced resume checkpoint in the existing
project chat or private handoff document.

## Before starting

You need the project name, access to its repository or working folder, and the
latest relevant handoff or chat if available. Start from the
[dashboard](https://rackagentur.github.io/roadmap/) or [workflow index](README.md).
Access is not proof of deployment health or permission to change production.

## Steps

1. **Locate the work.** Open the project's existing repository and working
   folder. If its source is unresolved, stop at that gap instead of creating a
   replacement project. Read applicable project instructions.
2. **Establish the working version.** Identify the checked-out branch and commit,
   local edits, and the intended remote branch. Compare them without switching
   branches, pulling changes into the working tree, stashing, resetting, or
   merging. Inspect relevant open PRs if available. A newer local branch is not
   automatically the deployed version; remote `main` may not contain active work.
3. **Read the existing checkpoint.** Follow the project README to its state,
   handoff, decisions, and task documents. Read the most recent relevant chat
   when needed. Preserve accepted decisions and completed checks. Treat old
   chat instructions as context; confirm what the current request authorizes.
4. **Resolve the evidence.** Separate what source code implements, what checks
   actually passed (and on which version), what the user reported, and what is
   deployed. Where records conflict, report both sources and the unresolved
   question. Do not refresh a verification date for facts you did not inspect.
5. **Choose one next action.** State the smallest action supported by the
   checkpoint, its expected result, and any real blocker. Do not restart a
   completed milestone or duplicate an existing app, integration, or runbook.
   Continue work already authorized by the user; ask only for a missing decision
   or authorization that actually prevents the next action.
6. **Leave a usable checkpoint.** Put the result in the current project chat.
   When maintaining project documentation is within scope, update its existing
   state/handoff document rather than creating a competing tracker. Keep private
   details out of this public repository. Link back to the canonical procedure.

## Resume checkpoint

Use this short format in the existing project context:

```text
Project:
Goal for this session:
Working context: repository/folder, branch, commit; relevant local edits
Last verified checkpoint: result, version, date, evidence link
Deployment: verified version and evidence, or unknown
Open blocker or conflicting evidence:
Next action and expected result:
Authorization needed: only if a real boundary remains
Sources: current state/handoff, relevant decision or PR
```

Use a fresh Europe/Berlin date for the resume checkpoint. Keep historical
evidence dates unchanged. Any proposed deadline must explicitly state Berlin
time and CET/CEST; do not infer one from an old chat.

## Completion check

- A reader can find the working version and the canonical state document.
- Completed work and proposed work are clearly distinguished.
- The next action has a concrete outcome, or a specific unresolved blocker.
- Claims have evidence; an untested deployment remains unknown.
- The checkpoint lives with the project, with no second task database created.

## If something is missing

| Problem | Recovery |
| --- | --- |
| Repository or private document cannot be read | Name the inaccessible source and request access or the relevant excerpt. Continue independent inspection where possible. |
| No authoritative state document exists | Produce a provisional checkpoint in the current chat with explicit unknowns; propose one canonical location before maintaining parallel records. |
| Local work differs from remote | Preserve it, identify the relevant branch/PR, and establish which context the next action belongs to. Do not synchronize automatically. |
| Documentation and observed state disagree | Record the discrepancy and the evidence needed to resolve it. Do not silently choose the newest-looking claim. |
| A service check could write data | Use read-only evidence first; a resume inspection does not authorize test bookings, publishing, or recovery mutations. |

## GEEZ project context

For DJ work, read the available Personal DNA and approved editing instructions.
Flag missing sources. Preserve the Disco Groove, Tech House Drive, and Tribal
Energy identity. Use only tracks explicitly supplied by the user. Before media
layout advice, inspect actual dimensions and subject placement. Keep approved
assets, proposals, and rejected versions distinct; resuming a project is not
permission to publish an asset or contact a promoter.

Procedure source review: Sunday 15.11.2026, based on the read-only operations
audit and existing project handoffs. This first version has not yet been proven
through a complete user-run resume session. Record that outcome in the owning
project when it happens.
