# The Architect — AI Write Agent Knowledge Base

Version: 7

This directory is the complete knowledge base and asset library for **The Architect**.

The project is organized so that the AI Write Agent can retrieve the smallest relevant set of files instead of loading everything blindly.

---

# 1. ENTRY POINTS

## `INSTRUCTIONS.md`

The **agent orchestrator**.

It defines:

- authority rules
- retrieval behavior
- chronology rules
- writing workflow
- continuity validation
- romance/age rules
- OST rules
- visual rules
- memory update rules

The agent should consult `INSTRUCTIONS.md` before performing a canon-sensitive writing task.

## `README.md`

The **knowledge-base index**.

It tells the agent what each file and asset group is for.

It is a navigation/reference document, not a replacement for the underlying source files.

## `world_calendar.md`

The **master World Calendar**.

It is authoritative for:

- WC years
- chronological ordering
- event dates
- age calculations
- historical timing

`02-timeline.md` provides the detailed narrative timeline and context.

---

# 2. AUTHORITY MODEL

When sources conflict:

1. Current explicit user instruction
2. Hard safety constraints
3. `world_calendar.md` for dates and ages
4. `00-story-bible.md` + `01-canon-rules.md`
5. Explicit revision files for the facts they revise
6. Relevant domain canon
7. Continuity/state memory
8. Creative inference

Do not resolve important conflicts silently.

`29-agent-memory.md` is mutable state, not superior canon.

---

# 3. CORE STORY CANON

These establish the foundation of the saga:

- `00-story-bible.md` — story premise, themes, central identity
- `01-canon-rules.md` — hard canon constraints
- `02-timeline.md` — detailed chronological timeline
- `03-characters.md` — canonical character profiles
- `04-relationships.md` — relationship structure
- `05-world.md` — world rules, peoples, cultures and geography
- `06-factions-and-politics.md` — factions, countries and political structures
- `07-magic-and-technology.md` — magic and technology foundations
- `08-multiverse-and-quantum-lore.md` — Builder, multiverse and deep lore
- `09-season-arc-outline.md` — Season 1 + four-movie macro structure

---

# 4. WRITING / STORY PROCEDURES

- `10-light-novel-writing-guide.md` — prose and light-novel writing style
- `11-foreshadowing-and-revelations.md` — mystery/reveal/foreshadowing procedure
- `12-continuity-tracker.md` — continuity tracking
- `13-chapter-generation-protocol.md` — chapter generation procedure

Procedural files explain **how to write**. They should not silently override canon.

---

# 5. CHARACTER INTELLIGENCE

- `14-character-psychology.md` — psychology, wounds, desires, fears, contradictions
- `15-character-voice.md` — dialogue/speech patterns
- `16-character-development-log.md` — chronological character development
- `17-character-secrets.md` — secrets and who knows them

For a major character, combine the static profile with psychology, voice, development and secrets.

---

# 6. NARRATIVE MEMORY / CONTINUITY

- `18-event-consequence-map.md` — event → downstream consequences
- `19-emotional-memory.md` — lasting emotional consequences
- `20-scene-memory.md` — established scene facts
- `21-dialogue-memory.md` — established important dialogue
- `28-unresolved-threads.md` — unresolved/open story threads
- `29-agent-memory.md` — mutable operational agent memory

These files preserve state.

They must be interpreted against canonical files.

---

# 7. WORLD CONTINUITY REGISTRIES

- `22-location-registry.md` — location-specific facts
- `23-organization-registry.md` — organization-specific facts
- `24-artifact-registry.md` — artifact-specific facts
- `25-technology-evolution.md` — technology progression and consequences

---

# 8. PLOT CONTROL

- `26-mystery-board.md` — mystery state and reveal tracking
- `27-conflict-and-antagonist-board.md` — antagonist/conflict state
- `28-unresolved-threads.md` — unresolved plot threads

For mystery work, normally combine `11 + 26 + 28`.

For antagonist/conflict work, normally combine `27 + 06 + 18 + 28`.

---

# 9. VISUAL SYSTEM

- `30-visual-bible.md` — canonical visual language/design
- `31-illustration-registry.md` — illustration history and continuity
- `32-image-generation-protocol.md` — image generation rules
- `33-reader-immersion.md` — reader-facing visual/narrative framing

## Character design assets

Directory:

`character_design/`

Files:

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

When generating or describing an established character visually, consult the relevant image plus `30`, `31`, `32`, character canon and chronology.

---

# 10. ROMANCE / HAREM / FAN-SERVICE

- `34-romance-harem-fanservice.md` — overall romance/fanservice rules
- `35-romance-subplot-engine.md` — romance subplot mechanics
- `36-secondary-heroines.md` — Iris, Seraphine, Isolde
- `37-relationship-state-machine.md` — formal relationship states/transitions
- `38-romance-integration-by-season.md` — romance by installment
- `39-fanservice-scene-library.md` — approved scene patterns
- `40-romance-foreshadowing-map.md` — romance setup/foreshadowing
- `41-romance-agent-rules.md` — operational romance rules
- `42-romance-continuity-memory.md` — current romance state

For romance, do not read only one file. Use the relevant combination.

Core romance is **The Architect × Elena** unless explicitly changed by the user.

---

# 11. OST SYSTEM

## Reference

`43-ost-reference.md`

Contains the project's canonical OST mapping, meanings and intended emotional use.

## Continuity

`44-ost-continuity.md`

Tracks OST state, including:

- used tracks
- reserved tracks
- single-use tracks
- locked tracks
- emotional associations
- continuity restrictions

## Actual audio

Directory:

`ost/`

Tracks:

- `ost/01. The Architect's Theme - The Architect.mp3`
- `ost/02. The Architect's Theme - A Place to Stay.mp3`
- `ost/03. Elena's Theme - Her Quiet Light.mp3`
- `ost/04. The Ark - The Ark Awakens.mp3`
- `ost/05. The Ark - Activation.mp3`
- `ost/06. Ark Countdown - Her Choice, My Silence.mp3`
- `ost/07. Empty House.mp3`
- `ost/08. Home.mp3`
- `ost/09. The Last Observer - The Truth.mp3`

The `.mp3` files are actual assets.

Do not invent musical characteristics merely from filenames.

Use `43` for semantic/emotional meaning and `44` for usage continuity.

OST information is internal writing guidance and should not appear as metadata in prose unless the user explicitly asks for it.

---

# 12. CANON REVISION

`45-session-update-wc16-revision-and-worldbuilding.md`

This is a **revision/update record**.

Use it when a task touches:

- WC16
- facts explicitly revised in this document
- worldbuilding introduced/changed by this document

It does not automatically override unrelated canon.

---

# 13. ICONIC DIALOGUE

`46-iconic-dialogue-registry.md`

Contains established iconic/signature dialogue.

For dialogue callbacks, combine:

- `46`
- `15-character-voice.md`
- `21-dialogue-memory.md`

Do not casually alter an iconic line when doing so changes its identity or meaning.

---

# 14. CHARACTER RETRIEVAL

For a character:

```text
03-characters
14-character-psychology
15-character-voice
16-character-development-log
17-character-secrets
```

Then add:

```text
04-relationships
46-iconic-dialogue-registry
```

when relevant.

Always consider the character's current WC state.

---

# 15. TIMELINE RETRIEVAL

For dates/ages:

```text
world_calendar.md
02-timeline.md
```

Then cross-check:

```text
00-story-bible.md
12-continuity-tracker.md
45-session-update-wc16-revision-and-worldbuilding.md
```

when relevant.

`world_calendar.md` wins for chronology and age math.

---

# 16. EVENT RETRIEVAL

For continuation of an existing event:

```text
18-event-consequence-map.md
20-scene-memory.md
28-unresolved-threads.md
```

Add:

```text
19-emotional-memory.md
21-dialogue-memory.md
```

when relevant.

---

# 17. MYSTERY RETRIEVAL

Use:

```text
11-foreshadowing-and-revelations.md
26-mystery-board.md
28-unresolved-threads.md
17-character-secrets.md
```

Do not reveal a mystery earlier than its intended reveal state.

---

# 18. RELATIONSHIP RETRIEVAL

Use:

```text
04-relationships.md
37-relationship-state-machine.md
42-romance-continuity-memory.md
```

For romance/fanservice, add the relevant files from `34`–`41`.

---

# 19. WORLD / POLITICS RETRIEVAL

### Location

```text
05-world.md
22-location-registry.md
```

### Organization / faction

```text
06-factions-and-politics.md
23-organization-registry.md
```

### Artifact

```text
24-artifact-registry.md
07-magic-and-technology.md
```

### Technology

```text
07-magic-and-technology.md
25-technology-evolution.md
06-factions-and-politics.md
18-event-consequence-map.md
```

### Builder / multiverse

```text
08-multiverse-and-quantum-lore.md
11-foreshadowing-and-revelations.md
26-mystery-board.md
28-unresolved-threads.md
```

---

# 20. VISUAL RETRIEVAL

For character design:

```text
30-visual-bible.md
31-illustration-registry.md
32-image-generation-protocol.md
character_design/<relevant asset>
```

Then cross-check:

```text
03-characters.md
world_calendar.md
33-reader-immersion.md
```

Do not casually redesign recurring characters.

---

# 21. OST RETRIEVAL

For a scene requiring music:

```text
43-ost-reference.md
44-ost-continuity.md
```

Then optionally:

```text
19-emotional-memory.md
20-scene-memory.md
ost/<relevant mp3>
```

Never assign a track that violates the continuity state.

---

# 22. AGENT MEMORY

`29-agent-memory.md` is mutable short-term/operational state.

Read it early in a writing session.

It can contain:

- recent decisions
- recent continuity state
- warnings
- retrieval hints

It can become stale.

Therefore, it never silently overrides:

- user instruction
- hard safety
- `world_calendar.md`
- core canon

---

# 23. RECOMMENDED AGENT FLOW

For a new chapter:

```text
1. Read INSTRUCTIONS.md
2. Read 29-agent-memory.md
3. Read 12-continuity-tracker.md
4. Establish installment + WC + POV + location + characters
5. Check world_calendar.md
6. Retrieve only relevant domain files
7. Check revision file when applicable
8. Write using the writing procedures
9. Validate continuity
10. Update only affected state files
```

Do not load all project files blindly.

---

# 24. IMPORTANT CANON REMINDERS

- The protagonist has no personal name.
- “The Architect” is a title earned at WC35.
- “Builder” and “Architect” are not synonymous.
- Season 1 is first-person Architect POV.
- Elena is the primary heroine and emotional center.
- Iris, Seraphine and Isolde are secondary heroines.
- Romance must never displace Elena's central role.
- No romantic/sexualized framing of a character before textual adulthood.
- `world_calendar.md` is the master chronology.
- `29-agent-memory.md` is mutable state.
- OST is internal writing guidance unless explicitly requested otherwise.
- Established visual designs must remain consistent.
