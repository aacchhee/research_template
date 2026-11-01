# Sync merged Padua rules into the reusable template

- Branch: `codex/sync-padua-rules-20261101` · Base: `d89af8343ebed16dd0b32f30ad2a58d06eac5bb0` · Developer: Codex · Auditor: Claude
- Stage: AUDIT · Next: `Claude (Sonnet 5.5 high): Continue codex/sync-padua-rules-20261101.` · Open handoff: [handoffs/01-audit.md](handoffs/01-audit.md)
- Reserved final-ID ranges: no range; scaffold rule maintenance only.
- Scientific claims: none; all scientific registries stay empty and unchanged.
- Open for AC: merge decision after the required independent audit; no storage destination or scientific configuration is selected by this port.

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

## Runs needed

No scientific runs. Required next step is independent Claude protocol audit of the exact candidate and template adaptations under handoff 01. Local working-track updates remain pending because no campaign folder is configured and this template has no scientific campaign.
