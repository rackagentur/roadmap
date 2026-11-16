# Rackagentur Projects Dashboard

The GitHub Pages dashboard lives in `index.html`. Project data is managed in
`projects.json` rather than hardcoded HTML. Existing radar visuals, cards,
theme toggle and responsive layout remain in place.

## Using the operations hub

Start with the [workflow library](docs/workflows/README.md) when you need a
process, or [Resume a project](docs/workflows/resume-a-project.md) when returning
to work. The dashboard links to both. Playbooks are version-controlled Markdown;
existing project procedures remain in their owning repositories. The library
includes a ready-to-copy ChatGPT prompt for retrieving the same sources.

This is a public navigation layer, not a private task or booking database.
Keep personal handoffs and operational records in their existing private homes.

## Updating the portfolio

1. Check the actual `rackagentur` repositories, README files, milestones,
   release evidence and relevant deployment evidence.
2. Edit the corresponding project record in `projects.json`.
3. For new projects, add a record with a GitHub repository URL, concise
   purpose, development and deployment statuses, next actionable step,
   evidence note and verification date.
4. Do not set `development_status: "Live"` based only on code or a deployment
   URL. Test the deployed app's availability and relevant functionality.
5. Update `verified_on` and per-record `last_verified` **only for facts
   actually inspected**. Do not date-stamp stale evidence as newly verified.
6. Preview from a web server (not `file://`, because the page fetches JSON).
   For example run `python3 -m http.server 8000` in the repo root and
   open `http://localhost:8000`.
7. Check light/dark mode, mobile layout, project count, links and JSON loading
   before merging. Deploy only when authorized.

## Status rules

Development: `Concept`, `Development`, `Testing`, `Live`,
`Maintenance`, `Paused`, `Archived`, or `Unverified`.

Deployment: descriptive evidence-aware status, e.g. `Verified live`,
`Unverified`, `Not released`, `Not applicable`, `Unknown`, or
`Legacy production reported`. The development state does not determine
deployment health automatically.

URLs in `production_url` are **listed addresses** until deployment
verification is recorded; the dashboard labels them as unverified.
Only records with `deployment_status: "Verified live"` get a
"Live site (verified)" link label (the date shows as "Checked"); every other status,
including "Reachable; defects found", keeps "Listed URL (unverified)".

`last_verified` is the date of the specific source review. The
`evidence` field records what supports a classification. Do not infer
application health from commit recency.

## Scope and open questions (baseline 2026-11-13)

- 15 accessible non-dashboard repositories were identified; 17 records
  are displayed because FilterStay and Groundwork exist only as historical
  dashboard entries.
- FilterStay and Groundwork source repositories have not been located.
- Production URLs, including previously marked Live entries, have not been
  newly health-checked. Those links are not proof of deployment.
- Confirm the post-event lifecycle of Big Brother GEEZ.
- The Order of the Keeper is a creative project, included under
  the existing "All Projects" scope rather than treated as an app.
- No CI automation, external API, database or scheduled job is required
  for this first refresh.

Use a short PR for each update and maintain the existing visual identity.
