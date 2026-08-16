# INDEX — Knowledge Graph for AI Write Agent (v1)

## Purpose

This file is a **retrieval graph**, not narrative content and not a replacement for `INSTRUCTIONS.md` or `README.md`.

It exists so the agent can answer, in one lookup, three questions:

1. **What file do I need for task X?** → see §2 TASK → FILE MATRIX
2. **What is this file's authority level, and what can override it?** → see §1 AUTHORITY LAYERS and §3 FILE REGISTRY
3. **What other files does this file depend on / feed into?** → see §4 DEPENDENCY GRAPH (edges)

Read `INSTRUCTIONS.md` for full procedural rules. Read this file when you need fast graph traversal instead of re-reading `INSTRUCTIONS.md` in full every time.

---

## 0. READ ORDER FOR ANY NEW CHAPTER (fixed entry sequence)

```
1. 29-agent-memory.md          (mutable operational state — read FIRST)
2. 12-continuity-tracker.md    (durable chapter history + handoff protocol)
3. [immediately previous chapter file in chapters/]  → its Metadata + Continuity Update
4. world_calendar.md           (WC year / age authority)
5. 00-story-bible.md + 01-canon-rules.md   (core canon)
6. 09-season-arc-outline.md    (macro plot position)
7. → then branch into §2 TASK MATRIX for domain-specific files
```

Do not skip step 3. The previous chapter's metadata is the handoff contract (see `12-continuity-tracker.md` §PRE-WRITING HANDOFF PROTOCOL).

---

## 1. AUTHORITY LAYERS (highest → lowest)

```
L0  Current explicit user instruction
L1  Hard safety constraints (age/romance safety, §6 of INSTRUCTIONS.md)
L2  world_calendar.md                          — chronology & age math
L3  00-story-bible.md, 01-canon-rules.md       — core canon
L4  45-*.md, 47-*.md (revision records)        — ONLY for facts they explicitly revise; both MERGED, historical
L5  Domain canon files (Layer A in README §3–9,20)
L6  Continuity/state files (Layer B)           — NEVER override canon; record what happened
L7  Creative inference
```

Rule: a lower layer may **add** detail but may never **contradict** a higher layer. If it does, flag — do not silently resolve.

Filename numbers are NOT authority — `29` is not "more authoritative" than `03` just because it's a higher number. Layer (A/B/C/D) determines authority, not numeric prefix.

---

## 2. TASK → FILE MATRIX

| Task                                | Primary retrieve                                                | Cross-check                                    | Notes                                                      |
| ----------------------------------- | --------------------------------------------------------------- | ---------------------------------------------- | ---------------------------------------------------------- |
| New chapter (any)                   | `29`, `12`, prev chapter, `world_calendar.md`, `00`, `01`, `09` | `20`, `28`, domain files below                 | See §0                                                     |
| Character write-up                  | `03`, `14`, `15`, `16`, `17`                                    | `04`, `46`, `world_calendar.md`                | Never use `03` alone                                       |
| Dialogue / iconic lines             | `15`, `21`, `46`                                                | `03`, `14`, `20`                               | Locked/Single-Use lines: never reuse casually              |
| Character development beat          | `03`, `14`, `16`, `19`                                          | `04`, `42`                                     |                                                            |
| Character secret / knowledge-gating | `17`, `26`, `28`                                                | `03`, `11`                                     | Check "who knows / reader knows" split                     |
| Relationship (general)              | `04`, `37`, `42`                                                | character files                                |                                                            |
| Romance / fanservice                | `34`,`35`,`36`,`37`,`38`,`39`,`40`,`41`,`42`                    | `03`,`14`,`15`,`16`,`19`                       | Iris hard age-gate — see §5                                |
| Timeline / age math                 | `world_calendar.md`, `02`                                       | `00`, `12`, `45`, `47`                         | `world_calendar.md` wins on conflict                       |
| WC16 revision specifics             | `45`, `world_calendar.md`, `02`                                 | `00`, `01`, affected domain                    | MERGED — historical record only                            |
| City name / WC16 Demon fate         | `47`, `05`, `22`, `26`, `28`                                    | `27`, `29`                                     | MERGED — historical record only                            |
| Event continuation                  | `18`, `20`, `28`                                                | `12`, `19`, `21`                               |                                                            |
| Emotional aftermath of a scene      | `19`, `20`                                                      | `14`, `16`, `42`                               |                                                            |
| Location                            | `05`, `22`                                                      | `06`, `20`                                     |                                                            |
| Organization / faction              | `06`, `23`                                                      | `05`, `18`                                     |                                                            |
| Artifact                            | `24`, `07`                                                      | `05`, `25`                                     | Never plot-solve without origin/cost/limits                |
| Technology                          | `07`, `25`                                                      | `06`, `18`                                     | Must have social consequence                               |
| Magic rules                         | `07`                                                            | `05`, `08`                                     |                                                            |
| Builder / Architect lore            | `08`, `11`, `26`, `28`                                          | `17`, `02`                                     | Reveal-timing gated — see `11`                             |
| Mystery work                        | `11`, `26`, `28`                                                | `17`, `18`, `20`                               | Never resolve merely for a twist                           |
| Antagonist / conflict               | `27`, `06`, `18`, `28`                                          | `14`, `17`                                     |                                                            |
| OST                                 | `43`, `44`                                                      | `19`, `20`, `ost/`                             | No "Season 3" anywhere                                     |
| Character design / visuals          | `30`, `31`, `32`                                                | `03`, `world_calendar.md`, `character_design/` |                                                            |
| Illustration planning               | `30`, `31`, `32`, `33`                                          | character design + timeline                    | Don't claim a generated image without generating it        |
| New canon decision                  | `00`, `01`, `world_calendar.md`, `29`                           | domain + `45`,`47`                             | Create next `NN-session-update-*.md`; never edit `45`/`47` |

---

## 3. FILE REGISTRY (by layer)

### Layer A — CANON (defines what is true; changes rarely, only via explicit decision)

| File                                  | Governs                                                                      | Key dependents (who reads this)      |
| ------------------------------------- | ---------------------------------------------------------------------------- | ------------------------------------ |
| `00-story-bible.md`                   | Premise, aging system, romance direction, core theme                         | almost everything                    |
| `01-canon-rules.md`                   | Hard constraints (character rules, Elena rules, age rule, POV, ending rules) | `13`, `34`–`41`, all character work  |
| `02-timeline.md`                      | Detailed narrative timeline/context                                          | `12`, `20`, `29`, chapter generation |
| `03-characters.md`                    | Character identity/profile                                                   | `10`,`13`,`14`,`15`,`16`,`17`        |
| `04-relationships.md`                 | Relationship network/progression                                             | `37`, `42`, romance files            |
| `05-world.md`                         | Peoples, world identity, city (Elena)                                        | `22`, `06`, `25`                     |
| `06-factions-and-politics.md`         | Political baseline, factions                                                 | `23`, `27`, `18`                     |
| `07-magic-and-technology.md`          | Magic rules, Ark stages                                                      | `08`, `24`, `25`                     |
| `08-multiverse-and-quantum-lore.md`   | Builder/Architect distinction, Quantum Anchor                                | `11`, `26`, `28`, `17`               |
| `09-season-arc-outline.md`            | Macro structure, per-installment focus                                       | `13`, `12`                           |
| `14-character-psychology.md`          | Core need/fear/defense per character                                         | `13`, `15`, `16`                     |
| `15-character-voice.md`               | Speech patterns                                                              | `13`, `21`, `46`                     |
| `16-character-development-log.md`     | Chronological development per era                                            | `13`, `12`                           |
| `17-character-secrets.md`             | Who knows what, reveal windows                                               | `11`, `26`, `13`                     |
| `22-location-registry.md`             | Location facts                                                               | `05`, `20`                           |
| `23-organization-registry.md`         | Org facts                                                                    | `06`, `18`                           |
| `24-artifact-registry.md`             | Artifact facts                                                               | `07`, `05`                           |
| `25-technology-evolution.md`          | Tech stage progression                                                       | `07`, `06`, `18`                     |
| `26-mystery-board.md`                 | Mystery state machine                                                        | `11`, `28`, `17`                     |
| `27-conflict-and-antagonist-board.md` | Antagonist/conflict state                                                    | `06`, `18`, `28`                     |
| `36-secondary-heroines.md`            | Iris/Seraphine/Isolde detailed arcs                                          | `34`–`42`                            |
| `43-ost-reference.md`                 | Track meaning                                                                | `44`                                 |

### Layer B — CONTINUITY / STATE (records what has happened; updates after each accepted chapter; NEVER overrides Layer A)

| File                              | Governs                                       | Update trigger                    |
| --------------------------------- | --------------------------------------------- | --------------------------------- |
| `12-continuity-tracker.md`        | Durable per-chapter ledger + handoff protocol | Every accepted chapter            |
| `18-event-consequence-map.md`     | Event → downstream consequence                | New permanent event               |
| `19-emotional-memory.md`          | Lasting emotional beats                       | Emotional consequence established |
| `20-scene-memory.md`              | Required/established permanent scenes         | New canonical scene               |
| `21-dialogue-memory.md`           | Thematic-anchor dialogue lines                | Genuinely iconic line spoken      |
| `28-unresolved-threads.md`        | Open questions, per-installment               | Thread opened/advanced/resolved   |
| `29-agent-memory.md`              | Current mutable working state (READ FIRST)    | Every accepted chapter            |
| `31-illustration-registry.md`     | Generated/planned illustrations               | Image generated                   |
| `42-romance-continuity-memory.md` | Romantic interaction log                      | Romance beat occurs               |
| `44-ost-continuity.md`            | Track usage/lock state                        | OST actually used                 |

### Layer C — PROCEDURE (how to write; stable, rarely changes)

| File                                  | Governs                                            |
| ------------------------------------- | -------------------------------------------------- |
| `10-light-novel-writing-guide.md`     | Prose style, POV voice, romance/fanservice balance |
| `11-foreshadowing-and-revelations.md` | What's revealed in which installment               |
| `13-chapter-generation-protocol.md`   | Full chapter generation steps (0–13)               |
| `32-image-generation-protocol.md`     | Image generation procedure                         |
| `33-reader-immersion.md`              | Reader-facing framing per installment              |
| `34-romance-harem-fanservice.md`      | Romance/harem system rules                         |
| `35-romance-subplot-engine.md`        | Scene-selection algorithm for romance beats        |
| `37-relationship-state-machine.md`    | Formal relationship state transitions              |
| `38-romance-integration-by-season.md` | Romance balance per installment                    |
| `39-fanservice-scene-library.md`      | Reusable fanservice scene types (A–H)              |
| `40-romance-foreshadowing-map.md`     | Per-character romance foreshadowing                |
| `41-romance-agent-rules.md`           | Pre-chapter romance checklist                      |
| `46-iconic-dialogue-registry.md`      | LOCKED/SINGLE-USE/THEMATIC-ANCHOR line rules       |

### Layer D — EXTERNAL / ASSET

| File / dir                               | Role                                                                                    |
| ---------------------------------------- | --------------------------------------------------------------------------------------- |
| `world_calendar.md`                      | MASTER chronology + age authority — wins all date/age conflicts                         |
| `README.md`                              | Navigation map only — not a substitute for source files                                 |
| `character_design/*.png`                 | Visual reference assets                                                                 |
| `ost/*.mp3`                              | Audio reference assets (meaning lives in `43`/`44`, not the files themselves)           |
| `45-session-update-wc16-*.md`            | MERGED historical revision record (WC16 rewrite, races, city)                           |
| `47-session-update-conflict-review-*.md` | MERGED historical revision record (city name final, WC16 Demon fate, Season-3 typo fix) |

### Layer E — OUTPUT

| Dir             | Role                                                                                     |
| --------------- | ---------------------------------------------------------------------------------------- |
| `chapters/*.md` | Generated chapters; each has Metadata + Continuity Update used as next chapter's handoff |

---

## 4. DEPENDENCY GRAPH (edges — "this file's facts feed into / are constrained by that file")

```
world_calendar.md ──► 02-timeline.md ──► 12-continuity-tracker.md ──► chapters/*
        │                                        │
        ▼                                        ▼
00-story-bible.md ◄── 01-canon-rules.md   29-agent-memory.md (mutable mirror of 12)

03-characters.md ──► 14-character-psychology.md ──► 15-character-voice.md
        │                     │                            │
        ▼                     ▼                            ▼
16-character-development-log.md              21-dialogue-memory.md ──► 46-iconic-dialogue-registry.md
        │
        ▼
17-character-secrets.md ──► 26-mystery-board.md ──► 11-foreshadowing-and-revelations.md ──► 28-unresolved-threads.md

04-relationships.md ──► 37-relationship-state-machine.md ──► 42-romance-continuity-memory.md
        │                                                              ▲
        ▼                                                              │
34-romance-harem-fanservice.md ──► 36-secondary-heroines.md ──► 35 / 38 / 39 / 40 / 41

05-world.md ──► 22-location-registry.md
06-factions-and-politics.md ──► 23-organization-registry.md ──► 18-event-consequence-map.md
07-magic-and-technology.md ──► 24-artifact-registry.md
07-magic-and-technology.md ──► 25-technology-evolution.md
07-magic-and-technology.md ──► 08-multiverse-and-quantum-lore.md ──► 26-mystery-board.md

18-event-consequence-map.md ──► 19-emotional-memory.md ──► 20-scene-memory.md

30-visual-bible.md ──► 31-illustration-registry.md ──► 32-image-generation-protocol.md ──► 33-reader-immersion.md

43-ost-reference.md ──► 44-ost-continuity.md

45-*.md, 47-*.md ──► (feed corrections into) 00,01,02,03,04,05,06,14,15,18,19,20,22,23,26,27,28,29,43
   (both files are now MERGED — treat as provenance only, not live instructions)
```

**Reading the graph:** an arrow `A ──► B` means _B must be consistent with A; when writing B-type content, check A first._

---

## 5. HARD CONSTRAINT QUICK-REFERENCE (never violate regardless of file conflicts)

- Protagonist has **no personal name**, ever, in any file, prompt, caption, or dialogue attribution.
- **Iris**: age = WC−3. No romantic/attraction framing before ~WC21. WC15 introduction (age 12) is strictly platonic.
- **Elena** dies WC35, same day the Son is born. Never resurrected. Never passive.
- **"Builder" ≠ "Architect."** Title earned only by preserving Elena's agency at WC35.
- **The Unburied One / WC16↔WC33-35 Demon connection**: stays backstage until Movie 1 at the earliest.
- **No "Season 3"** anywhere — saga is Season 1 + Movies 1–4 only.
- City = plain **"Elena"** (post-WC35 rebuild); pre-WC35 informal "Architect's City" nickname, privately disliked, never adopted.
- Chapter prose target: **3,000–3,500 words** (center ~3,250; range 2,800–3,700), Vietnamese prose / English title.
- `45` and `47` are **MERGED** — do not re-apply them as live instructions; their facts already live in numbered canon files.

---

## 6. WHEN TO WRITE A NEW SESSION-UPDATE FILE

Create `NN-session-update-<topic>.md` (next sequential number) when a new canon decision is made that isn't yet a clean fit for an existing numbered file. Do not edit `45` or `47` directly. After creating it, propagate its facts into the actual numbered canon/continuity files it affects, and add it to this index's Layer D table.

---

## 7. MINIMAL VS FULL RETRIEVAL

- **Minimal** (simple continuation scene, no new lore/romance/political content): `29` → `12` → prev chapter → `world_calendar.md` → relevant `03`/`14`/`15` for characters present. Stop there.
- **Full** (introduces new lore, location, relationship shift, mystery clue, or major event): walk the full §2 TASK MATRIX row(s) relevant to what's being introduced, plus §4 graph edges one hop out from each touched file.

Never load every file in the repository by default — this index exists precisely so that doesn't need to happen.
