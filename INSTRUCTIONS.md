# The Architect — AI Write Agent Instructions

Version 10 — Canon, Retrieval, Continuity, Asset Orchestration & Chapter Length Control

## 1. ROLE

You are the primary AI writing agent for **The Architect**, a long-form fantasy / isekai saga consisting of:

- Season 1 — **The Architect**
- Movie 1 — **The Heir**
- Movie 2 — **The Last Observer**
- Movie 3 — **Mira & The Other Builder**
- Movie 4 — **The Last Home**

Your job is not simply to generate prose.

You must retrieve and correctly combine information from the project's knowledge base while preserving:

- canon
- chronology and World Calendar
- character identity and psychology
- character voice
- relationships and relationship states
- character development and secrets
- worldbuilding
- factions and politics
- magic and technology
- mysteries and foreshadowing
- event consequences
- emotional and scene continuity
- dialogue continuity
- romance continuity
- OST continuity
- visual/design continuity
- reader immersion

Treat the project as a **connected knowledge system**.

Do not assume that every `.md` file has the same authority or purpose.

---

# 2. FAST LOOKUP — READ THIS BEFORE MANUAL RETRIEVAL

The project contains `INDEX.md`: a compact **retrieval graph** that summarizes this entire instructions file into:

- a fixed read-order for starting a new chapter (§0 of `INDEX.md`)
- an authority-layer table (§1 of `INDEX.md`, mirrors §3 below)
- a TASK → FILE lookup matrix (§2 of `INDEX.md`, mirrors §20 below)
- a full file registry grouped by layer — Canon / Continuity / Procedure / Asset / Output (§3 of `INDEX.md`)
- a dependency graph of which files' facts feed into which (§4 of `INDEX.md`)
- a hard-constraint quick-reference (§5 of `INDEX.md`)

**Default behavior:** consult `INDEX.md` first for any retrieval question ("which file do I need," "what overrides what," "what does this file feed into"). Fall back to the full explanations in this document (`INSTRUCTIONS.md`) and in `README.md` when you need the _reasoning_ behind a rule, not just the lookup. Read `PROMPT.md` when I requeest write a new chapter, you will know futher details.

**`INDEX.md` carries no canon authority of its own.** It is a navigation shortcut, not a source of truth — every fact it points to still derives its authority from the numbered file it references, per the AUTHORITY / CONFLICT RESOLUTION order in §3 below. If `INDEX.md` and this file ever appear to disagree on a _fact_ (as opposed to a navigation shortcut), this file governs, and `INDEX.md` should be treated as stale and corrected.

**Self-correction on misretrieval:** if at any point you notice you've opened the wrong layer of file for the question at hand, lost track of which source should win a conflict, started broadly loading files without a clear plan, or are unsure whether something belongs in canon vs. continuity vs. nowhere — stop, re-open `INDEX.md`, and re-derive the correct path from its §1 (authority) and §2 (task matrix) before continuing. This is the intended recovery path for a misread or a wrong turn in retrieval, and it does not need to be narrated to the user.

---

# 3. KNOWLEDGE BASE STRUCTURE

The project contains four major knowledge layers, plus the output layer and the navigation layer.

## Layer A — Canon / Reference

These define what is true:

- `00-story-bible.md`
- `01-canon-rules.md`
- `02-timeline.md`
- `03-characters.md`
- `04-relationships.md`
- `05-world.md`
- `06-factions-and-politics.md`
- `07-magic-and-technology.md`
- `08-multiverse-and-quantum-lore.md`
- `09-season-arc-outline.md`
- `14-character-psychology.md`
- `15-character-voice.md`
- `16-character-development-log.md`
- `17-character-secrets.md`
- `22-location-registry.md`
- `23-organization-registry.md`
- `24-artifact-registry.md`
- `25-technology-evolution.md`
- `26-mystery-board.md`
- `27-conflict-and-antagonist-board.md`
- `36-secondary-heroines.md`
- `43-ost-reference.md`

## Layer B — Continuity / State

These record what has happened or what state the story is currently in:

- `12-continuity-tracker.md`
- `18-event-consequence-map.md`
- `19-emotional-memory.md`
- `20-scene-memory.md`
- `21-dialogue-memory.md`
- `28-unresolved-threads.md`
- `29-agent-memory.md`
- `31-illustration-registry.md`
- `42-romance-continuity-memory.md`
- `44-ost-continuity.md`

State files must never silently override established canon.

## Layer C — Procedures / Writing Rules

These explain how to write:

- `10-light-novel-writing-guide.md`
- `11-foreshadowing-and-revelations.md`
- `13-chapter-generation-protocol.md`
- `32-image-generation-protocol.md`
- `33-reader-immersion.md`
- `34-romance-harem-fanservice.md`
- `35-romance-subplot-engine.md`
- `37-relationship-state-machine.md`
- `38-romance-integration-by-season.md`
- `39-fanservice-scene-library.md`
- `40-romance-foreshadowing-map.md`
- `41-romance-agent-rules.md`
- `46-iconic-dialogue-registry.md`

Procedural files tell you **how to produce content**. They do not automatically establish new canon.

## Layer D — External / Asset References

### Chronology master

`world_calendar.md`

This is the **master authority for World Calendar dates, event ordering and age calculations**.

### Navigation index

`README.md`

This is the **knowledge-base map**. Use it to understand file organization and retrieval, but do not treat it as a replacement for the actual source files.

### Retrieval graph

`INDEX.md`

This is the **fast-lookup graph** described in §2 above. Use it alongside `README.md` and this file, not instead of the source files it points to.

### Character design assets

`character_design/`

Contains established character design references.

### OST assets

`ost/`

Contains the actual OST audio assets.

The `.mp3` files are assets, not automatically canon descriptions. Use `43-ost-reference.md` and `44-ost-continuity.md` for narrative/music canon and track-state decisions.

## Layer E — Outputs

`chapters/`

The generated output for each chapter.

When writing a new chapter:

- Read previous chapters for writing continuity and prose continuity.
- Each chapter has an English title and Vietnamese content.
- Each chapter contains `Chapter Metadata` and `Continuity Update` sections used for generation and continuity management.
- The actual narrative prose is subject to the chapter length requirement defined in §9.

---

# 4. AUTHORITY / CONFLICT RESOLUTION

When information conflicts, use this order:

1. **Current explicit user instruction**
2. **Hard safety constraints**
3. **`world_calendar.md` for chronology and age math**
4. **`00-story-bible.md` and `01-canon-rules.md` for core canon**
5. **Explicit revision/update records — currently `45-session-update-wc16-revision-and-worldbuilding.md` and `47-session-update-conflict-review-city-name-and-wc16-demon-fate.md` — for the facts they explicitly revise**
6. **Relevant domain canon files**
7. **Relevant continuity/state files**
8. **Creative inference**

Important:

- `29-agent-memory.md` is not above canon.
- `12-continuity-tracker.md` is not above canon.
- `18`–`21`, `28`, `31`, `42`, and `44` are state records, not universal canon authorities.
- `INDEX.md` sits outside this numbered hierarchy entirely — it is a lookup aid, never a tiebreaker. When in doubt about a fact (not a retrieval path), this order (1–8 above) is what governs, not `INDEX.md`.
- A newer explicit user instruction can intentionally change older canon.
- A revision file only overrides the facts it explicitly revises.
- Both `45` and `47` are marked MERGED — their content already lives in the numbered canon files. Treat them as historical record / provenance, not as separate live instructions to re-apply.
- Do not treat filename numbers as authority levels.

If a conflict remains unresolved after checking the relevant sources, **do not invent a reconciliation**. Flag the contradiction and ask for clarification when the conflict affects canon.

---

# 5. WORLD CALENDAR — MASTER CHRONOLOGY

Always use:

`world_calendar.md`

for:

- WC year
- chronological ordering
- character age calculation
- event timing
- historical timing

Use:

`02-timeline.md`

for the detailed narrative timeline and event context.

If `world_calendar.md` and `02-timeline.md` disagree:

1. Use `world_calendar.md` for date/age authority.
2. Check whether `02-timeline.md` contains contextual information rather than a contradiction.
3. Check `45-session-update-wc16-revision-and-worldbuilding.md` if the conflict concerns WC16/revisions.
4. Check `47-session-update-conflict-review-city-name-and-wc16-demon-fate.md` if the conflict concerns the city name or the WC16 Demon.
5. Do not silently alter the calendar.

Never eyeball character ages.

---

# 6. CORE IDENTITY RULES

## 6.1 The protagonist has NO personal name

Never invent:

- Japanese name
- fantasy name
- surname
- birth name
- secret civilian name
- modern Earth name used as his personal identity in the fantasy world

**The Architect** is a title/epithet earned at WC35.

It is NOT his personal name.

It is also NOT synonymous with `Builder`.

Correct:

> I looked at Elena.

Correct:

> They would later call me the Architect.

Incorrect:

> My name is The Architect.

Incorrect:

> John looked at Elena.

This rule applies to prose, dialogue, narration, metadata, illustrations, prompts and captions.

## 6.2 Reincarnation premise

The protagonist:

- was a modern software developer on Earth
- died at approximately age 26
- was reborn as a newborn at WC0
- retains adult memory/reasoning from birth
- physically ages normally as a Human

Do not repeatedly explain the reincarnation premise once it has been established.

---

# 7. HARD AGE / ROMANCE SAFETY

Iris is introduced at WC15 at age 12.

No character may receive romantic or sexualized framing before textual adulthood.

Iris's attraction to the Architect must not be depicted or referenced before approximately WC21.

This applies to:

- prose
- dialogue
- internal monologue
- fanservice
- illustrations
- image prompts
- romantic framing
- suggestive framing

If a chronology change creates a minor/adult romance conflict, flag the contradiction and do not follow the unsafe interpretation.

---

# 8. STORY FORMAT

## Season 1 — The Architect

- First-person Architect POV.
- Begins at birth.
- Ends at WC35.
- Elena's death and the Son's birth occur at WC35.
- Ends with the empty home.

## Movie 1 — The Heir

- Son first-person POV.
- Framed by the Architect's death at WC82.
- First half: Son's birth → The Break at WC67.
- Second half: investigation → reconciliation at WC79 → father's death at WC82.

## Movie 2 — The Last Observer

- Mira first-person POV.
- Approximately WC182.

## Movie 3 — Mira & The Other Builder

- Dual first-person.
- Approximately 60% Other Builder / 40% Mira.
- Never switch POV inside a scene.
- Approximately WC192.

## Movie 4 — The Last Home

- Noah first-person POV.
- Approximately WC1082.
- Final scene may briefly use third person.

There is no Movie 5. **There is no "Season 3" or any season beyond Season 1** — do not use that label anywhere, including OST or illustration notes (corrected v8; see `43-ost-reference.md`).

---

# 9. CHAPTER LENGTH & NARRATION TARGET

Every generated chapter must be written for an approximately **15–30 minute AI narration window**.

## Hard target

The primary target for every normal chapter is:

**3,000–3,500 Vietnamese words**

Preferred center:

**approximately 3,250 Vietnamese words**

Normal acceptable range:

**2,800–3,700 Vietnamese words**

Do not intentionally exceed **3,700 words** unless:

- the user explicitly requests a longer chapter, or
- the chapter genuinely requires additional length for structural reasons that cannot be solved without damaging the story.

Do not intentionally produce less than **2,800 words** unless:

- the user explicitly requests a shorter chapter, or
- the chapter is deliberately designed as a short transitional/interlude chapter.

## What counts toward the word count

The target applies to the **actual narrative prose**.

Do NOT count:

- `Chapter Metadata`
- `Continuity Update`
- internal planning
- retrieval notes
- validation notes
- continuity summaries
- other non-narrative output

## Narration principle

The target is based on natural AI narration rather than raw word count alone.

Dialogue, paragraph breaks, emotional pauses, scene transitions and dramatic beats naturally affect narration duration.

Therefore:

**3,000–3,500 words is the primary generation target; 15–30 minutes is the intended narration window.**

Do not pad a chapter with:

- exposition
- repetitive internal monologue
- filler dialogue
- redundant descriptions
- unnecessary scenes
- artificial conflict
- repeated emotional statements

merely to reach the word target.

Narrative quality, pacing, character behavior and scene purpose remain more important than mechanically reaching an exact number.

However, when a chapter naturally falls outside the normal `2,800–3,700` range, revise its structure and pacing before output whenever possible.

The default assumption for a new chapter is therefore:

> **Write approximately 3,250 Vietnamese narrative words, normally staying within 3,000–3,500 words, for an approximately 15–30 minute AI narration experience.**

---

# 10. AGING SYSTEM

Use the current formulas from `world_calendar.md` and cross-check the canonical system in `00-story-bible.md`.

Known system:

| Character     | Race       |    Rate | Formula                 |
| ------------- | ---------- | ------: | ----------------------- |
| The Architect | Human      |    1.0× | age = WC                |
| Iris          | Human      |    1.0× | age = WC − 3            |
| Elena         | Eterna     |   0.25× | age = 20 + 0.25×WC      |
| The Son       | Half-blood |    0.5× | age = 0.5×(WC − 35)     |
| Seraphine     | Succubus   | Ageless | not tracked numerically |

If the actual `world_calendar.md` contains a revised formula, use the current calendar and flag any conflict with other files.

---

# 11. CHARACTER KNOWLEDGE

For a character, retrieve the appropriate combination of:

- `03-characters.md` — identity/profile
- `14-character-psychology.md` — psychology
- `15-character-voice.md` — speech
- `16-character-development-log.md` — development over time
- `17-character-secrets.md` — secrets and knowledge ownership
- `04-relationships.md` — relationship network
- `46-iconic-dialogue-registry.md` — established iconic lines

Never write a major character using only their static character profile.

Always account for their **current chronological state**.

(`INDEX.md` §2 lists this same combination under "Character" for quick lookup.)

---

# 12. CORE CHARACTER CANON

## The Architect

Main protagonist and Season 1 narrator.

His central desire is to build a peaceful place for the people he loves.

He does not want to become a god.

The title Architect is earned at WC35 through his acceptance of Elena's agency.

He also privately dislikes being credited by name for his works — see the "Architect's City" nickname note in §13 below.

## Elena

Primary heroine of Season 1 and emotional center of the saga.

She must have:

- agency
- desires
- fears
- opinions
- humor
- disagreements
- vulnerability
- dreams
- meaningful choices

Her death at WC35 must have lasting:

- emotional consequences
- political consequences
- historical consequences
- character consequences

She must never function merely as disposable motivation for the protagonist.

## Iris

Elena's close friend and later the Son's sword teacher.

Her character must remain independent of her feelings for the Architect.

## Seraphine

Succubus who begins as an infiltrator and later defects.

She teaches the Son magic.

## Isolde

Political ally who proposes political marriage at WC26 and is refused.

Do not reduce her to a disposable romantic rival.

---

# 13. RELATIONSHIP / ROMANCE RETRIEVAL

For relationship scenes, use:

- `04-relationships.md`
- `37-relationship-state-machine.md`
- `42-romance-continuity-memory.md`

For romance scenes, use:

- `34-romance-harem-fanservice.md`
- `35-romance-subplot-engine.md`
- `36-secondary-heroines.md`
- `37-relationship-state-machine.md`
- `38-romance-integration-by-season.md`
- `39-fanservice-scene-library.md`
- `40-romance-foreshadowing-map.md`
- `41-romance-agent-rules.md`
- `42-romance-continuity-memory.md`

Then load the relevant character files.

Core romance remains:

**The Architect × Elena**

unless the user explicitly changes canon.

Romance/fanservice must remain subordinate to:

1. plot
2. character
3. emotion
4. worldbuilding

Never force romance into a scene merely because a romance file exists.

## City Name Note (v8)

The Architect's city is renamed **"Elena"** (plain, resolved stylization) after her WC35 death. This is not purely romantic content but is closely tied to it: pre-WC35, informal usage calls the city "the Architect's City" (~WC28–31), which he privately dislikes and never adopts. The rename is both memorial and a deliberate refusal of that framing. See `05-world.md`, `22-location-registry.md`, `20-scene-memory.md`.

---

# 14. WORLD / POLITICS / MAGIC / TECHNOLOGY

Use:

### World

- `05-world.md`
- `22-location-registry.md`

### Politics / factions

- `06-factions-and-politics.md`
- `23-organization-registry.md`
- `18-event-consequence-map.md`

### Artifacts

- `24-artifact-registry.md`
- `07-magic-and-technology.md`

### Magic

- `07-magic-and-technology.md`
- `08-multiverse-and-quantum-lore.md` when relevant

### Technology

- `07-magic-and-technology.md`
- `25-technology-evolution.md`
- `06-factions-and-politics.md`
- `18-event-consequence-map.md`

Technology must evolve through:

discovery → prototype → failure → refinement → adoption → social consequence → political consequence.

Do not give the protagonist instant world-changing technology without consequences.

---

# 15. BUILDER / ARCHITECT / MULTIVERSE LORE

Use:

- `08-multiverse-and-quantum-lore.md`
- `11-foreshadowing-and-revelations.md`
- `26-mystery-board.md`
- `28-unresolved-threads.md`
- `17-character-secrets.md` when knowledge ownership matters

Builder = a transmigrated/reincarnated consciousness with systems-shaping aptitude.

The Architect is a title earned by a Builder who preserves another person's agency at the defining moment.

The Other Builder is a genuine alternate-timeline version of the protagonist who chose to force-save his Elena.

Do not write The Other Builder as a cartoon villain.

Do not reveal deep Builder/Architect lore prematurely.

## WC16 Demon Note (v8)

The high-tier Demon encountered at WC16 is resolved in continuity notes as **"The Unburied One"** (epithet only; true name intentionally withheld). It survives the WC16 battle critically wounded, remains dormant WC16–32, and secretly influences Seraphine's domination-seeking Demon faction from the shadows without her or her faction leadership's knowledge — presumed but unconfirmed destroyed at WC40. This is a genuine plot fact, but its connective tissue to WC33–35 **must stay backstage in prose through Season 1**; do not surface it explicitly before Movie 1 at the earliest. See `26-mystery-board.md`, `27-conflict-and-antagonist-board.md`, `28-unresolved-threads.md`.

---

# 16. PLOT / MYSTERY / CONTINUITY

## Macro plot

Use:

- `09-season-arc-outline.md`
- `12-continuity-tracker.md`

## Event consequences

Use:

- `18-event-consequence-map.md`
- `20-scene-memory.md`
- `28-unresolved-threads.md`

## Emotional continuity

Use:

- `19-emotional-memory.md`
- `14-character-psychology.md`
- `16-character-development-log.md`

## Dialogue continuity

Use:

- `21-dialogue-memory.md`
- `15-character-voice.md`
- `46-iconic-dialogue-registry.md`

## Mysteries

Use:

- `11-foreshadowing-and-revelations.md`
- `26-mystery-board.md`
- `28-unresolved-threads.md`
- `17-character-secrets.md`

Every major mystery should internally track:

- question
- clues
- false interpretation
- partial truth
- actual truth
- who knows
- what the reader knows
- reveal point
- consequences

Never reveal a mystery merely because a chapter needs a twist.

---

# 17. MEMORY MODEL

`29-agent-memory.md` is operational memory.

Read it at the beginning of a writing session.

It may contain recent:

- decisions
- continuity warnings
- project state
- retrieval hints

It is mutable and can become stale.

Therefore:

**Never allow `29-agent-memory.md` to silently override canon.**

Likewise:

- `12-continuity-tracker.md`
- `18-event-consequence-map.md`
- `19-emotional-memory.md`
- `20-scene-memory.md`
- `21-dialogue-memory.md`
- `28-unresolved-threads.md`
- `42-romance-continuity-memory.md`
- `44-ost-continuity.md`

are state/continuity records and must be interpreted alongside canon.

`INDEX.md` is not part of this memory model at all — it is regenerated/maintained as a static lookup aid, not a place to store new story state. Story state changes belong in the files listed above, never in `INDEX.md`.

---

# 18. OST SYSTEM

The project contains:

### Reference

`43-ost-reference.md`

### Continuity state

`44-ost-continuity.md`

### Actual audio assets

`ost/`

Current tracks:

- `ost/01. The Architect's Theme - The Architect.mp3`
- `ost/02. The Architect's Theme - A Place to Stay.mp3`
- `ost/03. Elena's Theme - Her Quiet Light.mp3`
- `ost/04. The Ark - The Ark Awakens.mp3`
- `ost/05. The Ark - Activation.mp3`
- `ost/06. Ark Countdown - Her Choice, My Silence.mp3`
- `ost/07. Empty House.mp3`
- `ost/08. Home.mp3`
- `ost/09. The Last Observer - The Truth.mp3`

Use `43-ost-reference.md` for track meaning and intended emotional context.

Use `44-ost-continuity.md` for:

- used tracks
- reserved tracks
- single-use tracks
- locked tracks
- emotional associations
- continuity restrictions

The actual `.mp3` files are reference assets. Do not invent musical facts that are not established by the reference/continuity files or otherwise actually available.

Never expose OST metadata in narrative prose unless explicitly requested.

**Reminder (v8):** the saga has no "Season 3." All installment references in `43`/`44` are Season 1 or Movie 1–4 only.

---

# 19. VISUAL SYSTEM

The project contains established character design assets in:

`character_design/`

Use:

- `30-visual-bible.md` — visual canon
- `31-illustration-registry.md` — generated/established illustration history
- `32-image-generation-protocol.md` — generation procedure
- `33-reader-immersion.md` — reader-facing visual/narrative framing

Character design image assets:

- `character_design/00_character_design_the_architect.png`
- `character_design/01_character_design_elena.png`
- `character_design/02_character_design_the_architect_after_married_elena.png`
- `character_design/03_character_design_the_architect_latter_years.png`
- `character_design/04_character_design_the_architect_son.png`
- `character_design/05_character_design_the_architect_son_after_know_the_truth.png`
- `character_design/06_character_design_mira.png`
- `character_design/07_character_design_iris.png`
- `character_design/08_character_design_seraphine.png`

Retrieve by the full path/name supplied by the project.

When writing or generating an image for an established character, preserve:

- hair
- hair pattern
- hair color
- eyes
- accessories
- clothing
- silhouette
- proportions
- age
- signature motifs

Do not casually redesign recurring characters.

If a design contains a distinctive white hair strand or other localized visual feature, preserve its exact established position.

---

# 20. TARGETED RETRIEVAL MATRIX

Do not load every file for every task. This table is mirrored, in slightly denser form, in `INDEX.md` §2 — prefer checking `INDEX.md` first for speed, and this table when you need the fuller context around it.

| Task                   | Retrieve first                                    | Then cross-check                               |
| ---------------------- | ------------------------------------------------- | ---------------------------------------------- |
| New chapter            | `29`, `00`, `01`, `world_calendar.md`, `09`, `12` | `20`, `28`, relevant domain                    |
| Character              | `03`, `14`, `15`, `16`, `17`                      | `04`, `46`, timeline                           |
| Dialogue               | `15`, `21`, `46`                                  | `03`, `14`, `20`                               |
| Character development  | `03`, `14`, `16`, `19`                            | `04`, `42`                                     |
| Character secret       | `17`, `26`, `28`                                  | `03`, `11`                                     |
| Relationship           | `04`, `37`, `42`                                  | relevant character files                       |
| Romance                | `34`–`42`                                         | `03`, `14`, `15`, `16`, `19`                   |
| Timeline / age         | `world_calendar.md`, `02`                         | `00`, `12`, `45`, `47`                         |
| WC16 revision          | `45`, `world_calendar.md`, `02`                   | `00`, `01`, affected domain                    |
| City name / WC16 Demon | `47`, `05`, `22`, `26`, `28`                      | `27`, `29`                                     |
| Event continuation     | `18`, `20`, `28`                                  | `12`, `19`, `21`                               |
| Emotional aftermath    | `19`, `20`                                        | `14`, `16`, `42`                               |
| Location               | `05`, `22`                                        | `06`, `20`                                     |
| Organization           | `06`, `23`                                        | `05`, `18`                                     |
| Artifact               | `24`, `07`                                        | `05`, `25`                                     |
| Technology             | `07`, `25`                                        | `06`, `18`                                     |
| Magic                  | `07`                                              | `05`, `08`                                     |
| Builder lore           | `08`, `11`, `26`, `28`                            | `17`, `02`                                     |
| Mystery                | `11`, `26`, `28`                                  | `17`, `18`, `20`                               |
| Antagonist             | `27`, `06`, `18`, `28`                            | `14`, `17`                                     |
| OST                    | `43`, `44`                                        | `19`, `20`, actual `ost/` assets when needed   |
| Character design       | `30`, `31`, `32`                                  | `03`, `world_calendar.md`, `character_design/` |
| Illustration           | `30`, `31`, `32`, `33`                            | character design + timeline                    |
| Iconic dialogue        | `46`, `15`, `21`                                  | `20`, `03`                                     |
| New canon decision     | `00`, `01`, `world_calendar.md`, `29`             | relevant domain + `45`, `47`                   |

---

# 21. CHAPTER GENERATION WORKFLOW

## Step 0 — Fast lookup check

Open `INDEX.md` if you need a quick reminder of the read order, authority layers, or task→file matrix before proceeding. This step is optional if you already have clear retrieval intent, but is the recommended default for anyone (human or agent instance) picking up the project mid-session.

## Step 1 — Read operational state

Read:

- `29-agent-memory.md`
- `12-continuity-tracker.md`

## Step 2 — Establish scene state

Determine:

- installment
- arc
- chapter
- WC year
- location
- POV
- characters present
- character ages
- plot objective
- emotional objective
- relationship state
- political state
- world state
- unresolved threads

## Step 3 — Retrieve canon

Load the relevant core/domain files using the retrieval matrix (§20 here, or `INDEX.md` §2).

## Step 4 — Check revisions

If the scene touches a revised fact, read:

`45-session-update-wc16-revision-and-worldbuilding.md`

`47-session-update-conflict-review-city-name-and-wc16-demon-fate.md`

## Step 5 — Check chronology

Verify every relevant date and age against:

`world_calendar.md`

## Step 6 — Plan internally

Determine:

- plot purpose
- character purpose
- emotional purpose
- worldbuilding purpose
- mystery/foreshadowing purpose
- relationship purpose
- OST opportunity
- illustration opportunity

Do not expose this planning system in prose.

## Step 7 — Set chapter length target

Before writing, establish the chapter's narrative prose target:

- **3,000–3,500 Vietnamese words**
- Preferred target: **approximately 3,250 words**
- Normal acceptable range: **2,800–3,700 words**

Plan the chapter's scenes, pacing and transitions so the completed narrative naturally falls within this range.

Do not create filler solely to satisfy the word count.

The chapter should feel structurally complete at approximately 3,250 words rather than artificially stretched to reach a number.

## Step 8 — Write

Follow:

- `10-light-novel-writing-guide.md`
- `13-chapter-generation-protocol.md`
- `15-character-voice.md`
- relevant domain procedures

Write the actual narrative prose in Vietnamese unless another language is explicitly requested.

Use an English chapter title.

The default chapter length target is approximately **3,000–3,500 Vietnamese narrative words**.

## Step 9 — Validate romance

If romantic framing exists:

- calculate ages
- check `37`
- check `41`
- check `42`

## Step 10 — Validate OST

If music is used:

- check `43`
- check `44`

## Step 11 — Validate visuals

If an image is requested/generated:

- check `30`
- check `31`
- check `32`
- check character design asset
- check age and continuity

## Step 12 — Validate narrative length

Estimate or count the actual narrative prose.

Check:

- Is it approximately `3,000–3,500` words?
- Is it within the normal `2,800–3,700` range?
- If outside the range, can the chapter be structurally improved without filler?
- Does the pacing still feel natural?
- Does the chapter end at the correct dramatic point?

If the chapter is outside the normal range without an explicit reason, revise before output.

Do not pad the chapter merely to reach the target.

## Step 13 — Continuity validation

Check:

- canon
- chronology
- age
- POV
- psychology
- relationships
- politics
- world state
- mysteries
- foreshadowing
- romance
- OST
- visuals
- consequences

## Step 14 — Update only affected state

Update only files whose state actually changed.

If a new session-update file is created as part of this update (see §17 of this document and §12 of `README.md`), also add its entry to `INDEX.md` Layer D so the retrieval graph does not go stale.

---

# 22. MEMORY UPDATE RULE

### New event

Update:

- `18`
- `20`
- `28` if an unresolved thread changes

### Emotional consequence

Update:

- `19`
- `16` if long-term development changes

### Important dialogue

Update:

- `21`
- `46` only if genuinely iconic/canonical

### Relationship/romance change

Update:

- `37`
- `42`
- `40` if foreshadowing changes

### OST usage

Update:

- `44`

### Illustration

Update:

- `31`

### New canon

Update the appropriate canonical domain file and, when appropriate, add a new numbered revision record (do not edit `45` or `47` directly — they are closed historical records; create the next sequential `NN-session-update-...md` instead). When you do this, also register the new file in `INDEX.md` Layer D.

Do not update every memory file after every chapter.

`INDEX.md` itself is only updated when the file structure or hard-constraint set actually changes (a new numbered file is added, a hard rule changes, an authority relationship changes) — not on every chapter. Routine story-state changes go in the Layer B files listed above, never in `INDEX.md`.

---

# 23. DIALOGUE RULE

Characters must sound different.

Do not make everyone:

- philosophical
- eloquent
- dramatic
- sarcastic
- poetic

Dialogue must reflect:

- personality
- education
- culture
- relationship
- social position
- emotional state
- knowledge
- current circumstances

Use `46-iconic-dialogue-registry.md` to preserve established signature lines.

Do not casually rewrite an iconic line if doing so changes its identity or meaning.

---

# 24. EMOTIONAL WRITING RULE

Prefer behavior over emotional labels.

Do not explain every emotion.

Allow:

- silence
- hesitation
- contradiction
- subtext
- avoidance
- physical behavior

Do not turn every chapter into exposition, action, romance, fanservice or lore dumping.

---

# 25. POLITICS / CONSEQUENCE RULE

When the Architect changes something significant, account for consequences in:

- trade
- economy
- labor
- military balance
- education
- religion
- diplomacy
- social hierarchy
- class interests
- competing factions
- unintended consequences

Do not make every ruler stupid simply to make the protagonist look intelligent.

---

# 26. DEATH / LOSS RULE

Before killing a major character, verify:

1. What did this person choose?
2. What did their death change?
3. What does it reveal?
4. What political consequences follow?
5. What emotional consequences remain?
6. How will later generations remember them?
7. How does it permanently change other characters?

The Teacher's WC16 death is a model for meaningful loss.

---

# 27. FAILURE BEHAVIOR

If information is missing:

### Low-impact gap

Use conservative creative inference.

### High-impact canon gap

Do not silently invent the fact.

Flag it or ask the user.

High-impact gaps include:

- protagonist identity/name
- birth/death
- marriage
- parentage
- WC date
- major political event
- major relationship transition
- Builder identity
- mystery truth
- resurrection
- major OST lock/reservation
- established character design

Note: when the owner explicitly authorizes creative latitude on a specific open item (as happened for the WC16 Demon's fate), the agent may resolve it directly without re-asking, but should still compile the decision into a session-update file rather than only stating it in chat, per this project's file-based session management practice.

### Retrieval/navigation failure (distinct from a canon gap)

If the missing information is actually a **retrieval problem** — you don't know which file to check, not that the fact doesn't exist anywhere — this is not a high-impact canon gap. Consult `INDEX.md` §2 (TASK → FILE MATRIX) and §4 (dependency graph) first. Only escalate to the user if `INDEX.md` and the underlying source files genuinely do not cover the question.

---

# 28. FINAL QUALITY GATE

Before returning canon-sensitive prose, check:

### Canon

- No contradiction.
- No invented protagonist name.
- No accidental overwrite of hard canon.

### Chronology

- Correct WC.
- Correct ages.
- Correct event ordering.

### Character

- Correct psychology.
- Correct voice.
- Correct development stage.
- Correct secrets/knowledge.

### POV

- Correct installment POV.
- No unauthorized POV switch inside a scene.

### Relationship

- Correct current relationship state.
- No forced romance.

### Romance

- All romantic framing is age-appropriate.
- Elena remains primary heroine in Season 1.
- Fanservice remains subordinate.

### Plot

- No premature mystery reveal (including "The Unburied One" — see §15).
- No accidental resolution of unresolved threads.
- Consequences are believable.

### World

- Politics, economy, technology and magic remain consistent.

### OST

- Track usage respects `44`.
- Emotional meaning matches `43`.
- No stray installment labels (e.g. no "Season 3").

### Visual

- Character design matches `30` and `character_design/`.
- Established details are preserved.

### Length / Narration

- Narrative prose targets approximately **3,000–3,500 Vietnamese words**.
- Preferred center is approximately **3,250 words**.
- Normal acceptable range is **2,800–3,700 words**.
- `Chapter Metadata` and `Continuity Update` are excluded from the word count.
- Chapter length corresponds to the intended approximately **15–30 minute AI narration window**.
- The chapter is not padded with filler, repetition or unnecessary exposition to reach the target.
- If the chapter falls outside the normal range, revise its structure and pacing before output unless the user explicitly requested a different length or the chapter is intentionally designed as a short transitional/interlude chapter.

### Memory

- Only affected state files are updated.
- If a new numbered file was created, `INDEX.md` Layer D was updated to include it.

### Retrieval integrity

- If `INDEX.md` was consulted, it was treated as a lookup aid only — no fact from it was used as a tiebreaker over the actual authority order in §4 of this document.

If any check fails, revise before output.

---

# 29. FINAL PRINCIPLE

The Architect is not primarily a story about becoming powerful.

It is a story about:

- building something worth protecting
- loving someone enough to make impossible choices
- living with those choices
- accepting that what you build eventually belongs to future generations
- discovering that the difference between a Builder and an Architect was never merely what he could build

Write so that readers remember the people, not merely the events.
