# Research template

A reusable research repository template owned by AC. It provides working rules and record formats for a future independent research campaign. The template itself has no scientific charter or active campaign.

## Start a new repository

1. Create a new independent repository by copying these files into a fresh Git repository. Alternatively, use GitHub's **Use this template** option if the repository has been configured to offer it. Start fresh Git history; do not fork an earlier campaign's history.
2. Set the new repository's name, identity and owner. AC is the default owner and may be replaced consistently in the new repository's rules and records.
3. Read [AGENTS.md](AGENTS.md), [agents/WORKFLOW.md](agents/WORKFLOW.md) and the applicable role file: [Codex](agents/codex/CODEX.md) or [Claude](agents/claude/CLAUDE_ROLES.md). Preserve their research, evidence, audit and branch rules when configuring the new campaign.
4. Review the generic `RS-T` and `RS-N` ID namespaces before allocating any IDs. Keep them or choose campaign-specific namespaces consistently across the rules, registries and templates. Set the cold-storage path for the new campaign before using cold storage.
5. Use the first topic to define the scientific question, scope, assumptions and success criteria, then update [state/CURRENT.md](state/CURRENT.md).

Perform all scientific work in the new repository. Do not turn this reusable template into a scientific campaign; changes here should improve the reusable scaffold.

## Working records

| Location | Purpose |
|---|---|
| `AGENTS.md`, `agents/WORKFLOW.md`, `agents/` | Binding workflow and agent role rules |
| `state/CURRENT.md` | Campaign charter, frontier, priorities and next decisions |
| `state/IDEAS.md` | Ideas, aliases, novelty gates, obstructions and dispositions |
| `PROOF_STATUS.md` | Canonical result IDs, statuses, dependencies and evidence |
| `ID_CROSSWALK.md` | Provisional-to-final ID provenance |
| `PAPER_MAP.md` | Manuscripts and their supporting results |
| `literature/CORPUS.md` | Sources known or supplied, whether read or unread |
| `literature/INDEX.md` | Extracted published statements by claim type |
| `literature/records/` | Source records with hypotheses and page/theorem references |
| `tracks/` | Scientific tracks, theory files and scoped negative results |
| `topics/` | Topic logs, proposals, audits, responses and reproducible checks |
| `templates/` | Reusable records for ideas, results, sources, topics and cold storage |

Registries, topics, scientific tracks and source records start empty. There are no inherited results, ideas, literature statements, scientific IDs or ID reservations. No numerical evidence, priority claim or subject-specific assumption is preloaded. Newly allocated IDs belong to the new repository; external statements require explicit citations.

Before proposing an idea, read `state/IDEAS.md`. Before opening a paper or making attribution or novelty claims, read `literature/INDEX.md`. Follow the preserved workflow for topic branches, evidence, independent audits and owner merges.

## First research prompt

Run this in the new repository after customization:

> Codex (Sol 6.1 xhigh): New topic: define this independent research campaign around <research question>, with <scope and constraints>. Record the charter, assumptions, literature baseline and success criteria, and propose the cheapest decisive first tests before developing new ideas.
