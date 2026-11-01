# Sync merged Padua rules into the reusable template

- Branch: `codex/sync-padua-rules-20261101` · Base: `d89af8343ebed16dd0b32f30ad2a58d06eac5bb0` · Developer: Codex · Auditor: Claude
- Stage: PR · Assigned agent work complete; next: AC's merge decision · Open handoff: none
- Reserved final-ID ranges: no range; scaffold rule maintenance only.
- Scientific claims: none; all scientific registries stay empty and unchanged.
- Open for AC: merge decision (audit-01 ACCEPTED; squash recommended by default); no storage destination or scientific configuration is selected by this port.

## 2026-11-01 — Codex development and integration

- Rules read at destination base `d89af8343ebed16dd0b32f30ad2a58d06eac5bb0`: AGENTS, complete WORKFLOW, Codex role. Source rules are pinned at Padua merged main `e24b21fe43cdd090f6dfac269147e75185f04c5b`.
- AC: "pr13 is merged. check now aacchhee/research-template and update its rules with everything from padua that differs, that is pr13 and one of previous prs". GitHub 404 for the hyphenated name was resolved by repository discovery: the intended repository is `aacchhee/research_template`.
- Compared all rules/roles/templates. Three missing reusable amendments found: Padua PR #13 (handoffs/reservations), #8 (local results guards), #6 (Fable allocation). Other differences are intentional template identity, namespaces and historical labels. Scope/provenance and all normalizations: [PORT.md](PORT.md).
- Delegated bounded five-file development to `port_template_rules`, requested `gpt-6.1-sol medium`, with disjoint ownership and no Git authority. Root owns README, maintenance records, verification and Git. Runtime-resolved model/effort metadata is not separately exposed. No cross-agent self-approval is claimed.
- Changes: AGENTS, WORKFLOW, Claude roles, TOPIC_LOG; new HANDOFF; README/topic index explain setup and maintenance-only records. Configurable local folder replaces Padua's path. No source campaign records or concrete scientific IDs are imported; no shared frontier or scientific registry change.
- Novelty gate: not applicable to rule/template maintenance; no mechanism, scientific claim, literature priority or result status added. No scientific runs or generated research artifacts.
- Independent Claude audit remains PENDING. The accepted Padua audits and developer/root comparison checks are source provenance and supplemental verification, not destination audit acceptance.

## 2026-11-01 — AC steering: Fable requires an explicit request

- AC: "Fable: only when explicitly asked by AC". This overrides the source's general Fable permission. The developer applies a task-specific explicit-request condition consistently to the workflow allocation row/scope paragraph and Claude's development/adversarial idea-check instructions. Existing Opus/Sonnet allocations and independent-auditor separation remain intact.
- This additional intentional source difference is recorded in PORT.md and will be an explicit acceptance criterion in the new audit handoff. No prior numbered handoff exists yet to supersede; this instruction is incorporated in handoff 01 when published.

## 2026-11-01 — AC steering: recommend squash merge by default

- AC: "and I'd rather recommend squash.merge by defaULT." The default is a recommendation for ready PRs; AC may choose a different method. WORKFLOW and README state that default and preserve the ban on agent merges. The existing disposable sequential squash rehearsal requirement remains unchanged.
- This explicit override to Padua's categorical merge-method sentence is recorded in PORT.md and in the first audit handoff; no source omission or assumed permission to merge is implied.

## 2026-11-01 — Verification and audit preparation

- Full pinned source comparison re-run after Fable steering. All remaining source differences match PORT.md's explicit generic adaptations and AC overrides; Codex roles and all six templates match source after namespace normalization, with HANDOFF/TOPIC_LOG byte-identical.
- Actual Python assertions pass: all four Fable permission clauses require a task-specific AC request; squash is recommended by default with AC choice and no agent merges; rehearsal policy retained; no concrete Padua namespace/path leaks into operative rules/templates; only authorized scaffold/maintenance paths change, preserving every scientific registry/state file. `git diff --check` passes.
- Independent Claude protocol audit is the next step. Prepare a draft PR with complete source provenance, both AC overrides and a numbered handoff pinned to the completed development commit. No range or allocation ledger is needed.
- Development outputs committed at `0e612234d8a141e87ff98f8c4b2a7d6e2d765dac`. [Handoff 01](handoffs/01-audit.md) requests independent Claude review of that exact input and both AC overrides; publication adds only handoff/log metadata. No draft-readiness or audit-acceptance claim is made.

## 2026-11-01 — Claude independent protocol audit

- Rules read at branch head `ab3363fa7dcace3f4b069bf5b0c202f4a1ff8688`; audited candidate `0e612234d8a141e87ff98f8c4b2a7d6e2d765dac`; destination main still `d89af83`, Padua main still `e24b21f`.
- Auditor: Claude Opus 5.5 high (handoff allowed Opus with reason; AC prefers Opus for independent reviews). Fable not used, not requested.
- [audit-01.md](audit-01.md): **ACCEPTED**. All ten rule/template files were compared with the pinned source; every residual difference maps to a PORT.md adaptation. All four Fable clauses require an explicit task-specific AC request. Squash is recommended by default, AC chooses the method, agents never merge, and rehearsal is retained. No Padua path leaks, and no scientific state changes. Two non-blocking observations: a pre-existing "a RS-N" article artefact at base, and README's non-binding Fable wording.
- Novelty gate and reruns not applicable (administrative scope). Stage set to PR; [handoff 02](handoffs/02-prepare.md) asks Codex to refresh main, validate and mark the PR ready for AC.

## Runs needed

No scientific runs. Final publication and closure follow the checks below; only AC's merge decision remains after publication. Local working-track updates remain pending because no campaign folder is configured and this template has no scientific campaign; no local write is part of this scaffold update.

## 2026-11-01 — Codex PR preparation

- AC invoked handoff 02 with `Codex (gpt-6-astra, medium): Continue codex/sync-padua-rules-20261101.` No scope override. Requested model/effort: gpt-6-astra medium; resolved runtime metadata unexposed. Rules/log/handoff read at refreshed branch head `f698099ca77d7d3d026c52150c5bbcc9e29b4e71`; rules match the earlier development candidate.
- Refreshed main and topic. Main is still `d89af8343ebed16dd0b32f30ad2a58d06eac5bb0`; no merge or rule/template change is needed. Claude audit outputs are `530a0ef25def10df1b78275640bd5c61e4a4e3d6`; published audit/handoff head is `f698099ca77d7d3d026c52150c5bbcc9e29b4e71`.
- Read audit-01: ACCEPTED by Claude Opus 5.5 high for candidate `0e612234d8a141e87ff98f8c4b2a7d6e2d765dac`. No findings need a response. Preserve O1 (pre-existing article artefacts, out of scope) and O2 (consistent README Fable wording, no change requested); neither is fixed or reopened here.
- Re-executed checks: all 12 changed paths at the audit head are accepted scaffold/maintenance paths; scientific state/registries/literature/tracks and .github match main exactly; all seven accepted scaffold files plus PORT.md match the audited candidate byte for byte; actual relative links resolve; all four operative Fable clauses require an explicit task-specific AC request; squash is recommended by default with AC choice and no agent merges; exactly one open preparation handoff; clean tree; `git diff --check origin/main HEAD` passes.
- Destination's only open PR is #1; no IDs are reserved or assigned, no allocation ledger is needed, and scientific registries remain empty. This is single-PR scaffold work, so the batch-only sequential rehearsal obligation does not apply. No scientific execution or local-track write is claimed.
- Final delivery changes only this LOG and handoff 02's status after the real output commit exists. Accepted rules/templates/README/PORT and the audit report remain unchanged, so no material-change re-audit is needed. Push the checked head, refresh PR #1's WORK/AUDIT/PR body and mark it ready for review. Recommend squash merge by default; AC chooses the method and alone merges.
- Preparation output commit: `14ec5e294157326833b4d4267dde54ae686a24d7`. Handoff 02 closes against that real existing commit in this subsequent publication commit. No successor is needed: all assigned agent work is complete and only AC's merge decision remains. The final publication head is recorded in PR #1; it differs from the accepted audit head only in preparation LOG entries and this handoff status.
