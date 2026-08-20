# Continuity Tracker (v12, World Calendar canon)

Updated after every accepted chapter/scene.

## Purpose

This is the durable continuity ledger. Unlike `29-agent-memory.md`, which stores only the current mutable handoff state, this file preserves the accepted chapter-by-chapter history.

## PRE-WRITING HANDOFF PROTOCOL — MANDATORY

Before writing a new chapter, the agent MUST retrieve the metadata of the **immediately previous accepted chapter**.

Required order:

1. Read `29-agent-memory.md`.
2. Read this tracker and identify the latest accepted chapter.
3. Locate that chapter file by chapter number/title.
4. Read its `## Chapter Metadata` and `## Continuity Update`.
5. Extract the handoff state: WC/time, location, POV, characters, conflict, emotional/plot objective, new facts, character/relationship/world changes, objects, foreshadowing, secrets, and unresolved questions.
6. Use that handoff as the starting state for the next chapter.
7. If metadata is insufficient, inspect the previous chapter prose and then the relevant immutable canon files.
8. Only after the handoff is established should the agent draft the new chapter.

### Mandatory handoff questions

Before drafting, the agent must be able to answer:

- What is the exact or bounded WC year at the start?
- How old is each active character under the Aging Rate System?
- Where did the previous chapter end?
- Who was physically present at the end?
- What relationships changed?
- What new knowledge did each relevant character gain?
- What remains unknown to each character?
- Which foreshadowing threads remain active?
- Which objects/locations/injuries/promises must carry forward?
- What is the most natural immediate consequence of the previous chapter?

If any answer is unknown, **do not invent it silently**. Search the source files first.

### Continuity chain

Use the shortest sufficient chain:

`29-agent-memory.md`
→ `12-continuity-tracker.md`
→ **immediate previous chapter metadata**
→ earlier chapter metadata when needed
→ immutable canon / `world_calendar.md`
→ relevant supporting knowledge files

The agent does NOT need to reread all chapters every time. The purpose of this protocol is to make the immediate previous chapter's metadata the explicit handoff contract.

---

## Accepted Chapter Records

### Chapters 1–13

*(Unchanged — see prior tracker version for full records of Chapters 1 through 13, from "Awaken" (WC0) through "Learning to Aim" (WC17). All facts, character/relationship/world changes, foreshadowing, and handoffs recorded there remain in force.)*

### Chapter 14 — What Cannot Be Optimized

- **Installment:** Season 1 — The Architect
- **WC:** WC18
- **POV:** The Architect, first-person
- **Location:** Southwestern ravine (Guild mission site); Architect's family home; front porch
- **Characters:** The Architect (18), Elena (24.5), Iris (15), The Guild Master, unnamed political delegation (two Kingdoms + one northern Empire)
- **Core conflict:** External — an unauthorized, underreported hazard-B Guild mission nearly kills the Architect; a political delegation attempts coercion and threatens his loved ones. Internal — the WC18 major argument with Elena directly names his defense mechanism as "becoming the monster"; first on-page loss of emotional control.
- **Emotional objective:** Deliver the WC18 major argument in full, as a genuine rupture rather than another gentle warning; establish Iris's shift to active, undisclosed protection; introduce a new external political threat that escalates the stakes of the Architect's isolation.
- **Plot objective:** Dramatize WC18 per `world_calendar.md` ("Architect tiếp tục nghiên cứu nhưng trở nên lạnh lùng... ông và Elena đã cãi nhau lớn"); establish new political-pressure thread (Kingdoms/Empire attempting to weaponize the Architect); give Iris a real sword and a new protective role.
- **New facts:** Architect takes an unauthorized hazard-B mission, misreports the threat count (three reported, eight actual), nearly dies, self-rescues via an improvised wide-area sealing structure rather than repeating his WC16 body-conduit mistake. Iris secretly shadows him with a real steel sword (newly given by the blacksmith), watches the full fight, deliberately does not intervene. Elena discovers both the reckless mission and continued solo nighttime pathway testing; the WC18 argument occurs in full, culminating in Elena's line comparing him to the monster that killed his parents; Elena moves out of the shared home. Three days later, a political delegation from two Kingdoms and a northern Empire attempts to coerce the Architect into weaponizing his research, threatens Elena and Iris directly, and is met with an uncontrolled, intimidating Mana outburst and an explicit warning from the Architect. That night, Iris commits to ongoing, undisclosed protective shadowing.
- **Character changes:** **PERMANENT (relational):** Elena moves out of the Architect's home — the first genuine rupture in their relationship, not merely tension. **PERMANENT:** the Architect demonstrates, for the first time on-page, a loss of emotional control (the Mana outburst) distinct from his usual calculation-based coping — a new and more dangerous failure mode. Iris is entrusted with a real steel sword and formally shifts from indirect to active, undisclosed protection.
- **Relationship changes:** Architect ↔ Elena ruptures — she moves out following the major argument; this is the direct, unresolved bridge to the already-logged WC19 reconciliation. Architect ↔ Iris deepens through her new protective commitment, still strictly platonic (age 15). Architect ↔ political delegation begins as a new, hostile relationship thread.
- **World changes:** First on-page instance of political coercion targeting the Architect's research for military use; early seed for the pro-/anti-/neutral-Architect factions that solidify around WC31.
- **New objects:** Iris's real steel sword (given by the village blacksmith) — added to `24-artifact-registry.md`.
- **New locations:** Southwestern ravine — non-registry unless it recurs.
- **Foreshadowing:** The Architect's uncontrolled Mana outburst foreshadows the controlling, intimidation-adjacent systems of the Darkest Point later dismantled in The Reform (~WC48–52). The political delegation's coercion attempt foreshadows the political faction formation of WC31. Iris's shift to active protection is a new through-line for future chapters.
- **Revealed secrets:** None. WC16 Demon reveal discipline unaffected.
- **Unresolved questions:** Where Elena goes after moving out; how/when WC19 reconciliation occurs on-page; identity of the political delegation's Kingdoms/Empire; whether the Architect ever learns Iris witnessed the full ravine fight without intervening.
- **Handoff to Chapter 15:** The Architect is alone in his home for the first time since WC16 (Elena moved out); Iris has committed to undisclosed protective shadowing; the WC19 reconciliation with Elena is the next expected major beat, alongside possible further political-delegation consequences.

---

## Required Chapter Record

Every accepted chapter record MUST contain:

chapter number · installment · WC year/range · location · POV · characters present · characters absent but relevant · conflict · emotional objective · plot objective · new facts · character changes · political changes · relationship changes · injuries · deaths · promises · unresolved questions · foreshadowing · secrets revealed · objects · organizations · end-state / handoff to next chapter

## Character State

Track: age (computed via the Aging Rate System); physical condition; emotional state; current goal; current belief; relationship state.

**Post-Chapter-14 note:** The Architect's coping pattern has produced a new failure mode — uncontrolled emotional/Mana outburst under threat to loved ones — that should be tracked alongside the existing "calculation instead of grief" pattern as the Darkest Point continues escalating toward its WC22 low point.

## World State

Track: city status; political alliances; wars; economy; magical infrastructure; technology level; institutions.

**Post-Chapter-14 note:** A new political threat exists — an unnamed coalition of two Kingdoms and a northern Empire attempting to coerce the Architect militarily, now hostile after his warning.

## Lore State

UNKNOWN → HINTED → SUSPECTED → PARTIALLY REVEALED → CONFIRMED → PUBLIC KNOWLEDGE

Apply this specifically to: the Builder concept, the Architect/Builder distinction, the Quantum Anchor, the Other Builder's existence, fragmentary Demon-activity rumors (status: HINTED, unchanged by Chapter 14).

## Relationship State

For primary romantic characters (Elena):

STRANGER → ACQUAINTANCE → TRUST → FRIEND → LOVE → PARTNER → CONFLICT → RECONCILIATION → FAMILY → LOSS

**Post-Chapter-14 note:** Architect ↔ Elena is now at CONFLICT, having ruptured following the WC18 major argument; RECONCILIATION (WC19) is the next expected state.

For secondary romantic characters (Iris, Seraphine, Isolde):

ATTRACTION → FLIRTATION → MUTUAL CHEMISTRY → UNREQUITED LOVE → ACCEPTANCE

Iris's track must show no ATTRACTION entries before she is an adult (~WC21).

## Update Rule

- Do not silently change established canon.
- Continuity updates must be explicit.
- Only accepted chapters/scenes enter the durable tracker.
- Drafts do not update the tracker.
- When a contradiction is discovered, flag it instead of silently rewriting history.
- If a later chapter intentionally revises canon, record the revision explicitly with its reason and affected records.
