# Handoff 01 — sync-padua-rules-20261101 — independent protocol audit

- Status: open
- Previous handoff: none
- Next agent / model / effort: Claude, Sonnet 5.5 high (protocol audit; auditor may choose Opus 5.5 high with a recorded reason)
- Role: independent auditor and handoff orchestrator
- Branch: `codex/sync-padua-rules-20261101` in `aacchhee/research_template`
- Input head SHA: `0e612234d8a141e87ff98f8c4b2a7d6e2d765dac` (development outputs; the next publication commit adds this handoff and log metadata only)
- Main / base: `d89af8343ebed16dd0b32f30ad2a58d06eac5bb0`
- Source main: Padua `e24b21fe43cdd090f6dfac269147e75185f04c5b`
- Stage: AUDIT
- Written by / date: Codex · 2026-11-01; delegated rule developer requested gpt-6.1-sol medium; root orchestration requested gpt-6-astra medium; runtime metadata unexposed

## Task

Audit the portable rule synchronization from merged Padua PRs #13, #8 and #6. Do not treat Padua's accepted audits or the developer/root checks as acceptance of this destination port. AC's two follow-up instructions override the source:

1. "Fable: only when explicitly asked by AC" — verify all four operative Fable permission clauses in WORKFLOW and Claude roles require AC to explicitly request Fable for the particular task. Conceptual ideas-campaign scope, Sonnet scripts, Opus allowance and independent auditing must remain intact. Do not use Fable for this audit; AC has not requested it.
2. "and I'd rather recommend squash.merge by defaULT." — verify squash merge is recommended by default, AC can choose another method, the agent-merge ban remains, and disposable sequential squash rehearsal is retained.

Refresh destination main/topic and inspect the exact candidate diff. Read PORT.md's complete comparison and all eight intentional adaptations. Compare all source/destination agent rules and templates at the pinned Padua source, confirming there are no missed reusable changes or campaign-specific imports. In particular:

- PR #13: full numbered-handoff lifecycle and short continuation prompt, immutable earlier bodies, active/completion/redirect/terminal cases, generic input SHA; fresh reserved ranges, closed/retired scans, priority/collision repair, rechecks, transition and reservation-only timing.
- PR #8: topic-owned local results, own-section-only shared RESULTS changes at preparation/post-merge, staging current bytes and modification-time guard/retry, recovery and privacy. Generic owner-configured folder must replace Downloads/Padua; no path is silently selected.
- PR #6: Fable clauses across workflow/roles, restricted by the explicit AC instruction above.
- Preserve generic owner/identity, RS-T/RS-N namespaces, empty scientific registries, unrelated templates and independent campaign status. Maintenance records are clearly separated from future campaign records.

Write `topics/sync-padua-rules-20261101/audit-01.md` with ACCEPTED or CHANGES REQUIRED, model/effort, exact coverage, commands actually executed, findings and limits. Propose exact fixes for actual issues; do not silently edit developer rules and approve them yourself. No scientific novelty gate/reruns are required for this administrative scope, but explicitly record the scope exception.

## Read first

Destination AGENTS, WORKFLOW and Claude role at the candidate; README; both role files; every template; this topic's LOG and PORT. Source equivalents from `aacchhee/padua_research` at the full pinned SHA. Source PR links and merge identities are in PORT.md.

## Scope limits

Rules, templates, scaffold documentation and this maintenance topic only. No scientific work, state/registry/ID allocation, Padua changes, actual local-track writes, other-topic changes, .github/settings/tag changes or published-history rewrite. No range is needed. Only AC merges; recommend squash merge by default, with AC's method choice preserved.

## Acceptance and outputs

- Audit report and LOG entry; update the draft PR's AUDIT section with the real verdict.
- If findings exist, set WORK and publish `02-response.md` for Codex with exact findings and acceptance criteria. Material fixes require re-audit.
- If accepted, set PR and publish `02-prepare.md` for Codex to refresh main, validate final scope/links and mark the PR ready for AC review.
- Commit outputs first, then in a following commit change only this file's status to `done in <output-commit-sha>` and open the next numbered handoff. Preserve this instruction body and exactly one open successor while work remains.
- Push the handoff before replying. Use the short next-agent Continue prompt.
