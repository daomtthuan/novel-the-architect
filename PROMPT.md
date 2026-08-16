# Generate Chapter + Continuity Update Package

Generate the next chapter of **The Architect** according to all project instructions, canon, chronology, character rules, writing rules, and continuity requirements.

---

# PRIMARY TASK

Your task has TWO outputs:

1. Generate the complete new chapter in markdown block.
2. After generating the chapter, determine every knowledge/continuity file whose content must change because of the new chapter, and provide the **COMPLETE UPDATED VERSION** of each affected file.

You are NOT allowed to directly modify repository files.

I will manually review your proposed updates and then copy/overwrite the files myself.

Think of this as:

> **Chapter Generation → Continuity Analysis → Full File Replacement Package**

Do NOT treat the continuity update as optional.

---

# PART 1 — GENERATE THE CHAPTER

Follow `13-chapter-generation-protocol.md`.

Before writing:

1. Read `29-agent-memory.md`.
2. Read the relevant canon files.
3. Read `world_calendar.md` for exact WC chronology and age calculations.
4. Read `02-timeline.md` for narrative timeline context.
5. Read relevant character files.
6. Read relevant relationship files.
7. Read relevant world/faction/magic/technology files.
8. Read relevant mystery/foreshadowing files.
9. Read relevant continuity/state files.
10. Read relevant romance files if romance or relationship development is present.
11. Read relevant OST files if music is used or affected.
12. Read relevant illustration/visual files if the chapter contains a visually significant scene.

Do not blindly load every file if it is irrelevant.

However, after drafting, perform a **second continuity-impact pass** against the full knowledge-base structure.

---

# PART 2 — CONTINUITY IMPACT ANALYSIS

After the chapter is written, analyze the chapter as if it were a new canonical event.

For EVERY meaningful fact introduced, changed, revealed, established, or resolved by the chapter, determine whether an existing project file should reflect that information.

Check at minimum:

## Chronology

- `world_calendar.md`
- `02-timeline.md`

Update these if the chapter introduces or changes a canonical event, date, age, ordering, historical event, or WC entry.

`world_calendar.md` remains the master chronology authority.

Never invent or silently alter WC dates.

---

## Core Canon

Check:

- `00-story-bible.md`
- `01-canon-rules.md`
- `09-season-arc-outline.md`

Only propose updates if the chapter establishes a fact that genuinely belongs in these files.

Do not add temporary scene details to the Story Bible merely because they occurred.

---

## Characters

Check:

- `03-characters.md`
- `14-character-psychology.md`
- `15-character-voice.md`
- `16-character-development-log.md`
- `17-character-secrets.md`
- `36-secondary-heroines.md`
- `46-iconic-dialogue-registry.md`

Update only the files whose canonical information has actually changed.

Examples:

- A permanent character trait is established → `03` / `14`
- Character speech pattern materially evolves → `15`
- Character development milestone → `16`
- New secret or knowledge ownership → `17`
- Secondary heroine development → `36`
- A genuinely iconic recurring line is established → `46`

Do not force every chapter into all character files.

---

## Relationships / Romance

Check:

- `04-relationships.md`
- `35-romance-subplot-engine.md`
- `36-secondary-heroines.md`
- `37-relationship-state-machine.md`
- `38-romance-integration-by-season.md`
- `39-fanservice-scene-library.md`
- `40-romance-foreshadowing-map.md`
- `41-romance-agent-rules.md`
- `42-romance-continuity-memory.md`

Only update relationship/romance files when the chapter creates an actual state change, new established pattern, meaningful milestone, or canonical relationship information.

Do NOT artificially increase romance state merely because characters interact.

For Iris in particular, strictly preserve the established chronology and adulthood rules.

---

## World / Location / Organization

Check:

- `05-world.md`
- `06-factions-and-politics.md`
- `22-location-registry.md`
- `23-organization-registry.md`
- `18-event-consequence-map.md`

Update when the chapter establishes:

- a new permanent location
- a new organization
- political changes
- faction relationships
- institutional changes
- lasting consequences
- economic/social consequences
- important historical facts

Do not turn temporary scene details into permanent world canon unless justified.

---

## Magic / Technology / Artifacts

Check:

- `07-magic-and-technology.md`
- `08-multiverse-and-quantum-lore.md`
- `24-artifact-registry.md`
- `25-technology-evolution.md`

Update when the chapter introduces or materially changes:

- magic rules
- magical capabilities
- technology
- technological progression
- artifacts
- Builder/Architect lore
- Quantum Anchor information
- Other Builder information
- other permanent mechanics

Respect revelation timing.

Do NOT reveal information earlier than permitted by:

`11-foreshadowing-and-revelations.md`

---

## Mysteries / Antagonists / Foreshadowing

Check:

- `11-foreshadowing-and-revelations.md`
- `26-mystery-board.md`
- `27-conflict-and-antagonist-board.md`
- `28-unresolved-threads.md`

Update when the chapter:

- creates a new mystery
- advances an existing mystery
- provides a clue
- changes a mystery state
- resolves an unresolved thread
- creates a new unresolved question
- introduces an antagonist or conflict
- establishes future foreshadowing

Do not mark a mystery as confirmed merely because the reader has received a clue.

Respect the project's knowledge states:

`UNKNOWN → HINTED → SUSPECTED → PARTIALLY REVEALED → CONFIRMED → PUBLIC KNOWLEDGE`

---

## Continuity / Memory

Check:

- `12-continuity-tracker.md`
- `18-event-consequence-map.md`
- `19-emotional-memory.md`
- `20-scene-memory.md`
- `21-dialogue-memory.md`
- `28-unresolved-threads.md`
- `29-agent-memory.md`
- `42-romance-continuity-memory.md`
- `44-ost-continuity.md`

These files are especially important.

If the chapter changes story state, the corresponding state/memory file must be considered for update.

Track:

- character state
- emotional state
- relationship state
- injuries
- promises
- deaths
- world state
- political state
- objects
- locations
- mysteries
- unresolved questions
- important dialogue
- emotional memories
- scene memories
- romance continuity
- OST continuity

Do not silently change established canon.

---

## Visual / Illustration Continuity

Check:

- `30-visual-bible.md`
- `31-illustration-registry.md`
- relevant files under `character_design/`

If the chapter establishes a visually canonical change or a canonical illustration candidate, determine whether these files need updating.

Do not generate images.

Do not invent visual changes merely because a scene can be illustrated.

---

## OST

Check:

- `43-ost-reference.md`
- `44-ost-continuity.md`
- relevant files under `ost/`

Only update these when the chapter actually establishes, uses, changes, or canonizes music-related information.

Do not invent an OST assignment simply because a scene is emotional.

---

# CRITICAL RULE — FULL FILE REPLACEMENT

For every file that requires an update, output the **ENTIRE FILE**, from the first line to the last line.

Never output:

- a diff
- a patch
- only changed sections
- excerpts
- "replace this paragraph"
- "append this section"
- "insert below..."
- "unchanged sections omitted"
- `...`
- placeholders
- pseudo-content

I need a complete file that I can copy and overwrite directly.

The output must be valid Markdown and must preserve the existing file's structure unless a structural change is genuinely necessary.

If a file is 500 lines long and only one line changes, output all 500 lines with the change incorporated.

---

# DO NOT UPDATE FILES UNNECESSARILY

Do not produce updated versions of files that are unaffected.

The goal is:

> **minimum necessary file set, maximum continuity accuracy**

A file should be included only if the new chapter genuinely changes or adds information that belongs in that file.

For each affected file, explain briefly WHY it needs updating before showing its complete replacement.

---

# IMPORTANT DISTINCTION

Separate these concepts:

### Chapter-local information

Information that only matters inside this chapter.

Examples:

- temporary atmosphere
- temporary gestures
- incidental descriptions
- one-time sensory details
- transient thoughts
- ordinary conversation

Do NOT automatically put these into knowledge files.

### Canonical information

Information that should remain true after the chapter.

Examples:

- permanent character development
- relationship state changes
- new historical facts
- new locations
- new organizations
- new magic rules
- new technology
- new artifacts
- permanent injuries
- deaths
- political consequences
- important secrets
- unresolved mysteries
- established emotional memories
- canonical dialogue
- canonical visual changes

These SHOULD be reflected in the appropriate knowledge files.

---

# NO SILENT CANON CHANGES

Before finalizing the chapter:

Check every new fact against existing canon.

If the chapter would require contradicting existing canon:

1. Do NOT silently rewrite the canon.
2. Do NOT choose whichever version seems more convenient.
3. Identify the contradiction.
4. Stop and clearly report it before presenting the final chapter, if the contradiction materially affects the chapter.

If the contradiction can be resolved by an already-established authority rule, follow the authority hierarchy.

The authority hierarchy is:

1. Current explicit user instruction
2. Hard safety constraints
3. `world_calendar.md` for chronology and age math
4. `00-story-bible.md`
5. `01-canon-rules.md`
6. Explicit revision/update records
7. Relevant domain canon files
8. Relevant continuity/state files
9. Creative inference

State files must never silently override established canon.

---

# CHAPTER OUTPUT FORMAT

First output the complete chapter using the project's established chapter format:

# Chapter N — Title

[Complete chapter prose]

---

## Chapter Metadata

- Installment:
- WC year:
- POV:
- Location:
- Characters (with computed ages):
- Conflict:
- Emotional objective:
- Plot objective:

## Continuity Update

- New facts:
- Character changes:
- Relationship changes:
- World changes:
- New objects:
- New locations:
- Foreshadowing:
- Revealed secrets:
- Unresolved questions:

---

# THEN OUTPUT A CONTINUITY UPDATE PACKAGE

After the chapter, output:

# Continuity Update Package

## 1. Files That Must Be Updated

List ONLY files that genuinely require modification.

For each file:

- File:
- Reason:
- Type of change:
  - Canon
  - Timeline
  - Character
  - Relationship
  - World
  - Lore
  - Mystery
  - Continuity
  - Memory
  - Romance
  - Visual
  - OST

Do not include unaffected files.

---

# 2. Complete Updated Files

For every affected file, output:

## `path/to/file.md`

Brief explanation of what changed.

Then provide the COMPLETE replacement file:

```md
[ENTIRE FILE CONTENT]
```

The Markdown inside the code block must be complete and directly copyable.

Repeat this for every affected file.

---

# 3. Files That Were Checked but Do Not Need Updates

At the end, provide a concise list of important files that were checked but intentionally left unchanged.

For example:

- `03-characters.md` — no permanent character profile change.
- `05-world.md` — no permanent world-state change.
- `07-magic-and-technology.md` — no new magic rule.
- `28-unresolved-threads.md` — no new unresolved thread.

Do not list every file in the repository. Only list the relevant files that were actually considered during continuity analysis.

---

# FINAL VALIDATION

Before returning the answer, perform a final internal audit:

### Canon

- No canon contradiction.
- No invented protagonist personal name.
- No accidental Builder/Architect terminology misuse.

### Chronology

- WC is correct.
- Ages are calculated from the canonical aging system.
- Event ordering is correct.

### Character

- Character psychology matches current development state.
- Character voice matches established voice.
- Relationships match current state.

### Romance

- Elena remains primary heroine.
- Secondary attraction does not become automatic love.
- Iris's chronology and adulthood restrictions are respected.
- No inappropriate romantic framing.

### Lore

- Magic and technology follow established rules.
- Builder/Architect lore is not prematurely exposed.
- Mystery revelation levels are respected.

### Continuity

- Every permanent new fact has a home in the appropriate continuity/canon file.
- No important state change was omitted.
- No irrelevant file was changed.

### File Replacement Integrity

- Every proposed update is a COMPLETE file.
- No omitted sections.
- No `...`.
- No placeholders.
- No pseudo-diffs.
- No instructions such as "insert this".
- Existing content is preserved unless intentionally changed.
- The output can be copied directly over the original file.

### Most Important Rule

**Do not merely tell me what files I should update.**

You must provide the **complete updated contents of those files**.

I should be able to perform this workflow:

1. Copy the generated chapter into `chapters/`.
2. Review each proposed continuity file.
3. Copy each approved complete file.
4. Overwrite the corresponding repository file.
5. Commit everything.

No manual merging should be required.

### WRITING FORMAT

- Chapter titles are written in English.
- Chapter body content is written in Vietnamese.
- Story-specific terminology may remain in English, but must be used sparingly and naturally.
- Avoid unnecessary English wording when a Vietnamese expression reads more naturally.
- Narrative prose targets approximately **3,000–3,500 Vietnamese words**.
- Preferred center is approximately **3,250 words**.
- Normal acceptable range is **2,800–3,700 words**.
- `Chapter Metadata` and `Continuity Update` are excluded from the word count.
- Chapter length should be calibrated for approximately 15–30 minutes of AI narration.
- Prioritize narrative quality, pacing, emotional rhythm, and scene completeness over hitting an exact word count.
- Do not artificially inflate the chapter with exposition merely to reach the target narration duration.
