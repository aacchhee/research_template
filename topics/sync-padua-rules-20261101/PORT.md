# Padua rule synchronization — provenance and scope

This is template maintenance only. No scientific campaign, claim, result, literature entry, ID reservation or local storage destination is introduced.

- Destination: `aacchhee/research_template`, base `d89af8343ebed16dd0b32f30ad2a58d06eac5bb0`.
- Source: `aacchhee/padua_research`, merged main `e24b21fe43cdd090f6dfac269147e75185f04c5b`.
- Branch: `codex/sync-padua-rules-20261101`.
- AC requested all differing Padua rules, identifying the merged PR #13 and an earlier rule PR. Repository discovery confirmed the destination uses an underscore, not a hyphen.

## Complete reusable-rule comparison

Compared AGENTS, all three agent role/workflow files, and all templates against the pinned source. Existing Codex roles, proof/status/negative-result policy and the IDEA, THEORY, LITERATURE_RECORD and COLD_STORAGE templates already agree after substituting the generic namespaces and campaign-specific storage wording.

| Missing source change | Portable update |
|---|---|
| [Padua PR #13](https://github.com/aacchhee/padua_research/pull/13), merged `e24b21f` | Numbered immutable handoff instructions, short Continue prompt, active/completed/redirect/withdrawn lifecycle, log-exempt and terminal cases; permanent fresh-range reservations, open/closed/retired scans, per-namespace maxima, priority/collision handling and transition away from single-owner prose. AGENTS, WORKFLOW, new HANDOFF template and TOPIC_LOG fields updated. |
| [Padua PR #8](https://github.com/aacchhee/padua_research/pull/8), merged `9739a0c56b7a3976422ce60a8441bfbbfd6554df` | Topic-owned local `results/<topic-slug>.md`; only the topic's section enters shared RESULTS at PR preparation or after merge. Stage current bytes, merge and use the modification-time guard; restage/remerge on rejection, never force. Restore lost sections from their topic files and keep private/third-party text outside Git. |
| [Padua PR #6](https://github.com/aacchhee/padua_research/pull/6), merged `a7e123476cef761807c69e5d0af1a094c7ac3df0` | Fable 5.1 xhigh for conceptual ideas campaigns and adversarial idea checks, **only when AC explicitly requests Fable for the task**, per AC's instruction during this port. The existing Sonnet script-development allocation and independent-auditor requirements are retained. WORKFLOW and Claude roles updated. |

## Intentional template adaptations

1. Preserve the existing generic repository identity, configurable owner and independent-campaign requirement in AGENTS. Do not import the Padua repository name or charter.
2. Substitute `RS-T`/`RS-N` for `PD-T`/`PD-N`, including provisional examples. This copies allocation policy, not any actual IDs or ranges.
3. Retain `campaign-specific` cold storage. Replace the source's `Downloads\padua` local-results folder with an owner-chosen campaign folder outside Git; until configured, updates remain pending. All write ownership, section scope, timing, modification-time guard, retry/recovery and privacy clauses are retained.
4. Use `Transition (when adopting this procedure)` rather than falsely assigning the source's 2026-11-01 adoption date to every future campaign. All transition instructions are retained.
5. Omit Padua's historical Fable authorization aside and `AC's L5 decision` label from operative rules. Preserve the permissions and complete negative-result policy. Source dates and attribution are recorded here instead.
6. HANDOFF and TOPIC_LOG are copied byte for byte. Existing generic roles/templates receive no unrelated edits. README and the topic index explain customization and distinguish scaffold maintenance from scientific records.
7. AC's follow-up instruction, "Fable: only when explicitly asked by AC", takes precedence over the source's general allowance. The WORKFLOW table/scope paragraph and both Claude development/audit instructions require an explicit task-specific AC request before using Fable. This is a deliberate policy restriction, not an omission from the source comparison.
8. AC also requested a default recommendation for squash merge. Replace the source's categorical squash-merge sentence with a recommendation by default, allow AC to choose another method, and retain the prohibition on agent merges. Keep the local sequential squash rehearsal obligation unchanged.

The Padua audits establish the source's accepted protocol scope. They do not constitute a Claude audit of these template adaptations. The destination PR remains draft until the independent handoff is completed.

## Verification scope

Developer: delegated Codex `gpt-6.1-sol medium` for five disjoint rule/template files, as required by the destination's development allocation. Root Codex owns scope, all Git operations, README/topic metadata, source comparisons and PR delivery. Resolved runtime metadata beyond the requested configurations is not independently exposed. The developer's self-check and root's comparisons supplement the required independent Claude audit.

Checks: full source/destination rule inventory with explicit normalizations; exact copies for HANDOFF/TOPIC_LOG; generic namespace/path scan; unchanged scientific registries and all unrelated base files; actual local links outside placeholder templates; Markdown whitespace diagnostics. No scientific tests or runs are needed or claimed for the documentation-only port. No local results folder has been selected or written, and no modification-time guard implementation or concurrency execution is claimed.

## Reproduce the source comparison

Fetch Padua main at the full source SHA, then read source files with `git show e24b21fe43cdd090f6dfac269147e75185f04c5b:<path>`. Compare them with the destination AGENTS, `agents/WORKFLOW.md`, both role files and every file under `templates/`. Apply only the eight adaptations above; any other remaining difference requires disposition. Verify preservation with `git diff --name-only d89af8343ebed16dd0b32f30ad2a58d06eac5bb0 HEAD` and `git diff --check`. The exact auditable candidate commit is supplied by handoff 01 after the output commit exists.
