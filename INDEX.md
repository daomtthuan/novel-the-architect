# INDEX — Knowledge Graph (v2, optimized)

Retrieval graph only — not narrative, not a procedural guide. This is the **single canonical copy** of the authority table and task matrix; `INSTRUCTIONS.md` and `README.md` both point here instead of repeating them. If this file and a numbered canon/continuity file disagree on a **fact**, the numbered file wins — this file is navigation only, never a source of truth for story facts.

## 0. READ ORDER — NEW CHAPTER

```
1. 29-agent-memory.md          (mutable state — read FIRST)
2. 12-continuity-tracker.md    (durable ledger + handoff protocol)
3. [previous chapter file]     → its Metadata + Continuity Update (do not skip)
4. world_calendar.md           (WC year / age authority)
5. 00-story-bible.md + 01-canon-rules.md
6. 09-season-arc-outline.md    (macro plot position)
7. → branch into §2 TASK MATRIX for domain files
```

## 1. AUTHORITY LAYERS (highest → lowest)

```
L0  Current explicit user instruction
L1  Hard safety constraints (age/romance safety — §6 INSTRUCTIONS.md)
L2  world_calendar.md                    — chronology & age math
L3  00-story-bible.md, 01-canon-rules.md — core canon
L4  95-canon-revisions-archive.md        — ONLY for facts it explicitly revises (historical, MERGED)
L5  Domain canon files (Layer A)
L6  Continuity/state files (Layer B)     — NEVER override canon; record what happened
L7  Creative inference
```

A lower layer may **add** detail but never **contradict** a higher one — if it does, flag it, don't silently resolve it. Filename numbers ≠ authority; layer (A/B/C/D) does.

## 2. TASK → FILE MATRIX

| Task | Primary | Cross-check | Notes |
|---|---|---|---|
| New chapter | `29,12,`prev ch`,world_calendar,00,01,09` | `20,28,`domain | See §0 |
| Character write-up | `03,14,15,16,17` | `04,46,world_calendar` | Never use `03` alone |
| Dialogue / iconic lines | `15,21,46` | `03,14,20` | Locked/Single-Use lines: never reuse casually |
| Character development beat | `03,14,16,19` | `04,42` | |
| Character secret | `17,26,28` | `03,11` | check who-knows/reader-knows split |
| Relationship (general) | `04,37,42` | character files | |
| Romance / fanservice | `34–42` | `03,14,15,16,19` | Iris hard age-gate — §5 |
| Timeline / age math | `world_calendar,02` | `00,12,95` | calendar wins |
| WC16 revision specifics | `95,world_calendar,02` | `00,01` | MERGED, historical only |
| City name / WC16 Demon fate | `95,05,22,26,28` | `27,29` | MERGED, historical only |
| Event continuation | `18,20,28` | `12,19,21` | |
| Emotional aftermath | `19,20` | `14,16,42` | |
| Location | `05,22` | `06,20` | |
| Organization / faction | `06,23` | `05,18` | |
| Artifact | `24,07` | `05,25` | Never plot-solve w/o origin/cost/limits |
| Technology | `07,25` | `06,18` | Must have social consequence |
| Magic rules | `07` | `05,08` | |
| Builder / Architect lore | `08,11,26,28` | `17,02` | Reveal-timing gated — `11` |
| Mystery work | `11,26,28` | `17,18,20` | Never resolve for a twist |
| Antagonist / conflict | `27,06,18,28` | `14,17` | |
| OST | `43,44` | `19,20,ost/` | No "Season 3" anywhere |
| Character design / visuals | `30,31,32` | `03,world_calendar,character_design/` | |
| Illustration planning | `30,31,32,33` | design + timeline | Don't claim a generated image without generating it |
| New canon decision | `00,01,world_calendar,29` | domain + `95` | Create next `NN-session-update-*.md`; never edit `95` |

## 3. FILE REGISTRY (by layer)

### Layer A — CANON (defines what is true)

| File | Governs | Key dependents |
|---|---|---|
| `00-story-bible.md` | Premise, aging system, romance direction, theme | almost everything |
| `01-canon-rules.md` | Hard constraints | `13,34–41`, all character work |
| `02-timeline.md` | Detailed narrative timeline | `12,20,29`, chapters |
| `03-characters.md` | Identity/profile | `10,13,14,15,16,17` |
| `04-relationships.md` | Relationship network | `37,42`, romance files |
| `05-world.md` | Peoples, world identity, city Elena | `22,06,25` |
| `06-factions-and-politics.md` | Political baseline, factions | `23,27,18` |
| `07-magic-and-technology.md` | Magic rules, Ark stages | `08,24,25` |
| `08-multiverse-and-quantum-lore.md` | Builder/Architect distinction | `11,26,28,17` |
| `09-season-arc-outline.md` | Macro structure | `13,12` |
| `14-character-psychology.md` | Need/fear/defense per char | `13,15,16` |
| `15-character-voice.md` | Speech patterns | `13,21,46` |
| `16-character-development-log.md` | Chronological development | `13,12` |
| `17-character-secrets.md` | Who knows what, reveal windows | `11,26,13` |
| `22-location-registry.md` | Location facts | `05,20` |
| `23-organization-registry.md` | Org facts | `06,18` |
| `24-artifact-registry.md` | Artifact facts | `07,05` |
| `25-technology-evolution.md` | Tech stage progression | `07,06,18` |
| `26-mystery-board.md` | Mystery state machine | `11,28,17` |
| `27-conflict-and-antagonist-board.md` | Antagonist/conflict state | `06,18,28` |
| `36-secondary-heroines.md` | Iris/Seraphine/Isolde arcs | `34–42` |
| `43-ost-reference.md` | Track meaning | `44` |

### Layer B — CONTINUITY / STATE (never overrides Layer A)

| File | Governs | Update trigger |
|---|---|---|
| `12-continuity-tracker.md` | Per-chapter ledger + handoff protocol | Every accepted chapter |
| `18-event-consequence-map.md` | Event → downstream consequence | New permanent event |
| `19-emotional-memory.md` | Lasting emotional beats | Emotional consequence established |
| `20-scene-memory.md` | Required/established permanent scenes | New canonical scene |
| `21-dialogue-memory.md` | Thematic-anchor dialogue | Genuinely iconic line spoken |
| `28-unresolved-threads.md` | Open questions, per-installment | Thread opened/advanced/resolved |
| `29-agent-memory.md` | Current mutable working state (READ FIRST) | Every accepted chapter |
| `31-illustration-registry.md` | Generated/planned illustrations | Image generated |
| `42-romance-continuity-memory.md` | Romantic interaction log | Romance beat occurs |
| `44-ost-continuity.md` | Track usage/lock state | OST actually used |

### Layer C — PROCEDURE (stable, rarely changes)

`10-light-novel-writing-guide.md` · `11-foreshadowing-and-revelations.md` · `13-chapter-generation-protocol.md` · `32-image-generation-protocol.md` · `33-reader-immersion.md` · `34-romance-harem-fanservice.md` · `35-romance-subplot-engine.md` · `37-relationship-state-machine.md` · `38-romance-integration-by-season.md` · `39-fanservice-scene-library.md` · `40-romance-foreshadowing-map.md` · `41-romance-agent-rules.md` · `46-iconic-dialogue-registry.md`

### Layer D — EXTERNAL / ASSET

| File / dir | Role |
|---|---|
| `world_calendar.md` | MASTER chronology + age authority — wins all date/age conflicts |
| `README.md` | Short onboarding pointer to this file (no duplicated tables) |
| `character_design/*.png` | Visual reference assets |
| `ost/*.mp3` | Audio assets (meaning lives in `43`/`44`) |
| `95-canon-revisions-archive.md` | MERGED historical revision record — WC16 rewrite, races, city rename, WC16 Demon fate, Season-3 typo fix (replaces old `45`+`47`) |

### Layer E — OUTPUT

`chapters/*.md` — generated chapters; each has Metadata + Continuity Update used as the next chapter's handoff.

## 4. DEPENDENCY GRAPH

```
world_calendar.md ──► 02-timeline.md ──► 12-continuity-tracker.md ──► chapters/*
        │                                        │
        ▼                                        ▼
00-story-bible.md ◄── 01-canon-rules.md   29-agent-memory.md (mutable mirror of 12)

03-characters.md ──► 14-character-psychology.md ──► 15-character-voice.md
        │                     │                            │
        ▼                     ▼                            ▼
16-character-development-log.md          21-dialogue-memory.md ──► 46-iconic-dialogue-registry.md
        │
        ▼
17-character-secrets.md ──► 26-mystery-board.md ──► 11-foreshadowing-and-revelations.md ──► 28-unresolved-threads.md

04-relationships.md ──► 37-relationship-state-machine.md ──► 42-romance-continuity-memory.md
        │                                                              ▲
        ▼                                                              │
34-romance-harem-fanservice.md ──► 36-secondary-heroines.md ──► 35/38/39/40/41

05-world.md ──► 22-location-registry.md
06-factions-and-politics.md ──► 23-organization-registry.md ──► 18-event-consequence-map.md
07-magic-and-technology.md ──► 24-artifact-registry.md
07-magic-and-technology.md ──► 25-technology-evolution.md
07-magic-and-technology.md ──► 08-multiverse-and-quantum-lore.md ──► 26-mystery-board.md
18-event-consequence-map.md ──► 19-emotional-memory.md ──► 20-scene-memory.md
30-visual-bible.md ──► 31-illustration-registry.md ──► 32-image-generation-protocol.md ──► 33-reader-immersion.md
43-ost-reference.md ──► 44-ost-continuity.md
95-canon-revisions-archive.md ──► (corrections feed into) 00,01,02,03,04,05,06,14,15,18,19,20,22,23,26,27,28,29,43
```

`A ──► B` = _B must stay consistent with A; check A before writing B-type content._

## 5. HARD CONSTRAINTS (never violate regardless of file conflicts)

- Protagonist has **no personal name**, ever.
- **Iris**: age = WC−3. No romantic/attraction framing before ~WC21. WC15 intro (age 12) strictly platonic.
- **Elena** dies WC35, same day Son is born. Never resurrected. Never passive.
- **"Builder" ≠ "Architect."** Title earned only by preserving Elena's agency at WC35.
- **The Unburied One** (WC16 Demon): connection to WC33-35 stays backstage until Movie 1 at earliest.
- **No "Season 3"** anywhere — saga is Season 1 + Movies 1–4 only.
- City = plain **"Elena"** post-WC35; pre-WC35 informal "Architect's City" nickname, privately disliked, never adopted.
- Chapter prose target: **3,000–3,500 words** (center ~3,250; range 2,800–3,700), Vietnamese prose / English title.
- `95-canon-revisions-archive.md` is **MERGED, historical** — never re-apply as a live instruction; facts already live in numbered canon files.
- The Architect permanently loses his **left arm at WC16** — visual/prose canon from WC16 onward.

## 6. NEW SESSION-UPDATE FILES

Create `NN-session-update-<topic>.md` (next sequential number) for a new canon decision not yet fitting an existing file. Never edit `95-canon-revisions-archive.md` directly — append a new session-update file instead, then propagate its facts into the numbered canon/continuity files and add it to §3 Layer D above.

## 7. MINIMAL VS FULL RETRIEVAL

- **Minimal** (simple continuation, no new lore/romance/political content): `29 → 12 → prev chapter → world_calendar → relevant 03/14/15` for characters present. Stop there.
- **Full** (new lore, location, relationship shift, mystery clue, or major event): walk the full §2 row(s) plus §4 graph edges one hop out.

Never load every file by default — this index exists precisely so that doesn't need to happen.
