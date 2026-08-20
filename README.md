# The Architect — AI Write Agent Knowledge Base

Version: 10 (optimized — deduplicated against `INDEX.md`)

This directory is the complete knowledge base and asset library for **The Architect**.

## Start here

1. **`INDEX.md`** — the retrieval graph. Read order, authority-layer table, task→file matrix, full file registry by layer, dependency graph, hard constraints. This is the **only copy** of those tables in the project — `INSTRUCTIONS.md` and this file both point here instead of repeating them.
2. **`INSTRUCTIONS.md`** — the agent orchestrator: procedural rules, writing workflow, and the *reasoning* behind each rule (INDEX gives you the lookup, this gives you the "why" and "how").
3. **`PROMPT.md`** — task-specific instructions used when generating a new chapter (chapter + continuity-update-package format).
4. **`world_calendar.md`** — master chronology; wins all date/age conflicts. `02-timeline.md` supplies narrative context around it.
5. **`chapters/`** — generated output. Read the previous chapter's Metadata + Continuity Update before writing a new one (see `12-continuity-tracker.md`'s handoff protocol).

## Authority model (short form — full table in `INDEX.md` §1)

User instruction > hard safety > `world_calendar.md` > `00`+`01` core canon > `95-canon-revisions-archive.md` (only for facts it explicitly revises) > domain canon > continuity/state > creative inference. `29-agent-memory.md` is mutable state, never superior canon. `INDEX.md` itself carries no authority — it's a navigation aid; if it and a numbered file disagree on a *fact*, the numbered file wins.

## File groups (see `INDEX.md` §3 for the authoritative per-file table)

- **Core canon (Layer A):** `00–09` foundation files, `14–17` character intelligence, `22–27` world/plot registries, `36` secondary heroines, `43` OST reference.
- **Continuity/state (Layer B):** `12,18,19,20,21,28,29,31,42,44` — record what happened; never override canon.
- **Procedure (Layer C):** `10,11,13,32–41,46` — how to write; not canon-establishing.
- **Visual system:** `30-visual-bible.md`, `31-illustration-registry.md`, `32-image-generation-protocol.md`, `33-reader-immersion.md`, `character_design/*.png`.
- **Romance/fanservice:** `34–42`. Core romance is Architect × Elena unless the user explicitly changes canon. Do not read only one file — combine the relevant set per `INDEX.md` §2.
- **OST:** `43-ost-reference.md` (meaning) + `44-ost-continuity.md` (usage state) + `ost/*.mp3` (assets — meaning lives in the `.md` files).
- **Canon revision history:** `95-canon-revisions-archive.md` — MERGED historical record (WC16 rewrite, Empire of Veyrand correction, new races, city rename to "Elena," WC16 Demon fate as "The Unburied One," the "Season 3" typo fix). Its facts already live in the numbered canon files; treat it as provenance only. Future new decisions go in a new `NN-session-update-*.md`, never edited into `95` directly — see `INDEX.md` §6.
- **Iconic dialogue:** `46-iconic-dialogue-registry.md` — combine with `15` and `21` for callbacks; never casually alter a LOCKED line.

## Important canon reminders (full detail in `INDEX.md` §5)

No personal name for the protagonist · "Builder" ≠ "Architect" · Elena dies WC35, same day as the Son's birth, never resurrected · Iris: no romantic framing before ~WC21 · no "Season 3" · city = plain "Elena" post-WC35 · Architect permanently loses his left arm at WC16 · chapter target 3,000–3,500 Vietnamese words.

## Self-correction on misretrieval

If you're unsure which file to open, have lost track of which source wins a conflict, are loading files broadly without a plan, or don't know whether a fact belongs in canon vs. continuity vs. nowhere — stop and consult `INDEX.md` §1–2 before continuing. This is an internal navigation step; it doesn't need to be narrated to the user.
