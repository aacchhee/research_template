# Audit 01 — sync-padua-rules-20261101

**Verdict: ACCEPTED.** No findings require changes. Two non-blocking observations below; neither affects acceptance.

- Auditor: Claude, Opus 5.5 high (protocol/technical audit). Handoff 01 named Sonnet 5.5 high and allowed Opus 5.5 high with a recorded reason. Reason: this session ran on Opus 5.5, and AC's standing preference is that independent reviews run on Opus. Fable was not used; AC did not request it.
- Developer: Codex (delegated gpt-6.1-sol medium; root orchestration gpt-6-astra medium). Auditor and developer are different agents.
- Rules read at branch head `ab3363fa7dcace3f4b069bf5b0c202f4a1ff8688`: AGENTS, WORKFLOW, Claude roles.
- Audited candidate: `0e612234d8a141e87ff98f8c4b2a7d6e2d765dac` (development outputs). Head `ab3363f` differs from it only by `handoffs/01-audit.md` (new) and one LOG line, as stated in handoff 01; verified.
- Destination main at audit time: `d89af8343ebed16dd0b32f30ad2a58d06eac5bb0` (unchanged since the recorded base).
- Source: `aacchhee/padua_research` at `e24b21fe43cdd090f6dfac269147e75185f04c5b`, still Padua's `main` head at audit time.

## Scope

Rules, templates, scaffold documentation and this maintenance topic. Scope exception recorded: the novelty gate, `state/IDEAS.md` full read and scientific reruns do not apply, because the change adds no idea, mechanism, claim, ID, reservation or evidence. No scientific state or registry file changed (verified below).

## Coverage

1. **Full source/destination comparison.** All ten source rule/template files at the pinned SHA (AGENTS; WORKFLOW; Claude roles; Codex roles; COLD_STORAGE, HANDOFF, IDEA, LITERATURE_RECORD, THEORY, TOPIC_LOG templates) were compared with the candidate. The set of files is identical on both sides.
   - Byte-identical: HANDOFF, LITERATURE_RECORD, TOPIC_LOG.
   - Every remaining hunk was checked line by line and maps to exactly one PORT.md adaptation: (1) generic identity/owner in AGENTS title and first paragraph; (2) `PD-` → `RS-` in Claude roles, Codex roles, IDEA, THEORY and WORKFLOW (lines 24, 65, 81, 91, 93, 119), including provisional examples; (3) `Padua-specific` → `campaign-specific` in AGENTS, COLD_STORAGE and WORKFLOW 103, and the owner-chosen local-track folder in WORKFLOW 105; (4) transition heading in WORKFLOW 139; (5) removal of the 2026-10-31 Fable aside and the "AC's L5 decision" label (WORKFLOW 16/93, Claude roles 7) with the rule content retained; (7) the Fable restriction; (8) the squash recommendation in WORKFLOW 149. No unexplained difference remains.
2. **Missed reusable changes.** Files touched by the three source PRs (first-parent diffs for the #8 and #6 merge commits, direct diff for #13) were listed. Outside the compared rule/template set they touched only Padua campaign records (topic logs/audits/handoffs, the batch ALLOCATIONS ledger, `topics/README.md` index rows, registries, literature, tracks). None is reusable rule content; correctly not imported. The template's `topics/README.md` gains a generic handoff sentence and a maintenance section instead.
3. **PR #13 content.** Present in full in AGENTS (short Continue prompt, numbered handoff, immutability) and WORKFLOW (handoff lifecycle, one-open rule, completion/redirect/withdrawn/close, log-exempt case, input-SHA distinction, reservations, scans, priority/collision, transition and reservation-only timing). Coverage follows from item 1: these WORKFLOW passages are byte-identical to source apart from the namespace and transition-heading adaptations.
4. **PR #8 content.** WORKFLOW 105 retains topic-owned `results/<topic-slug>.md`, single-writer ownership, own-section-only RESULTS changes at PR preparation or after merge, staging current bytes, modification-time guard, restage/remerge on rejection, never force, no regeneration from older copies, recovery from topic files and privacy. Only the location changes: an AC-chosen campaign folder, with updates reported as pending until configured. README step 4 states the same. No path is silently selected; no Padua or Downloads path remains in operative files.
5. **PR #6 + AC override "Fable: only when explicitly asked by AC".** Exactly four operative Fable clauses exist, and all four require AC to explicitly request Fable for the particular task: WORKFLOW allocation row (line 16), WORKFLOW scope paragraph (line 18), Claude roles development (line 7), Claude roles audit (line 18). The README sentence agrees. Ideas-campaign scope restriction, the Sonnet 5.5 high script row, the Opus 5.5 xhigh alternative, the unchanged Codex column and developer/auditor separation are intact.
6. **AC override "recommend squash merge by default".** WORKFLOW 149 and README recommend squash by default, let AC choose another method and state that agents never merge. The disposable sequential squash rehearsal sentence is unchanged from source. AGENTS still forbids merging, force-pushing and tag operations; WORKFLOW "Only AC merges" retained.
7. **Template integrity.** Changed paths vs base: AGENTS, README, WORKFLOW, Claude roles, TOPIC_LOG, new HANDOFF, `topics/README.md`, and this topic's LOG/PORT/handoff. Codex roles and the other templates were not touched. `state/`, `PROOF_STATUS.md`, `ID_CROSSWALK.md`, `PAPER_MAP.md`, `literature/` and `tracks/` were unchanged. The maintenance topic is labelled scaffold-only in README and in `topics/README.md`.
8. **Hygiene.** `git diff --check` clean; all relative Markdown links in changed non-template files resolve.

## Commands actually executed

```
git clone --depth 1 https://github.com/aacchhee/research_template
git fetch --depth=50 origin codex/sync-padua-rules-20261101; git fetch origin main   # main = d89af83
GIT_LFS_SKIP_SMUDGE=1 git clone --depth 1 https://github.com/aacchhee/padua_research
git fetch --depth=200 origin main; git fetch origin e24b21fe43cdd090f6dfac269147e75185f04c5b
for f in <10 rule/template files>: git show e24b21f…:$f > src/$f; cmp / diff src/$f $f
git show --name-status e24b21f…; git diff --name-status 9739a0c^1 9739a0c; git diff --name-status a7e1234^1 a7e1234
grep -rniE 'padua|PD-[TN]|Downloads'  (outside this topic: only the topics/README maintenance link)
grep -rni 'fable'; grep -niE 'squash|merge method|never merge|only AC merges'
git diff --name-status d89af83 HEAD; git diff --check d89af83 HEAD; git diff --stat 0e61223 HEAD
python3 relative-link check over changed non-template files
gh api repos/aacchhee/research_template/pulls?head=…   # draft PR #1
```

## Non-blocking observations

- **O1 (pre-existing, out of scope).** Mechanical article artefacts "A RS-N" / "a `RS-N`" in `templates/THEORY.md` line 37 and WORKFLOW 91/93 read "an" in English. They already exist at base `d89af83` and come from the original `PD-` → `RS-` substitution. Not introduced by this port. A later scaffold-maintenance topic may fix them; do not fold them into this PR.
- **O2 (wording, no change requested).** README's Fable sentence says "available"; the binding rule text in WORKFLOW and Claude roles says "allowed only when AC explicitly requests Fable for the particular task". The meanings agree and README is non-binding.

## Limits

This is a protocol and text audit. It does not test the modification-time guard, the reservation procedure or the handoff lifecycle in live use, and it does not re-audit Padua's source rules. Source acceptance rests on Padua's own merged audits.
