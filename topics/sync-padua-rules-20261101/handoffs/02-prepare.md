# Handoff 02 — sync-padua-rules-20261101 — PR preparation

- Status: done in 14ec5e294157326833b4d4267dde54ae686a24d7
- Previous handoff: 01-audit.md

- Next agent / model / effort: Codex, gpt-6-astra medium
- Role: orchestrator (developer side; PR preparation)
- Branch: `codex/sync-padua-rules-20261101` in `aacchhee/research_template`
- Input head SHA: `530a0ef25def10df1b78275640bd5c61e4a4e3d6` (audit outputs; the commit that publishes this file comes later)
- Main / base: `d89af8343ebed16dd0b32f30ad2a58d06eac5bb0`
- Stage: PR
- Written by / date: Claude, Opus 5.5 high · 2026-11-01

## Task

[audit-01.md](../audit-01.md) ACCEPTED the development candidate `0e612234d8a141e87ff98f8c4b2a7d6e2d765dac` with no required changes. Prepare draft PR #1 for AC's merge decision:

1. Fetch `main` and the topic head. If `main` has moved past `d89af83`, merge `origin/main` into the branch (never rebase or force-push published history), resolve any conflict, and re-run the checks below. If the merge changes any rule or template text, stop: that is a material change and returns to AUDIT under a new numbered handoff.
2. Re-run the scope checks against the base: `git diff --name-status <base> HEAD` lists only the paths audit-01 item 7 accepted, plus this topic's audit/handoff files; `git diff --check` is clean; relative links in changed non-template files resolve; `state/`, `PROOF_STATUS.md`, `ID_CROSSWALK.md`, `PAPER_MAP.md`, `literature/` and `tracks/` are unchanged.
3. Update PR #1's body. The AUDIT section gets the real verdict: ACCEPTED by Claude Opus 5.5 high in audit-01, at the candidate SHA, plus the two non-blocking observations (O1 pre-existing "a RS-N" article artefact at base, out of scope; O2 README Fable wording, no change). The PR section gets the final head SHA, keeps "no range needed", and adds: **recommend squash merge by default; AC chooses the method and alone merges**.
4. Mark PR #1 ready for review (REST: `POST /repos/aacchhee/research_template/pulls/1/ccr/ready_for_review` or the equivalent available route).
5. Record a LOG entry. Then close the topic's work on the agent side: set this handoff to `done in <output-commit-sha>` in a following commit. The only remaining action is AC's merge, so no successor handoff is needed unless AC requests follow-up. Record this in the LOG.

## Read first

AGENTS, `agents/WORKFLOW.md` (Work cycle, PR procedure) and `agents/codex/CODEX.md` at the branch head; this topic's LOG, PORT.md, audit-01.md and handoff 01; PR #1's current body.

## Scope limits

Do not edit rules, templates, README or PORT.md. Any such edit is material and needs re-audit. Do not fix O1 in this PR. No scientific work, ID allocation, local-track writes, `.github`/settings/tag changes or history rewrites. Never merge; only AC merges.

## Acceptance and outputs

- PR #1 is ready (not draft), and its body carries the real audit verdict, final head SHA and squash-by-default recommendation.
- LOG records the preparation checks actually executed and the final head.
- Handoff 02 is closed as described in Task step 5. The reply to AC states that the PR awaits AC's merge and gives no Continue prompt unless work remains.
